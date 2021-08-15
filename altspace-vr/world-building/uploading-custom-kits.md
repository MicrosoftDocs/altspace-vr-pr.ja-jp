---
title: カスタム キットのアップロード
description: AltspaceVR で独自のカスタム キットを設定、生成、アップロードする方法とトラブルシューティングのヘルプについて説明します。
ms.date: 03/11/2021
ms.topic: article
keywords: キット、アップロード、トラブルシューティング
ms.openlocfilehash: 9a90bff2360d854dc398a35501f07cddcbce5c6c66ef8230f2e412a022f8aed0
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "119125528"
---
# <a name="uploading-custom-kits"></a>カスタム キットのアップロード

ワールド エディターには、ワールドにArtifactsを含むキットがあります。 たとえば [、Campfire Kit には多](https://account.altvr.com/kits/993516233267609824) くの種類のツリーがあります。ツリーの種類はアーティファクトです。 独自の Kit を作成するには、Unity AssetBundles を作成し、各成果物の Unity プレハブを含む .zip ファイルをアップロードし、各成果物を Web サイトに登録する必要があります。 さいわい、コミュニティ駆動型の Unity アップデータツールは、ワークフローの大部分を自動化します。 アップロードすると、Worlds 内の独自のキットからオブジェクトを生成できます。他のユーザーはそれらを自動的に表示できます。 後で、Kit を友人と共有したり、機能を利用してCommunity全体を共有したりすることもできます。

## <a name="prerequisites"></a>前提条件

1. [Unity Hub と Unity をインストールする](world-building-toolkit-getting-started.md)
2. 最新バージョンの Unity [Uploader をダウンロードする](https://altvr.com/download-latest-unity-uploader/)

## <a name="setup"></a>セットアップ 

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-1-Setup/player]

1. Worlds > Kits の Web サイトで [キットを作成する](https://account.altvr.com/kits)
2. ブラウザーのアドレス バーからクリップボードに Kit ID をコピーします (Uploader バージョン 0.9 以上では、この手順が簡単になります)
3. 新しい Unity テンプレートを作成Project
4. パッケージをダブルクリックして Unity Uploader をインポートする

![インポートされた Unity アップデータラー パッケージ](images/custom-kits-img-01.png)

5. Altspace の電子メールとパスワードを使用して Uploader にサインインします

![Unity の AltspaceVR サインイン インターフェイス](images/custom-kits-img-02.png)

## <a name="generate-and-upload-your-kit"></a>キットを生成してアップロードする

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-2/player]

1. [キット フォルダー **名**] には、プレフィックスとしてキット ID とテーマ **(1137484494681408069_pirates** など) を入力し、キットの資産名にプレフィックスとして Kit ID を入力します。 すべての資産には、このプレフィックスが必要です。

![Kit フォルダー名を使用した Unity の AltspaceVR インターフェイス](images/custom-kits-img-03.png)

2. アーティファクトまたは一連の成果物ごとにArtifacts。
* ソースのプレハブを [階層] タブにドラッグします
* セットに含めるもの (5 種類のけじなど) を選択します
* Kit **Asset Name をに更新****する**
* **[GameObject を Kit Prefab に変換する] を選択します**
* Assets/Prefabs フォルダーに新しいプレハブとスクリーンショットが作成されたのを確認します

![アーティファクトが選択された Unity の AltspaceVR インターフェイス](images/custom-kits-img-04.png)

> [!NOTE]
> 生成されたプレハブに変更を加える場合は、それを [階層] にドラッグし、変更を加え、[インスペクター] タブの [適用] をクリックしてプレハブを更新します。 

3. 準備ができたら、[Uploader] タブを下にスクロールし、アセット バンドルを使用して zip ファイルを生成する準備をします
4. イテレーションを高速化するには **、[Build Kit for Android? ]をオフにします**。 後でキットの反復または機能の共有/機能を行う場合は、Android 用のバージョンをビルドしてアップロードしてください。 
5. [Load **Kit Prefab Directories]/(キットプレハブ ディレクトリの読み込み)を**
6. Kit **フォルダー名に** 一致する名前の横にある [ビルド] を選択します。 同じ Unity プロジェクトから複数のキットを生成するのが一般的です。 キットのサイズによっては、これには時間がかかる場合があります。 完了すると、zip ファイルを含むフォルダーが自動的に開きます。 
7. Web サイトに移動し、前に作成したキットを編集して、生成した zip ファイルをアップロードします。 ファイルサイズによっては、このアップロードに時間がかかる場合があります。
    * 成功した場合は、左側の [アップロード] の下にファイル サイズと PC と Android の場合、および最後に更新された時間が表示されます
    * 失敗した場合は、スクリプトを持たなかったり、スクリプトがサポートされなかったり、セキュリティの確認を行って、もう一度やり直してください。

おめでとうございます。 独自の Kit を使用して Worlds を構築する準備ができました。

## <a name="troubleshooting"></a>トラブルシューティング 

**制限はありますか?**
ハード制限はまだありませんが、アーティファクトが 1 つしか使用されていない場合でも、ユーザーは Kit 全体のプラットフォーム用に AssetBundle をダウンロードする必要があります。 プラットフォームごとのダウンロードを 5 MB 以下に維持してください。 これを行う 1 つの方法は、小さなキットに分割する方法です。 たとえば、200 props を半分に分割する必要があります。 

**"分割された目" が表示されますか?**
最新のアップデーターを再アップロードして、適切なレンダリング設定を取得する

**更新/変更が反映されない場合**
    * [キット] ページで更新時刻を確認する
    * World の再入力は機能しません。クライアントを再起動します。 その場合でも、更新に数分かかる場合があります
    * フォルダー名またはプレハブ名にスペース (例: **'party_favors' と 'party favors' が含されていないことを確認します**

**スクリプトは持っているが、私は持ってはいないと言い続ける** AssetBundle Browser には、ファイルが自動的に含まれる場合があります。 取り込むモデルを分離してみてください。 たとえば、既に別のプレハブの一部である場合は、ドラッグしない

**パーティクル システムとアニメーションについて**
これらに対して、Mesh Rendering と Collision を無効にした状態で、原点に配置された 1x1x1 キューブの下に配置します。 パーティクル システムではループが有効になっている **必要があります。** また、Altspace で適切にスケーリングできるよう、スケーリングを **Hierarchy** に設定する必要があります。 すべてのアニメーションのプレハブを生成した後、それぞれの競合オブジェクトの競合 **を** 無効にします。

**色Artifacts濃い** モデルの素材シェーダーを **Mobile/Vertex の照明専用の方向ライトに設定しましたか**?

**成果物が正しい方向に向かっている** モデルと **コライダー** を **回転させ、** プレハブを更新します。 親を回転しても何も実行されません。これは無視されます。 [回転のオーバーライド] **フィールドを使用** すると、これを簡単に行うことができます。

**これらの関数Artifacts SDK の **CreateFromLibrary 関数で使用** できますか?**
はい