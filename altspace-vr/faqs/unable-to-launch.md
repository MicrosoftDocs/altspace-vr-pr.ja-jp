---
title: Altworkplace Evr を起動できません
description: Altworkplace Evr 環境の起動に関連する問題を特定、報告、および修正する方法について説明します。
ms.date: 02/10/2021
ms.topic: article
keywords: faq
ms.openlocfilehash: fc49b5b7ed708e43a12616d782a397a364b2264e
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213133"
---
# <a name="i-cant-launch-altspacevr"></a>Altworkplace Evr を起動できません

このような場合には、いくつかの理由により、Altare が起動しないことがあります。 アプリケーションが必要なサードパーティ製ソフトウェアと共に正しくインストールされるようにするには、次の手順を試してください。

## <a name="if-youre-trying-to-launch-altspacevr-for-the-first-time"></a>最初に Altを起動しようとしている場合は、次のようにします。

1. デバイスがサポートされており、 [指定された最小要件](../getting-started/system-requirements.md)を満たしていることを確認します。
2. 最新の [Oculus ソフトウェア](https://www.oculus.com/setup) がインストールされていることを確認し、その設定 > 全般 > 不明なデバイスがオンに設定されていることを確認します。 2D モードで起動する場合は、Oculus をインストールする必要はありません。
3. インターネット接続が動作していることを確認します。 ネットワークファイアウォール内から Altspace を起動しようとしている場合は、UDP ポート5055と5056、TCP ポート80および443を開きます。 企業または教育機関のファイアウォールのネットワーク内にいる場合は、ネットワーク管理者または IT 部門に問い合わせなければならないことがあります。
4. 関連項目:
    * [Oculus クエスト用の Alt Evr のインストール](../getting-started/oculus-installation.md)
    * [Windows Mixed Reality の Altのインストール](../getting-started/wmr-installation.md)

## <a name="if-altspacevr-reports-that-the-current-version-is-out-of-date"></a>現在のバージョンが最新ではないことを Altを報告する場合は、次のようになります。

* 使用しているアプリケーションのバージョンはサポートされなくなりました。 店頭からダウンロードした場合、ストアがクライアントを更新できるようになる前に、更新プログラムが最近起動した可能性があります。
* 更新を強制する場合は、さまざまなネットショップを通じて行うことができます。
    * **Microsoft Store:** [Microsoft Store サポート-Microsoft Store でアプリとゲームの更新プログラムを取得する](https://support.microsoft.com/account-billing/get-updates-for-apps-and-games-in-microsoft-store-a1fe19c0-532d-ec47-7035-d1c5a1dd464f)
    * **Oculus:** Oculus ライブラリを開き、左側のナビゲーションバーで [更新] に移動します。
    * **ストリーム:** [ストリームサポート-更新プログラム & のインストールに関する問題](https://support.steampowered.com/kb_article.php?ref=2274-IFLV-5334)

## <a name="if-the-program-was-working-but-ceased-to-launch-after-update"></a>プログラムが動作していたが、更新後に起動するなった:

* ソフトウェアのクリーン再インストールを実行します。 このためには、アプリケーションの既存のバージョンをアンインストールまたは削除する必要があります。 システムから完全に削除されたら、ストリーム、Oculus、または Microsoft Store を使用して、Altspace をインストールします。
* Altworkplace Evr の起動で問題が発生した場合は、 [サポートチケット](https://help.altvr.com/hc/requests/new)を通じてお知らせください。 セッションの [ログファイル](uploading-client-logs.md) を含めます。

## <a name="if-altspacevr-fails-to-launch-after-customizing-your-home-space"></a>ホームスペースをカスタマイズした後に Altspace Evr を起動できない場合は、次のようになります。

* [ホームスペースの web サイト](https://account.altvr.com/users/sign_in)に移動します。
* 世界のテンプレートがまだ存在していることを確認します。 テンプレートが共有されている場合は、所有者によって削除されている可能性があります。これにより、ホームスペースの読み込みに失敗します。
    * テンプレートが削除されている場合は、左側の [ワールドツール] パネルで世界を "編集" し、既存のテンプレートを別のテンプレートに置き換え、[更新] を使用して変更を保存します。
* 左側の [ワールドツール] パネルから [オブジェクト] を選択して、読み込みに失敗した可能性のあるすべてのオブジェクトを削除します。 問題のあるオブジェクトには次のようなものがあります。
    * 削除されたキットのオブジェクト、またはキットから削除されたオブジェクト (まだ世界中に存在するもの)。
    * 実験的な GLTFs。
* 上の項目をアドレス指定した後、Altを再入力してください。

ネットワーク管理者または IT 部門 (Azure の IP 範囲とサービスタグを含む) の高度なサポートについては、 [ダウンロードの詳細](https://www.microsoft.com/en-us/download/details.aspx?id=56519)を参照してください。