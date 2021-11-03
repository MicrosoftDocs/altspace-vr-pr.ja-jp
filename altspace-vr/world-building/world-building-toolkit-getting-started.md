---
title: Altspace Uploader の紹介
description: Altspace Uploader で Unity シーン テンプレートを使用して、AltspaceVR ワールドを設定してアップロードする方法について説明します。
ms.date: 10/29/2021
ms.author: v-vtieto
ms.topic: article
ms.openlocfilehash: 6d28b3efe75d589a0a09d4969add5d043a3116d0
ms.sourcegitcommit: 20605c50a93852f93a3464c5c339f6a7da67a047
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/03/2021
ms.locfileid: "131278964"
---
# <a name="introducing-the-altspace-uploader"></a>Altspace Uploader の紹介

> [!NOTE]
> - 興味がある場合は、公式 [の AltspaceVR Discord](https://discordapp.com/invite/altspacevr) に参加し、新しい#worldにアクセスしてください。  
> - 古い領域を取り込もうとしている場合は、アップグレード ガイド を [参照してください](upgrading-old-unity-projects.md)。 

Uploader を使用すると、Unity シーンをワールドのテンプレートとして使用できます。 お気に入りの作成用の家を、お気に入りの家に持ち込むには、Minecraft。 Unity にインポートできる場合は、この方法で Altspace に取り込む可能性があります。 Worlds の例 [を次に示します](https://account.altvr.com/worlds/1046572460192825569)。

![ワールドの例](images/unity-uploader-img-01.png)

## <a name="setup"></a>セットアップ

1. 公式の [AltspaceVR Discord に参加し](https://discordapp.com/invite/altspacevr) 、#worldチャネルにアクセスします。 友人は、友人がワールドを単独で構築できません。
2. 基本については [、World-Building はじめに ガイド](world-building-getting-started.md) を参照してください
3. [Unity Hub をインストール](https://blogs.unity3d.com/2018/01/24/streamline-your-workflow-introducing-unity-hub-beta) し [**、2020.3.18f1 をインストールします**](https://unity3d.com/unity/whats-new/2020.3.18)。 このバージョンと正確に一致しない限り、アップアップロード機能は機能しません。 無料の Unity アカウントを持ってない場合は、無料のUnity アカウントが必要です。これを楽しく行うので、[個人用] を選択します。 インストール中に、必ず **[Android** ビルド] オプションをオンにし、自動更新を無効にします。
    * Android ビルド **サポート モジュールを含** める。
    * このWindows、Mac ビルド サポート **(Mono) モジュールを含める必要** があります。
    * Mac では、Windows **ビルド サポート (Mono) モジュールを含** める。
4. [最新の Unity Uploader をダウンロードする](https://altvr.com/download-latest-unity-uploader)
5. [Web サイトでテンプレート](https://account.altvr.com/space_templates/new) を作成します。 テンプレート に名前 **Hello World付けします**。
6. [World を作成し](https://account.altvr.com/worlds/my)、 という名前を **付Hello World。** [テンプレート **Hello Worldテンプレート]** を選択します。

![作成されたワールド画面](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a>アップロードを作成する

> [!NOTE]
> 詳細なステップ バイ ステップ ガイドについては、こちらを参照 [してください](https://buildingthemetaverse.medium.com/how-to-make-your-own-altspace-templates-and-kits-unity-2020-3-9-uploader-2-x-5b40e92bb759)。

1. Unity Hub を開き、新しい Unity 2020.3.9 プロジェクトを作成します。 テンプレートの [ユニバーサル レンダリング パイプライン **] を選択します**。

    ![URP Unity テンプレートを選択する](images/001-unity-templates.png)

1. Altspace Uploader をダウンロードしたフォルダーに移動し、そのフォルダーから新しい Unity プロジェクトのルート フォルダーにコピーまたは移動します。
1. メニュー バーの Unity で、[ウィンドウ] ボタンを **選択**  >  **パッケージ マネージャー。**
1. メニュー バーパッケージ マネージャープラス記号ドロップダウン ("+") を選択し、[tarball からパッケージを追加する]**を選択します**。
1. Altspace Uploader が含まれているフォルダーに移動し、Uploader を選択して、[開く] を **クリックします**。  パッケージが読み込まれると **、AltspaceVR** がメニュー バーに表示されます。

    ![メニュー バーの AltspaceVR](images/002-altspacevr-on-menu-bar.png)

> [!NOTE]
> Altspace で使用する Unity プロジェクトごとに、Altspace Uploader パッケージをインポートする必要があります。
1. メニュー バーで **、AltspaceVR** の [テンプレート] >選択します。
1. **[Altspace VR テンプレート] ダイアログ** で、Altspace アカウントの資格情報でサインインします。 (MSA ログインは間もなく使用できる予定です。 Microsoft アカウント で Altspace にログインしただけの場合は、Web サイトの [パスワードを忘れた場合] オプションを使用してパスワードを作成する必要があります)。
1. [テンプレート **の選択] ドロップダウンを** クリックし、[テンプレートの選択 **Hello World選択します**。
1. シーンを選択する: **[.unity ファイル** の選択] 省略記号ボタン (3 つのドット) をクリックし、プロジェクトの **Assets** Scenes フォルダーに移動し  >  **、[SampleScene.unity]** を選択して開きます。
1. [**プラットフォームのビルド: ]** で、[ビルド]**がWindows** 確認します。 現在のところ、Android と **Mac** の他の 2 つの **オプションは** 選択されません。  ユーザーにアクセスを望んだら、すべてのプラットフォーム用にビルドしてアップロードする必要があります。"
1. [ビルド]**ボタン& アップロード** 選択します。 このプロセスには 1、2 分かかる場合があります。
1. Altspace を起動し、[メイン メニュー **] を** 選択し、メニュー バーで [マイ ワールド] **を選択します**。
1. [ファイル] **Hello World** し、開きます。

    シーンは、Unity エディターで見たものに似ている必要があります。

## <a name="whats-supported"></a>サポートされる操作

* はい: モデル、衝突、アニメーション、パーティクル効果、オーディオ、Skybox などです。
* いいえ: スクリプト。 セキュリティ上の理由から、スクリプトを含むアップロードは拒否されます。
* おそらく、動的なグローバル 照明のような空想的なもの。
* アップロード異なるプラットフォームのシーンを個別に、または一緒に作成します。
* 「 [おすすめワールド」を参照してください](https://account.altvr.com/worlds/featured)。 多くはアップアップロードツールを使用して構築されました。

## <a name="tips"></a>ヒント

* 公式の [AltspaceVR Discord に参加します](https://discordapp.com/invite/altspacevr)。
* 左側の [テンプレート] ページに、プラットフォーム別の最新のアップロードが表示されます。 成功した場合は **、1 ~ 2 分前に が表示されます**。 

![アップロードが強調表示された [テンプレート] パネルが開きます](images/template-upload-list.png)

* 更新時にワールド内に表示できます。 Uploader が [完了]**アップロードした瞬間に**、ワールドをリセットして変更を確認できます。
* 単純なシーンで PC 専用に構築する場合、Altspace の変更を表示するには 1 分未満かかる必要があります。
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
    * 最も一般的なアップロード エラーは、間違った Unity バージョンが発生した結果です。 必要なバージョンと正確に一致する必要があります。
    * アップロードが大きすぎる可能性があります。 PC シーンを 100 MB <してください。 小規模から始め、ビルドアップします。 最適化、最適化、最適化。
    * 単純なキューブを含む新しいプロジェクトを試してみてください。
    * ビルド中に強制的に終了しない -- シーンが破損する可能性があります。 再アップロードしてみてください。

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
