---
title: 世界ビルの Toolkit を紹介する
description: Unity シーンテンプレートを使用して、世界ビルの Toolkit で、Altを設定してアップロードする方法について説明します。
ms.date: 03/11/2021
ms.topic: article
keywords: toolkit
ms.openlocfilehash: 8b66e35509060e00b2e52d3770380d009d7060339003f534d23fdd47372a57f0
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "119125408"
---
# <a name="introducing-the-world-building-toolkit"></a>世界ビルの Toolkit を紹介する

> [!NOTE]
> 世界ビルの Toolkit は、当社のすばらしい友人である[Anthony madden](https://twitter.com/chigamesstudio)によって実行されるコミュニティプロジェクトです。 興味をお持ちの場合は、 [公式の Altspacevr Discord](https://discordapp.com/invite/altspacevr) に参加し、#world ビルディングチャネルにアクセスしてください。 現在、Mac 試用版ベータ版があります。詳細については、こちらを[参照](https://altvr.com/altspacevr-mac)してください。

アップローダーでは、Unity シーンを世界のテンプレートとして使用することができます。 Minecraft から、満塁の家にハロウィーンやお気に入りの作成を持ち込むことができます。 Unity にインポートできる場合は、この方法で Altspace にアクセスできる可能性があります。 いくつかの [例](https://account.altvr.com/worlds/1046572460192825569)を次に示します。

![ワールドの例](images/unity-uploader-img-01.png)

## <a name="setup"></a>セットアップ

1. 公式の [Altspacevr Discord](https://discordapp.com/invite/altspacevr) に参加して、#world ビルのチャネルにアクセスしてください。友人は、友人が自分だけをビルドすることはできません。
2. 基本については、 [世界ビルのはじめにガイド](world-building-getting-started.md) を参照してください。
3. [Unity Hub をインストール](https://blogs.unity3d.com/2018/01/24/streamline-your-workflow-introducing-unity-hub-beta) し、 **unity 2020.3.9** をインストールします。 このバージョンと正確に一致しない限り、アップローダーは機能しません。 お持ちでない場合は、無料の Unity アカウントが必要です 。このアカウントをお持ちでない場合は、無料でお試しください。 インストール中に、[ **Android のビルド** ] オプションをオンにして、自動更新を無効にしてください。
4. [最新の Unity アップローダーをダウンロードする](upgrading-content-to-the-latest-unity.md#altspacevr-uploader-v090-upgrade-guide)
5. Web サイトに[テンプレートを作成](https://account.altvr.com/space_templates/new)します。 **Hello World テンプレート** に名前を指定します。
6. **Hello World** という名前を [作成](https://account.altvr.com/worlds/my)します。 テンプレートとして [ **Hello World テンプレート** ] を選択します。

![作成されたワールド画面](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a>シーンのアップロード

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-a-Template/player]

1. Unity Hub を開き、新しい Unity 2020.3.9 プロジェクトを作成します。
2. プロジェクトを開いた状態で、ダウンロードしたファイル (Unity パッケージ) をダブルクリックしてアップローダーをインポートします。 これで、 **altと** いう新しいタブが表示されます。 Altspace で使用するすべての Unity プロジェクトのパッケージをインポートする必要があります。
3. **メニュー > alt> Build 設定** を開く
4. Altspace アカウントの資格情報でサインインします
5. [**テンプレートの読み込み**] を選択し、[ **Hello World テンプレート**] を選択します。
6. シーンにキューブを追加して保存します。
7. **Windows のビルド** を確認し、 **Android 用のビルドをオフにしますか**?
8. **[アップロード]** を選択します。 約1分で **アップロード** 完了したことがわかります。
9. Altspace を起動して **メニュー > ワールド >** を入力して **Hello World** 参加する
10. **メニュー > 設定 > 中 > 程度の間隔で領域** をリセットします。
11. キューブが表示されます。 上記のビデオのようにすばやく実行すると、10秒ほどではなく変更を確認できます。

## <a name="whats-supported"></a>サポートされる操作

* はい: モデル、競合、アニメーション、パーティクル効果、オーディオ、skyboxes など
* いいえ: スクリプト。 セキュリティ上の理由から、スクリプトを含むアップロードは拒否されます
* 場合によっては、動的なグローバル照明のような凝った
* 異なるプラットフォームのシーンを個別または組み合わせてアップロード
* アップローダーを使用して構築された、 [おすすめの世界](https://account.altvr.com/worlds/featured)をご覧ください

## <a name="tips"></a>ヒント

* 公式の [Altspacevr Discord](https://discordapp.com/invite/altspacevr)に参加します。
* 左側の [テンプレート] ページに、プラットフォーム別の最新のアップロードが表示されます。 成功した場合は、 **1-2 分前** に表示されます。Screen_Shot_2019-01-11 _at_1.21.04_AM.png

![アップロードが強調表示された状態で開く [テンプレート] パネル](images/unity-uploader-img-03.png)

* を更新するときに、その中でも使用できます。 アップローダーが **完了アップロード** と表示されたら、世界をリセットして変更を確認することができます。
* 簡単なシーンを使用した PC 用のビルドでは、Altspace の変化を確認するために1分未満でなければなりません。
* 取られるを避けるために、世界をプライベートに設定し、一覧から削除します。
* 既定でユーザーが生成する場所を確認できるように、キューブを配信元に配置します。 アップロード時にキューブを非表示にします。

## <a name="troubleshooting"></a>トラブルシューティング

**何かを挿入することはできません。** オブジェクトへの競合を追加して、それらにテレポートする必要があります。

**何も変更されません**
    * Unity にシーンを保存しましたか?
    * テスト対象のプラットフォームを選択しましたか?
    * お持ちの方は、 アップローダーと World 形式で適切なテンプレートを選択しましたか?
    * テンプレートページの統計情報を確認しましたか?

**アップロードの失敗またはタイムアウト**
    * 最も一般的なアップロードエラーの Unity バージョンが間違っています。 必要なバージョンと正確に一致している必要があります。
    * アップロードが大きすぎる可能性があります。 PC のシーン < 100 MB に保つようにしてください。 小規模に開始し、構築します。 Optimize、optimize、optimize。
    * 単純なキューブを使用して、新しいプロジェクトを試してください。
    * ビルド中に強制的に終了しないでください。シーンを破損させることができます。 再アップロードをお試しください。

**処理速度が遅い**
    * 後で Android を反復処理する場合にのみ、PC 用にビルドすることをお勧めします。
    * 未使用のファイルを削除してみてください。 何らかの理由により、Unity は熱心になることがあります。

**Altspace 資格情報でサインインできません**
    * 電子メールでは大文字と小文字が区別されます。
    * 新しいプロジェクトを試してみてください。
    * Altspace アカウントが良好な場所にあることを確認します。

## <a name="see-also"></a>関連項目

* [Unity の学習](https://unity3d.com/learn)
* [Unity フォーラム](https://forum.unity.com)
