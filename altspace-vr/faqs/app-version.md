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
# <a name="finding-the-altspacevr-app-version"></a><span data-ttu-id="b770f-104">AltspaceVR アプリのバージョンの検索</span><span class="sxs-lookup"><span data-stu-id="b770f-104">Finding the AltspaceVR app version</span></span>

<span data-ttu-id="b770f-105">問題のトラブルシューティングの過程で、現在実行している AltspaceVR アプリのバージョンを尋ねられる場合があります。</span><span class="sxs-lookup"><span data-stu-id="b770f-105">In the course of troubleshooting an issue, you may be asked what version of the AltspaceVR app you're currently running.</span></span>

## <a name="in-altspacevr"></a><span data-ttu-id="b770f-106">AltspaceVR で</span><span class="sxs-lookup"><span data-stu-id="b770f-106">In AltspaceVR</span></span>

<span data-ttu-id="b770f-107">AltspaceVR でアプリのバージョンを見つけるには、設定メニューに移動し **、左側の** ナビゲーション バーで **[バージョン情報** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b770f-107">To find the app version in AltspaceVR, navigate to the **settings menu** and select **About** in the left navigation bar.</span></span> <span data-ttu-id="b770f-108">次のスクリーンショットに示すように、"アプリのバージョン" がここに報告されます。</span><span class="sxs-lookup"><span data-stu-id="b770f-108">The 'App Version' is reported here, as shown in the screenshot below.</span></span>

![[設定] メニューが開き、約パネルが開きます](images/app-version-img-01.png)

## <a name="in-windows-system-settings"></a><span data-ttu-id="b770f-110">[Windows システム設定]</span><span class="sxs-lookup"><span data-stu-id="b770f-110">In Windows System Settings</span></span>

<span data-ttu-id="b770f-111">Windows システム設定を使用して AltspaceVR Microsoft Store場合は、さらに Windows システム設定でアプリのバージョンを確認できます。</span><span class="sxs-lookup"><span data-stu-id="b770f-111">If you installed AltspaceVR via the Microsoft Store, you can additionally find the app version in the Windows system settings.</span></span>  <span data-ttu-id="b770f-112">このシナリオは、クライアントに正常にログインできない場合にアプリのバージョンを報告する場合に適しています。</span><span class="sxs-lookup"><span data-stu-id="b770f-112">This scenario is a good fit when reporting the app version if you're unable to successfully log into the client.</span></span>

<span data-ttu-id="b770f-113">Windows システム設定でアプリのバージョンを見つけるには、 [スタート]メニューを開き、 [アプリと機能] に「&」と入力して、結果を選択します。</span><span class="sxs-lookup"><span data-stu-id="b770f-113">To find the app version in Windows system settings, open the **Start Menu**, type in **Apps & Features**, and select the result.</span></span> <span data-ttu-id="b770f-114">アプリの **一覧で AltspaceVR** に移動します。</span><span class="sxs-lookup"><span data-stu-id="b770f-114">Navigate to **AltspaceVR** in the list of apps.</span></span> <span data-ttu-id="b770f-115">AltspaceVR を左クリックし、表示 **されるメニューから** [詳細オプション] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b770f-115">Left-click AltspaceVR and select **Advanced Options** from the menu that appears.</span></span>

![[詳細設定] オプションが強調表示された [アプリと機能] メニューが開きます](images/app-version-img-02.png)

<span data-ttu-id="b770f-117">[詳細 **オプション] の**[**仕様**]ヘッダーの下に、[バージョン] ラベルの右側に [アプリのバージョン] が **表示** されます。</span><span class="sxs-lookup"><span data-stu-id="b770f-117">In the **Advanced Options**, under the **Specifications** header, the **App Version** should be listed to the right of the **Version** label.</span></span>

![アプリのバージョンが強調表示された詳細オプションが開きます](images/app-version-img-03.png)

## <a name="in-client-logs"></a><span data-ttu-id="b770f-119">クライアント ログ内</span><span class="sxs-lookup"><span data-stu-id="b770f-119">In Client Logs</span></span>

<span data-ttu-id="b770f-120">AltspaceVR は、アプリケーションの起動時に、クライアント ログ ファイル内のアプリのバージョンを "Altspace バージョン" として報告します。</span><span class="sxs-lookup"><span data-stu-id="b770f-120">AltspaceVR reports the app version in the client logs file as "Altspace Version" during application startup.</span></span> <span data-ttu-id="b770f-121">これは、クライアントに正常にログインできないが、失敗する前に開始しようとした場合に、アプリのバージョンを取得する場合に便利なオプションです。</span><span class="sxs-lookup"><span data-stu-id="b770f-121">This would be a good option to get the app version if you can't successfully log into the client, but it did attempt to start before failing.</span></span>

## <a name="windows"></a><span data-ttu-id="b770f-122">Windows</span><span class="sxs-lookup"><span data-stu-id="b770f-122">Windows</span></span>

<span data-ttu-id="b770f-123">Windows では、クライアント ログ ファイルは、Windows エクスプローラーから次の場所で確認できます。</span><span class="sxs-lookup"><span data-stu-id="b770f-123">On Windows, the client logs file can be found via Windows Explorer at:</span></span>

```
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player.log
%userprofile%\AppData\LocalLow\Microsoft\AltspaceVR\Player-prev.log
```

<span data-ttu-id="b770f-124">このファイルは、AltspaceVR を起動するごとに上書きされます。</span><span class="sxs-lookup"><span data-stu-id="b770f-124">This file is overwritten each time you launch AltspaceVR.</span></span> <span data-ttu-id="b770f-125">'Player.log' は最新のセッションを表し、'Player-prev.log' は前のセッションを表します。</span><span class="sxs-lookup"><span data-stu-id="b770f-125">'Player.log' represents your latest session, and 'Player-prev.log' represents the previous session.</span></span>

## <a name="via-powershell"></a><span data-ttu-id="b770f-126">PowerShell から</span><span class="sxs-lookup"><span data-stu-id="b770f-126">Via PowerShell</span></span>

<span data-ttu-id="b770f-127">上級ユーザーは、次のように PowerShell を使用してこの文字列のクライアント ログを検索できます。</span><span class="sxs-lookup"><span data-stu-id="b770f-127">Advanced users can search the client logs for this string via PowerShell as follows:</span></span>

<span data-ttu-id="b770f-128">次の内容を入力します。</span><span class="sxs-lookup"><span data-stu-id="b770f-128">Input:</span></span>

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

<span data-ttu-id="b770f-129">出力:</span><span class="sxs-lookup"><span data-stu-id="b770f-129">Output:</span></span>

<span data-ttu-id="b770f-130">[2.047] AltspaceVR バージョン: 3.2.23.e66c2</span><span class="sxs-lookup"><span data-stu-id="b770f-130">[2.047] AltspaceVR Version: 3.2.23.e66c2</span></span>