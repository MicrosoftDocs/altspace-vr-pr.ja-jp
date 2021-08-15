---
title: glTF モデルのインポート
description: 3D glTF モデルを AltspaceVR エクスペリエンスに適切にインポートし、問題のトラブルシューティングを行う方法について説明します。
ms.date: 03/11/2021
ms.topic: article
keywords: モデル, glTF, インポート, スケッチハブ, トラブルシューティング
ms.openlocfilehash: 527c38fc49028258fa432445fe14a355710a18be65ee74252a8c39bc1bfe5190
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127062"
---
# <a name="importing-gltf-models"></a>glTF モデルのインポート

> [!NOTE]
> この機能は、現時点では早期アクセス プログラムの一部のユーザーが使用できます。

3D モデルとシーンを Altspace に取り込む方法の 1 つは [、glTF 標準 を使用する方法です](https://en.wikipedia.org/wiki/GlTF)。 .glb ファイル (パックされた glTF) をアップロードして、後でワールド エディターで生成できるモデルを作成できます。 独自のキット をアップロード [する代わりに使用できます](uploading-custom-kits.md)。 パフォーマンスと再利用性を最大限に高める必要がある場合は、Unity と Kits を使用する必要がないので、簡単なデモ用にモデルを作成することをお勧めします。 

1. いくつかの glTF 3D アセットを見つける。 検索する場所の 1 つは、Sketchfab です (このようなダウンロード可能な **モデルのフィルター** 処理を [試してください](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models))。 見つけたら **、[3D モデルのダウンロード] を選択します**。

![Sketchfab の 3D 犬モデル](images/importing-models-img-01.png)

2. モデルへのリンクをコピーし、ライセンス要件を読み取る。 
3. 自動変換 **形式 (glTF) バージョンをダウンロード** する

![自動変換形式が強調表示された Sketchfab ダウンロード オプション](images/importing-models-img-02.png)

4. [GLB Packer サイトを開き](https://glb-packer.glitch.me)、[PNG を JPEG に **変換する (ベータ版)** ] チェック ボックスをオンにします
5. ダウンロードした glTF ファイルの圧縮を解除し、一度にすべて GLB Packer ブラウザー タブにドラッグします

![モデルの圧縮解除を示すウィンドウ](images/importing-models-img-03.png)

6. ファイルの数とサイズによっては、処理に時間がかかる場合があります。 処理が完了すると **、out.glb ファイル** がダウンロードされます。 そのファイルの名前を情報に変更します。これは、世界のオブジェクトの名前になります (例: **Low Poly Rename.glb**)
7. [その他 altvr.com > [モデル>移動し、[](https://account.altvr.com/users/sign_in) 作成] を **選択します**
8. .glb ファイルの場所を指定し、属性の説明に Sketchfab リンクをコピーしてください。 必要に合ってプレビュー イメージを指定し、 [モデルの作成] **を選択します**。

![AltspaceVR のモデル プレビュー](images/importing-models-img-04.png)

9. [クリップボード **にコピー] を選択する**
10. **[World Editor]/(ワールド エディター> Altspace > Basics > GLTF**
11. URL を貼り付け、[確認] を **選択します**

おめでとうございます! 最初のモデルを生成したばかりです。

## <a name="troubleshooting"></a>トラブルシューティング

**[何も起こ **っていないことを確認** する] をクリックした場合**
    * 現在、100,000 の多角形の制限があります。 失敗した場合は、 オブジェクトを削除して、World に参加しているユーザーに関する潜在的な問題を回避します
    * 資産に他の問題がある可能性があります。 可能な限り少ない多角形のアセットを使用してみてください。
    * 取り込むモデルは、小さい場合も大きい場合があります。 スケールを増減したり、アバターを動かしたりしてみてください。モデル内に立っている可能性があります。

**読み込み速度が遅い** ワールド内の他のユーザーが読み込む速度は、接続速度によって異なっています。 また、Kit アセットのようにキャッシュされません。 ホームに配置すると、参加するごとに同じモデルが再ダウンロードされます。これは良いではありません。

**競合がない** 既定では、この方法で取り込まれるオブジェクトに競合はありません

**生成すると、6** つの DOF でコントロールが失われるか、内部にあるので操作が難しいはい。これらの問題を認識し、すぐに対処する予定です。  