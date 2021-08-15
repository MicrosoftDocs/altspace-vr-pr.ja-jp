---
title: World Building Toolkit のToolkit
description: World Building Toolkit で Unity シーン テンプレートを使用して AltspaceVR ワールドをセットアップしてアップロードする方法について説明します。
ms.date: 03/11/2021
ms.topic: article
keywords: ツールキット
ms.openlocfilehash: 8b66e35509060e00b2e52d3770380d009d7060339003f534d23fdd47372a57f0
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "119125408"
---
# <a name="introducing-the-world-building-toolkit"></a>World Building Toolkit のToolkit

> [!NOTE]
> World Building Toolkitは、すばらしい友人である[Anthony Madden](https://twitter.com/chigamesstudio)が運営するコミュニティ プロジェクトで、私たちのサポートを受け取っています。 興味がある場合は、公式 [の AltspaceVR Discord](https://discordapp.com/invite/altspacevr) に参加し、新しい#worldにアクセスしてください。 現在、Mac 試用版ベータ版があります [。詳細](https://altvr.com/altspacevr-mac)

Uploader を使用すると、Unity シーンをワールドのテンプレートとして使用できます。 お気に入りの作成は、Minecraft から、お気に入りの家を持ち込むか、Minecraft。 Unity にインポートできる場合は、この方法で Altspace に取り込む可能性があります。 Worlds の例 [を次に示します](https://account.altvr.com/worlds/1046572460192825569)。

![ワールドの例](images/unity-uploader-img-01.png)

## <a name="setup"></a>セットアップ

1. 公式の [AltspaceVR Discord](https://discordapp.com/invite/altspacevr) に参加し、#world作成チャネルにアクセスします。友人はワールドを単独で構築できません。
2. 基本については [、World-Building はじめに ガイド](world-building-getting-started.md) を参照してください
3. [Unity Hub をインストール](https://blogs.unity3d.com/2018/01/24/streamline-your-workflow-introducing-unity-hub-beta) し **、Unity 2020.3.9 をインストールします**。 このバージョンと正確に一致しない限り、アップアップロード機能は機能しません。 無料の Unity アカウントを持ってない場合は、無料のUnity アカウントが必要です。これを楽しく行うので、[個人用] を選択します。 インストール中に、必ず [Android ビルド] **オプションをオンに** し、自動更新を無効にします。
4. [最新の Unity Uploader をダウンロードする](upgrading-content-to-the-latest-unity.md#altspacevr-uploader-v090-upgrade-guide)
5. [Web サイトでテンプレート](https://account.altvr.com/space_templates/new) を作成します。 テンプレート にHello World **します**。
6. [World を作成し](https://account.altvr.com/worlds/my)、 という名前を付 **Hello World。** [ **テンプレートHello Worldテンプレート]** を選択します。

![作成されたワールド画面](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a>アップロードを作成する

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-a-Template/player]

1. Unity Hub を開き、新しい Unity 2020.3.9 プロジェクトを作成します。
2. プロジェクトを開いた後、ダウンロードしたファイルをダブルクリックして Uploader をインポートします (これは Unity パッケージです)。 これで **、AltspaceVR** という名前の新しいタブが表示されます。 Altspace で使用する Unity プロジェクトごとにパッケージをインポートする必要があります
3. **AltspaceVR >メニューを開>ビルド設定**
4. Altspace アカウントの資格情報を使用してサインインする
5. [テンプレート **の読み込み** ] を選択し、[テンプレート **Hello World選択します**
6. キューブをシーンに追加して保存します。
7. [Build **for Windows?] をオンにし、[Build** **for Android?] をオフにします。**
8. **[アップロード]** を選択します。 約 1 分で、**完了したアップロード** されます。
9. Altspace **Hello World** を起動し、Menu > Worlds > **My Worlds から入力して参加します**
10. [メニューからワールドをリセット **する] > 設定 >中程度の>領域**
11. キューブが表示されます。 上記のビデオのように高速に実行すると、10 秒以内に変更を確認できます。

## <a name="whats-supported"></a>サポートされる操作

* はい: モデル、衝突、アニメーション、パーティクル効果、オーディオ、Skybox など
* いいえ: スクリプト。 セキュリティ上の理由から、スクリプトを含むアップロードは拒否されます
* おそらく:動的なグローバル 照明のような空想的なもの
* アップロード異なるプラットフォームのシーンを個別または一緒に作成する
* 「 [おすすめの世界」を参照してください](https://account.altvr.com/worlds/featured)。多くはアップアップロードツールを使用して構築されました

## <a name="tips"></a>ヒント

* 公式の [AltspaceVR Discord に参加します](https://discordapp.com/invite/altspacevr)。
* 左側の [テンプレート] ページに、プラットフォーム別の最新のアップロードが表示されます。 成功した場合は **、1 ~ 2 分前に が表示されます**。Screen_Shot_2019-01-11 _at_1.21.04_AM.png

![アップロードが強調表示された [テンプレート] パネルが開きます](images/unity-uploader-img-03.png)

* 更新時にワールド内に表示できます。 Uploader が [完了]**アップロードした瞬間に**、ワールドをリセットして変更を確認できます。
* 単純なシーンを使用した PC 専用の構築では、Altspace の変更を表示するには 1 分未満かかる必要があります
* 気を散らさないように、ワールドをプライベートおよび一覧に含めないように設定します。
* ユーザーが既定で生成される場所を確認できるよう、キューブを原点に配置します。 アップロード時にキューブを非表示にする。

## <a name="troubleshooting"></a>トラブルシューティング

**私が落ちているか、何にもテレポートできない** オブジェクトに競合を追加して、そのオブジェクトにテレポートする必要があります。

**何も変更されません**
    * Unity でシーンを保存しましたか?
    * テストするプラットフォームを選択しましたか?
    * あなたは正しい世界にいますか? Uploader AND in the World フォームで適切なテンプレートを選択しましたか?
    * テンプレート ページの統計を確認しましたか?

**アップロード失敗またはアウト**
    * 最も一般的なアップロード エラーは、間違った Unity バージョンを持つことです。 必要なバージョンと正確に一致する必要があります。
    * アップロードが大きすぎる可能性があります。 PC シーンを 100 MB <してください。 小規模から始め、ビルドアップします。 最適化、最適化、最適化。
    * 単純なキューブで新しいプロジェクトを試してみてください。
    * ビルド中に強制的に終了しない -- シーンが破損する可能性があります。 再アップロードを試してください。

**プロセスが遅い**
    * 反復中にのみ PC 用を構築し、後で Android 用に構築することをお勧めします。
    * 使用されていないファイルを削除してみてください。 何らかの理由で、Unity が過剰な場合があります。

**Altspace 資格情報でサインインできない**
    * 電子メールでは大文字と小文字が区別されます。
    * 新しいプロジェクトを試してください。
    * Altspace アカウントが良好な位置にある必要があります。

## <a name="see-also"></a>関連項目

* [Unity Learn](https://unity3d.com/learn)
* [Unity フォーラム](https://forum.unity.com)
