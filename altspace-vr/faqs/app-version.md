---
title: AltspaceVR アプリのバージョンを検索しています
description: 現在実行している altのバージョンを確認するには、アプリ、設定、およびクライアントの各ログを使用する方法について説明します。
ms.date: 02/10/2021
ms.topic: article
keywords: アプリのバージョン
ms.openlocfilehash: 5d503d3b89cd213696dd53616c5c7e3013aeef01
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213183"
---
# <a name="finding-the-altspacevr-app-version"></a>AltspaceVR アプリのバージョンを検索しています

問題のトラブルシューティングを行う過程で、現在実行している Altworkplace Evr アプリのバージョンを確認するメッセージが表示される場合があります。

## <a name="in-altspacevr"></a>Altworkplace Evr

Altspace Evr でアプリのバージョンを確認するには、[ **設定] メニュー** に移動し、左側のナビゲーションバーで [バージョン **情報** ] を選択します。 次のスクリーンショットに示すように、"アプリのバージョン" はここで報告されます。

![[バージョン情報] パネルが開いている状態で [設定] メニューを開く](images/app-version-img-01.png)

## <a name="in-windows-system-settings"></a>Windows のシステム設定

Microsoft Store を使用して Altをインストールした場合は、Windows の [システム設定] でさらにアプリのバージョンを見つけることができます。  このシナリオは、クライアントに正常にログインできない場合にアプリのバージョンを報告するときに適しています。

Windows システム設定でアプリのバージョンを確認するには、[ **スタート] メニュー** を開き、[ **アプリ & 機能**] に「」と入力して、結果を選択します。 アプリの一覧で [ **Altworkplace Evr** ] に移動します。 [Alt] を左クリックし、表示されるメニューから [ **詳細オプション** ] を選択します。

![[アプリと機能] メニューを開き、[詳細設定] オプションが強調表示されている](images/app-version-img-02.png)

[**詳細設定] オプション** の [**仕様**] ヘッダーで、[**バージョン**] ラベルの右側にアプリの **バージョン** が表示されます。

![アプリバージョンが強調表示されている状態で開く詳細設定オプション](images/app-version-img-03.png)

## <a name="in-client-logs"></a>クライアントログで

Altspace Evr は、アプリケーションの起動時にクライアントログファイルのアプリバージョンを "Altspace Version" として報告します。 これは、クライアントに正常にログインできないが、エラーが発生する前に開始しようとした場合に、アプリのバージョンを取得するのに適したオプションです。

## <a name="windows"></a>Windows

Windows では、クライアントログファイルは Windows エクスプローラーで次の場所にあります。

```
%userprofile%\appdata\locallow\altspacevr\altspacevr\Player.log
%userprofile%\appdata\locallow\altspacevr\altspacevr\Player-prev.log
```

このファイルは、Altworkplace Evr を起動するたびに上書きされます。 ' Player .log ' は最新のセッションを表し、' Player-prev ' は前のセッションを表します。

## <a name="via-powershell"></a>PowerShell から

上級ユーザーは、次のように PowerShell を使用して、この文字列のクライアントログを検索できます。

次の内容を入力します。

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

出力:

[2.047] Alte66c2 Evr バージョン: 3.2.23。