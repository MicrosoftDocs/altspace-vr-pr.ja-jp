---
title: Altworkplace Evr アプリに関してよく寄せられる質問
description: Altworkplace Evr アプリのトラブルシューティングとサポート。
ms.date: 8/16/2021
author: qianw211
ms.author: v-qianwen
ms.topic: article
keywords: vr、Alt、Evr、トラブルシューティング、サポート
ms.openlocfilehash: a0df1e100ef8511fe3c9129548529577964c2336
ms.sourcegitcommit: 5c452a9092297c0bfbc8efabebf395e7ee31853f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/30/2021
ms.locfileid: "129311897"
---
# <a name="frequently-asked-questions-about-the-altspacevr-app"></a>Altworkplace Evr アプリに関してよく寄せられる質問

## <a name="finding-the-altspacevr-app-version"></a>AltspaceVR アプリのバージョンを検索しています

問題のトラブルシューティングを行う過程で、現在実行している Altworkplace Evr アプリのバージョンを確認するメッセージが表示される場合があります。

### <a name="in-altspacevr"></a>Altworkplace Evr

Altspace Evr でアプリのバージョンを確認するには、[ **設定] メニュー** に移動し、左側のナビゲーションバーで [バージョン **情報** ] を選択します。 次のスクリーンショットに示すように、"アプリのバージョン" はここで報告されます。

![[バージョン情報] パネルが開いている状態で [設定] メニューを開く](images/app-version-img-01.png)

### <a name="in-windows-system-settings"></a>Windows のシステム設定

Microsoft Store を使用して Altをインストールした場合は、Windows の [システム設定] でさらにアプリのバージョンを見つけることができます。  このシナリオは、クライアントに正常にログインできない場合にアプリのバージョンを報告するときに適しています。

Windows システム設定でアプリのバージョンを確認するには、[ **スタート] メニュー** を開き、[ **アプリ & 機能**] に「」と入力して、結果を選択します。 アプリの一覧で [ **Altworkplace Evr** ] に移動します。 [Alt] を左クリックし、表示されるメニューから [ **詳細オプション** ] を選択します。

![[アプリと機能] メニューを開き、[詳細設定] オプションが強調表示されている](images/app-version-img-02.png)

[**詳細設定] オプション** の [**仕様**] ヘッダーで、[**バージョン**] ラベルの右側にアプリの **バージョン** が表示されます。

![アプリバージョンが強調表示されている状態で開く詳細設定オプション](images/app-version-img-03.png)

### <a name="app-version-in-client-logs"></a>クライアントログのアプリバージョン

Altspace Evr は、アプリケーションの起動時にクライアントログファイルのアプリバージョンを "Altspace Version" として報告します。 これは、クライアントに正常にログインできないが、エラーが発生する前に開始しようとした場合に、アプリのバージョンを取得するのに適したオプションです。

### <a name="windows"></a>Windows

Windows では、クライアントログファイルは Windows エクスプローラーで次の場所にあります。

```
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player.log
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player-prev.log
```

このファイルは、Altworkplace Evr を起動するたびに上書きされます。 ' Player .log ' は最新のセッションを表し、' Player-prev ' は前のセッションを表します。

### <a name="via-powershell"></a>PowerShell から

上級ユーザーは、次のように PowerShell を使用して、この文字列のクライアントログを検索できます。

次の内容を入力します。

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

出力:

[2.047] Alte66c2 Evr バージョン: 3.2.23。

## <a name="how-do-i-upload-my-client-logs"></a>クライアントログをアップロード操作方法には

Altworkplace Evr クライアントアプリケーションは、Altの使用中に発生する診断データとイベントのログを保持します。 問題のトラブルシューティングを行う過程で、「ログをアップロードする」というメッセージが表示される場合があります。 これは、問題のトラブルシューティングに役立つように、チームのローカルログコンテンツをチームに送信することができるようにするための、Altworkplace Evr の機能です。

### <a name="in-altspacevr"></a>Altworkplace Evr

Altspace Evr のクライアントログをアップロードするには、[ **設定] メニュー** に移動し、左側のナビゲーションバーで [ **サポート** ] を選択します。 次のスクリーンショットに示すように、ログをアップロードするためのオプションがいくつかあります。

![[サポート] パネルの [開く] および [ログ] フィールドが強調表示されている [設定] メニュー](images/help-altvr-uploadlogs.png)

### <a name="fields"></a>フィールド

