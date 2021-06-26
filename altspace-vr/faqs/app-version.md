---
title: AltspaceVR アプリのバージョンの検索
description: AltspaceVR アプリ、設定、およびクライアント ログを使用して、現在実行している AltspaceVR のバージョンを見つける方法について学習します。
ms.date: 02/10/2021
ms.topic: article
keywords: アプリのバージョン
ms.openlocfilehash: 6b710e1724b890fa7ba0eecfcd774ef63128d5b7
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923179"
---
# <a name="finding-the-altspacevr-app-version"></a>AltspaceVR アプリのバージョンの検索

問題のトラブルシューティングの過程で、現在実行している AltspaceVR アプリのバージョンを尋ねられる場合があります。

## <a name="in-altspacevr"></a>AltspaceVR で

AltspaceVR でアプリのバージョンを見つけるには、設定メニューに移動し **、左側の** ナビゲーション バーで **[バージョン情報** ] を選択します。 次のスクリーンショットに示すように、"アプリのバージョン" がここに報告されます。

![[設定] メニューが開き、約パネルが開きます](images/app-version-img-01.png)

## <a name="in-windows-system-settings"></a>[Windows システム設定]

Windows システム設定を使用して AltspaceVR Microsoft Store場合は、さらに Windows システム設定でアプリのバージョンを確認できます。  このシナリオは、クライアントに正常にログインできない場合にアプリのバージョンを報告する場合に適しています。

Windows システム設定でアプリのバージョンを見つけるには、 [スタート]メニューを開き、 [アプリと機能] に「&」と入力して、結果を選択します。 アプリの **一覧で AltspaceVR** に移動します。 AltspaceVR を左クリックし、表示 **されるメニューから** [詳細オプション] を選択します。

![[詳細設定] オプションが強調表示された [アプリと機能] メニューが開きます](images/app-version-img-02.png)

[詳細 **オプション] の**[**仕様**]ヘッダーの下に、[バージョン] ラベルの右側に [アプリのバージョン] が **表示** されます。

![アプリのバージョンが強調表示された詳細オプションが開きます](images/app-version-img-03.png)

## <a name="in-client-logs"></a>クライアント ログ内

AltspaceVR は、アプリケーションの起動時に、クライアント ログ ファイル内のアプリのバージョンを "Altspace バージョン" として報告します。 これは、クライアントに正常にログインできないが、失敗する前に開始しようとした場合に、アプリのバージョンを取得する場合に便利なオプションです。

## <a name="windows"></a>Windows

Windows では、クライアント ログ ファイルは、Windows エクスプローラーから次の場所で確認できます。

```
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player.log
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player-prev.log
```

このファイルは、AltspaceVR を起動するごとに上書きされます。 'Player.log' は最新のセッションを表し、'Player-prev.log' は前のセッションを表します。

## <a name="via-powershell"></a>PowerShell から

上級ユーザーは、次のように PowerShell を使用してこの文字列のクライアント ログを検索できます。

次の内容を入力します。

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

出力:

[2.047] AltspaceVR バージョン: 3.2.23.e66c2