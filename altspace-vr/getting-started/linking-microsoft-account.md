---
title: Microsoft アカウントのリンク
description: トラブルシューティングのヒントと共に、PC 上の2D モードの Microsoft アカウントと、イマーシブヘッドセットの VR モードをリンクする方法について説明します。
ms.date: 03/11/2021
ms.topic: article
keywords: microsoft、2D モード、VR モード
ms.openlocfilehash: 87185a167acc58f0254d1fccbb36b0707abc06c1
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212988"
---
# <a name="linking-your-microsoft-account"></a>Microsoft アカウントのリンク

Altをサポートするように [なりまし](https://account.microsoft.com/account)た。 Microsoft アカウントを使用すると、1回のログインでお気に入りの Microsoft 製品やサービスにアクセスできます。 Microsoft アカウントを使用すると、Office や Windows から Xbox や Minecraft まで、最も関心のあるファイル、写真、人、コンテンツに接続できます。 

Altworkplace Evr での Microsoft アカウントの統合はフェーズでロールアウトされ、現在、すべての altて Evr アカウント所有者に対して使用できます。 ロードマップと Microsoft アカウントの統合の詳細については、こちらの [ブログ](https://altvr.com/microsoft-account-integration)を参照してください。 

このアカウントと Microsoft アカウントをリンクするためのステップバイステップガイドをコンパイルしました。 アカウントリンクプロセスを完了する必要があるのは1回だけです。 その後、システムによって記憶されます。

## <a name="how-to-link-accounts"></a>アカウントをリンクする方法

開始するには、Microsoft アカウントが必要です。 [新しい Microsoft アカウントを作成](https://signup.live.com/?lic=1)するか、既にある既存のアカウントを使用することができます。 

## <a name="in-2d-mode-on-pc"></a>PC の2D モード

1. Altworkplace Evr を起動する
2. **メインメニュー > 自分の > アカウント** で開く
3. Microsoft アカウントのリンクを求めるメッセージが表示されたら、[ **リンク** ] を選択します。

![[アカウント] パネルが強調表示された状態で、AltspaceVR アプリを開く](images/linking-accounts-img-02.png)

4. 別のウィンドウが開き、リンクする Microsoft アカウントを選択するよう求めるメッセージが表示されます。 
    * 接続するものを選択し、[**続行**] を選択します。

![Microsoft アカウントサインインウィンドウを開く](images/linking-accounts-img-03.jpg)

アカウントリンクプロセスが完了すると、アカウントの資格情報が更新されていることがわかります。

![アカウントパネルと資格情報が強調表示されている Alt、アプリを開く](images/linking-accounts-img-04.png)
 
## <a name="in-vr-mode-on-your-headset"></a>ヘッドセットの VR モード

1. Altworkplace Evr を起動する
2. **メインメニュー > 自分の > アカウント** で開く
3. Microsoft アカウントのリンクを求めるメッセージが表示されたら、[ **リンク** ] を選択します。

![[アカウント] パネルが強調表示されている状態で、[Alt] を開く](images/linking-accounts-img-02.png)

4. 別の画面が表示され、一意のコードを使用してデバイスをアクティブ化するように求められます。この場合、次の内容をコピーする必要があります。

![アクティブ化 pin が表示されているアカウントパネルを使用して、AltspaceVR アプリを開く](images/linking-accounts-img-05.png)

5. コンピューターのブラウザー画面に切り替えて、 [microsoft.com/devicelogin](https://login.microsoftonline.com/common/oauth2/deviceauth)に移動します。
    * 一意のコードを入力し、[ **次へ** ] を選択します。コードの大文字と小文字は区別されません
    * 表示されたログインの指示に従います。

![アクティベーションコードのテキストテキストを含む Web ブラウザー](images/linking-accounts-img-06.png)

これで、[Alt] に戻り、更新されたアカウントの資格情報を確認できるようになりました。

![アカウントパネルを使用して開くと、資格情報が強調表示された [Alt]](images/linking-accounts-img-04.png)

## <a name="troubleshooting-tips"></a>トラブルシューティングのヒント

* アカウントリンクプロセス中に問題が発生した場合は、アカウントへの接続を再試行する前に、作業を終了して終了してください。
* VR モードで問題が発生している場合は、ヘッドセットを取り外し、2D PC モード (またはその逆) に切り替えてみてください。
* Microsoft アカウントに再接続できないことがわかった場合でも、ユーザー名とパスワードを使用して Altlt Evr に戻ることができます。 [ALTを使用してサインイン] ボタンを選択するだけです。
* 問題が発生した場合にログを送信するには、 **メインメニュー > 設定 > サポート > ログのアップロード]** の順に移動します。

![[サポート] パネルが強調表示された状態で開いている [Alt] Evr アプリの設定](images/linking-accounts-img-07.png)

## <a name="microsoft-account-integration-faq"></a>Microsoft アカウント統合に関する FAQ

**これにより、ユーザー名が変更されるか、または my name タグに詳細が表示されますか。**

Altlt Evr アカウントを Microsoft アカウントにリンクしても、パブリックに表示されるユーザー名または名は変更されません。 アカウントのログイン資格情報 (プライベート) のみが変更されます。自分の名前、ユーザー名、およびプロファイルの画像が、Altlt Evr の他のユーザーにどのように表示されるかを完全に制御できます。

**アカウントを引き続き切り替えることはできますか?このオプションは、[設定] の下ではなくなりました。**

はい、もう少し修飾しました。 アカウントを管理できるようになりました。 [**メイン] メニュー** の [アカウント] を &、[自分の > アカウント] >

**Microsoft アカウントを既にお持ちですか?**

Microsoft アカウントを既にお持ちの可能性があります。 Minecraft や Xbox でゲームをプレイしたり、Office 365 をサブスクライブしたり、他のマイクロソフト製品やサービスを定期的に使用したりしていますか。 その場合は、既に Microsoft ログインがあることがあります。 [ここで](https://login.live.com/login.srf?wa=wsignin1.0&rpsnv=13&ct=1610764342&rver=7.0.6738.0&wp=MBI_SSL&wreply=https:%2F%2Faccount.microsoft.com%2Fauth%2Fcomplete-signin%3Fru%3Dhttps%253A%252F%252Faccount.microsoft.com%252F%253Frefp%253Dsignedout-index&lc=1033&id=292666&lw=1&fl=easi2)は、電子メールが既存の MSA に既に関連付けられているかどうかを確認できます。

**これは Outlook で新しい電子メールアドレスを作成する必要があることを意味しますか。**

いいえ。 Microsoft でホストされていない場合でも、現在の電子メールアドレスを使用して Microsoft アカウントをセットアップできます。 (例: G-Mail、Yahoo など)

**コストはかかりますか。**

いいえ! Microsoft アカウントの作成は無料です。 Alt領域 Evr の使用も無料です。 Microsoft アカウントは他の製品やサービスにリンクされているので、サブスクリプション (例: Office 365) や専門商品 (例: Minecraft Marketplace) など、AltspaceVR 以外のものを購入するために使用できます。

**アカウントのリンクに問題がある場合はどうすればよいですか。**

行き詰まっている場合は、いつでも [ヘルプデスク](https://help.altvr.com/hc/requests/new)に連絡することができます。

**複数の Altて Evr アカウントを持っている場合はどうすればよいですか。**

1つの Microsoft アカウントにリンクできるのは、AltspsaceVR アカウントだけです。 接続する各 Altworkplace Evr アカウントには、別の Microsoft アカウントが必要です。

**ログインの詳細を忘れた場合はどうすればよいですか。**

Microsoft アカウントに接続した後に、Altworkplace Evr へのログインで問題が発生した場合は、 [ヘルプデスク](https://help.altvr.com/hc/requests/new)にお問い合わせください。 Microsoft アカウントへのログインに関するトラブルシューティングのヒントとリソースの一覧については、こちらまたは[こちら](https://support.microsoft.com/account-billing/how-to-help-keep-your-microsoft-account-safe-and-secure-628538c2-7006-33bb-5ef4-c917657362b9)を[参照して](https://support.microsoft.com/account-billing/when-you-can-t-sign-in-to-your-microsoft-account-475c9b5c-8c25-49f1-9c2d-c64b7072e735)ください。

**Microsoft アカウントに接続する必要がありますか。**

心配しないでください。更新を行うまでしばらく時間がかかることがあります。 Microsoft アカウントの統合を段階的にロールします。 ただし、時間の経過と共に、現在取り組んでいる主要な新機能の一部は、そのアカウントを Microsoft アカウントにリンクしたユーザーのみが利用できます。 その理由は、これらの機能 (たとえば、チケットイベントなど) に強力で堅牢なセキュリティ対策が必要であるためです。 詳細については、こちらの [ブログ](https://altvr.com/microsoft-account-integration)を参照してください。

**プライバシーとデータについて**

[サービス利用規約](../community/terms-of-service.md)や[プライバシーポリシー](https://privacy.microsoft.com/privacystatement)に変更はありません。 お客様のプライバシーを保護し、お客様のデータや情報に関して完全に制御できることを保証するために、Microsoft と Altを提供しています。 プライバシーに関する Microsoft の主要な原則の詳細については、 [こちら](https://privacy.microsoft.com)を参照してください。 Microsoft アカウントに関する Microsoft の個人データに関する詳細情報を [ここで](https://www.microsoft.com/concern/privacyrequest-msa)要求することもできます。 最後に、アクティブな Altworkplace Evr アカウントがある場合は、データのコピーを要求し、いつでもデータを削除するように要求できます。

## <a name="see-also"></a>こちらもご覧ください

* [MSA とは](https://account.microsoft.com/account?lang=)
* [MSA のサービス条件](https://www.microsoft.com/servicesagreement/)
* [すべてのデバイスに Microsoft アカウントを設定する](https://account.microsoft.com/account/connect-devices)
* [サインインできない場合のヘルプ](https://support.microsoft.com//account-billing/when-you-can-t-sign-in-to-your-microsoft-account-475c9b5c-8c25-49f1-9c2d-c64b7072e735)
* [MSA パスワードをリセットする方法](https://support.microsoft.com//account-billing/how-to-reset-your-microsoft-account-password-eff4f067-5042-c1a3-fe72-b04d60556c37)
* [Microsoft アカウントを安全で安全な状態に保つ](https://support.microsoft.com//account-billing/how-to-help-keep-your-microsoft-account-safe-and-secure-628538c2-7006-33bb-5ef4-c917657362b9)
* [子供と家族のアカウントとコントロール](https://account.microsoft.com/family/about?refd=www.microsoft.com&ru=https:%2F%2Faccount.microsoft.com%2Ffamily%3Frefd%3Dwww.microsoft.com)