**"問題が発生しました"**
何が起こったかについて説明します。たとえば、バグが見つかった場合は、実際に発生したことと比較して、予想されることを説明します。 この情報は、[アップロードするときにログと一緒に送信されます。

**"ログのアップロード"** このボタンをクリックすると、現在のセッションからログがアップロードされます。 このオプションは、同じセッションで問題が見つかった場合 (たとえば、Altのクライアントを閉じていない場合など)、レポートを作成する場合に使用します。

**"最後のログをアップロードする"** このボタンをクリックすると、前のセッションからログがアップロードされます。

**"最後のクラッシュログをアップロードする"** このボタンをクリックすると、経験した最新のクラッシュからさらに多くのログコンテンツがアップロードされます。

### <a name="in-client-logs"></a>クライアントログで

コンピューターからログファイルを取得することもできます。 これらのログを取得する方法については、 [こちら](#app-version-in-client-logs)を参照してください。


これらのファイルを見つけたら、 [サポートチケットを開き](https://help.altvr.com/hc/en-us/requests/new) 、[送信] をクリックする前にチケット要求でログをアップロードします。

## <a name="what-do-i-do-if-i-cant-launch-altspacevr"></a>Altworkplace Evr を起動できない場合はどうすればよいですか。

このような場合には、いくつかの理由により、Altare が起動しないことがあります。 アプリケーションが必要なサードパーティ製ソフトウェアと共に正しくインストールされるようにするには、次の手順を試してください。

### <a name="if-youre-trying-to-launch-altspacevr-for-the-first-time"></a>最初に Altを起動しようとしている場合は、次のようにします。

1. デバイスがサポートされており、 [指定された最小要件](../getting-started/system-requirements.md)を満たしていることを確認します。
2. 最新の [Oculus ソフトウェア](https://www.oculus.com/setup) がインストールされていることを確認し、その設定 > 全般 > 不明なデバイスがオンに設定されていることを確認します。 2D モードで起動する場合は、Oculus をインストールする必要はありません。
3. インターネット接続が動作していることを確認します。 ネットワークファイアウォール内から Altspace を起動しようとしている場合は、UDP ポート5055と5056、TCP ポート80および443を開きます。 企業または教育機関のファイアウォールのネットワーク内にいる場合は、ネットワーク管理者または IT 部門に問い合わせなければならないことがあります。
4. 関連項目:
    * [Oculus クエスト用の Alt Evr のインストール](../getting-started/oculus-installation.md)
    * [Windows Mixed Reality の Altのインストール](../getting-started/wmr-installation.md)

### <a name="if-altspacevr-reports-that-the-current-version-is-out-of-date"></a>現在のバージョンが最新ではないことを Altを報告する場合は、次のようになります。

* 使用しているアプリケーションのバージョンはサポートされなくなりました。 店頭からダウンロードした場合、ストアがクライアントを更新できるようになる前に、更新プログラムが最近起動した可能性があります。
* 更新を強制する場合は、さまざまなネットショップを通じて行うことができます。
    * **Microsoft Store:** [Microsoft Store サポート-Microsoft Store でアプリとゲームの更新プログラムを取得する](https://support.microsoft.com/account-billing/get-updates-for-apps-and-games-in-microsoft-store-a1fe19c0-532d-ec47-7035-d1c5a1dd464f)
    * **Oculus:** Oculus ライブラリを開き、左側のナビゲーションバーで [更新] に移動します。
    * **ストリーム:** [ストリームサポート-更新プログラム & のインストールに関する問題](https://support.steampowered.com/kb_article.php?ref=2274-IFLV-5334)

### <a name="if-the-program-was-working-but-ceased-to-launch-after-update"></a>プログラムが動作していたが、更新後に起動するなった:

* ソフトウェアのクリーン再インストールを実行します。 このためには、アプリケーションの既存のバージョンをアンインストールまたは削除する必要があります。 システムから完全に削除されたら、ストリーム、Oculus、または Microsoft Store を使用して、Altspace をインストールします。
* Altworkplace Evr の起動で問題が発生した場合は、 [サポートチケット](https://help.altvr.com/hc/requests/new)を通じてお知らせください。 セッションの [ログファイル](altspacevr-app-faq.md#how-do-i-upload-my-client-logs) を含めます。

### <a name="if-altspacevr-fails-to-launch-after-customizing-your-home-space"></a>ホームスペースをカスタマイズした後に Altspace Evr を起動できない場合は、次のようになります。

* [ホームスペースの web サイト](https://account.altvr.com/users/sign_in)に移動します。
* 世界のテンプレートがまだ存在していることを確認します。 テンプレートが共有されている場合は、所有者によって削除されている可能性があります。これにより、ホームスペースの読み込みに失敗します。
    * テンプレートが削除されている場合は、左側の [ワールドツール] パネルで世界を "編集" し、既存のテンプレートを別のテンプレートに置き換え、[更新] を使用して変更を保存します。
* 左側の [ワールドツール] パネルから [オブジェクト] を選択して、読み込みに失敗した可能性のあるすべてのオブジェクトを削除します。 問題のあるオブジェクトには次のようなものがあります。
    * 削除されたキットのオブジェクト、またはキットから削除されたオブジェクト (まだ世界中に存在するもの)。
    * 実験的な GLTFs。
* 上の項目をアドレス指定した後、Altを再入力してください。

ネットワーク管理者または IT 部門 (Azure の IP 範囲とサービスタグを含む) の高度なサポートについては、 [ダウンロードの詳細](https://www.microsoft.com/en-us/download/details.aspx?id=56519)を参照してください。

## <a name="support"></a>サポート

Altworkplace Evr チームに関する質問やフィードバックはありますか? 

> [!div class="nextstepaction"]
> [サポートリクエストを送信するには、ここをクリックしてください](https://help.altvr.com/hc/requests/new)