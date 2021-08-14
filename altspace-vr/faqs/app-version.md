---
title: AltspaceVR アプリのバージョンを検索しています
description: 現在実行している altのバージョンを確認するには、アプリ、設定、およびクライアントの各ログを使用する方法について説明します。
ms.date: 02/10/2021
ms.topic: article
keywords: アプリのバージョン
ms.openlocfilehash: fbf67a8302a67ddb916772420949cf0509a0d4a60c472711975c651862438b93
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "119128254"
---
# <a name="finding-the-altspacevr-app-version"></a>AltspaceVR アプリのバージョンを検索しています

問題のトラブルシューティングを行う過程で、現在実行している Altworkplace Evr アプリのバージョンを確認するメッセージが表示される場合があります。

## <a name="in-altspacevr"></a>Altworkplace Evr

Altspace Evr でアプリのバージョンを確認するには、[ **設定] メニュー** に移動し、左側のナビゲーションバーで [バージョン **情報** ] を選択します。 次のスクリーンショットに示すように、"アプリのバージョン" はここで報告されます。

![[バージョン情報] パネルを開いた状態で設定メニューを開く](images/app-version-img-01.png)

## <a name="in-windows-system-settings"></a>Windows システム設定

Microsoft Store を使用して altをインストールした場合は、[Windows システム設定] でアプリのバージョンを確認することもできます。  このシナリオは、クライアントに正常にログインできない場合にアプリのバージョンを報告するときに適しています。

Windows システム設定でアプリのバージョンを確認するには、[**スタート] メニュー** を開き、[**アプリ & 機能**] を入力して、結果を選択します。 アプリの一覧で [ **Altworkplace Evr** ] に移動します。 [Alt] を左クリックし、表示されるメニューから [ **詳細オプション** ] を選択します。

![[アプリと機能] メニューを開き、[詳細設定] オプションが強調表示されている](images/app-version-img-02.png)

[**詳細設定] オプション** の [**仕様**] ヘッダーで、[**バージョン**] ラベルの右側にアプリの **バージョン** が表示されます。

![アプリバージョンが強調表示されている状態で開く詳細設定オプション](images/app-version-img-03.png)

## <a name="in-client-logs"></a>クライアントログで

Altspace Evr は、アプリケーションの起動時にクライアントログファイルのアプリバージョンを "Altspace Version" として報告します。 これは、クライアントに正常にログインできないが、エラーが発生する前に開始しようとした場合に、アプリのバージョンを取得するのに適したオプションです。

## <a name="windows"></a>Windows

Windows では、クライアントログファイルは Windows エクスプローラーで次の場所にあります。

```
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player.log
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player-prev.log
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