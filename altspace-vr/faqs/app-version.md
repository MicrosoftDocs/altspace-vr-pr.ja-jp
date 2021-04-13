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
# <a name="finding-the-altspacevr-app-version"></a><span data-ttu-id="99fab-104">AltspaceVR アプリのバージョンを検索しています</span><span class="sxs-lookup"><span data-stu-id="99fab-104">Finding the AltspaceVR app version</span></span>

<span data-ttu-id="99fab-105">問題のトラブルシューティングを行う過程で、現在実行している Altworkplace Evr アプリのバージョンを確認するメッセージが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="99fab-105">In the course of troubleshooting an issue, you may be asked what version of the AltspaceVR app you're currently running.</span></span>

## <a name="in-altspacevr"></a><span data-ttu-id="99fab-106">Altworkplace Evr</span><span class="sxs-lookup"><span data-stu-id="99fab-106">In AltspaceVR</span></span>

<span data-ttu-id="99fab-107">Altspace Evr でアプリのバージョンを確認するには、[ **設定] メニュー** に移動し、左側のナビゲーションバーで [バージョン **情報** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="99fab-107">To find the app version in AltspaceVR, navigate to the **settings menu** and select **About** in the left navigation bar.</span></span> <span data-ttu-id="99fab-108">次のスクリーンショットに示すように、"アプリのバージョン" はここで報告されます。</span><span class="sxs-lookup"><span data-stu-id="99fab-108">The 'App Version' is reported here, as shown in the screenshot below.</span></span>

![[バージョン情報] パネルが開いている状態で [設定] メニューを開く](images/app-version-img-01.png)

## <a name="in-windows-system-settings"></a><span data-ttu-id="99fab-110">Windows のシステム設定</span><span class="sxs-lookup"><span data-stu-id="99fab-110">In Windows System Settings</span></span>

<span data-ttu-id="99fab-111">Microsoft Store を使用して Altをインストールした場合は、Windows の [システム設定] でさらにアプリのバージョンを見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="99fab-111">If you installed AltspaceVR via the Microsoft Store, you can additionally find the app version in the Windows system settings.</span></span>  <span data-ttu-id="99fab-112">このシナリオは、クライアントに正常にログインできない場合にアプリのバージョンを報告するときに適しています。</span><span class="sxs-lookup"><span data-stu-id="99fab-112">This scenario is a good fit when reporting the app version if you're unable to successfully log into the client.</span></span>

<span data-ttu-id="99fab-113">Windows システム設定でアプリのバージョンを確認するには、[ **スタート] メニュー** を開き、[ **アプリ & 機能**] に「」と入力して、結果を選択します。</span><span class="sxs-lookup"><span data-stu-id="99fab-113">To find the app version in Windows system settings, open the **Start Menu**, type in **Apps & Features**, and select the result.</span></span> <span data-ttu-id="99fab-114">アプリの一覧で [ **Altworkplace Evr** ] に移動します。</span><span class="sxs-lookup"><span data-stu-id="99fab-114">Navigate to **AltspaceVR** in the list of apps.</span></span> <span data-ttu-id="99fab-115">[Alt] を左クリックし、表示されるメニューから [ **詳細オプション** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="99fab-115">Left-click AltspaceVR and select **Advanced Options** from the menu that appears.</span></span>

![[アプリと機能] メニューを開き、[詳細設定] オプションが強調表示されている](images/app-version-img-02.png)

<span data-ttu-id="99fab-117">[**詳細設定] オプション** の [**仕様**] ヘッダーで、[**バージョン**] ラベルの右側にアプリの **バージョン** が表示されます。</span><span class="sxs-lookup"><span data-stu-id="99fab-117">In the **Advanced Options**, under the **Specifications** header, the **App Version** should be listed to the right of the **Version** label.</span></span>

![アプリバージョンが強調表示されている状態で開く詳細設定オプション](images/app-version-img-03.png)

## <a name="in-client-logs"></a><span data-ttu-id="99fab-119">クライアントログで</span><span class="sxs-lookup"><span data-stu-id="99fab-119">In Client Logs</span></span>

<span data-ttu-id="99fab-120">Altspace Evr は、アプリケーションの起動時にクライアントログファイルのアプリバージョンを "Altspace Version" として報告します。</span><span class="sxs-lookup"><span data-stu-id="99fab-120">AltspaceVR reports the app version in the client logs file as "Altspace Version" during application startup.</span></span> <span data-ttu-id="99fab-121">これは、クライアントに正常にログインできないが、エラーが発生する前に開始しようとした場合に、アプリのバージョンを取得するのに適したオプションです。</span><span class="sxs-lookup"><span data-stu-id="99fab-121">This would be a good option to get the app version if you can't successfully log into the client, but it did attempt to start before failing.</span></span>

## <a name="windows"></a><span data-ttu-id="99fab-122">Windows</span><span class="sxs-lookup"><span data-stu-id="99fab-122">Windows</span></span>

<span data-ttu-id="99fab-123">Windows では、クライアントログファイルは Windows エクスプローラーで次の場所にあります。</span><span class="sxs-lookup"><span data-stu-id="99fab-123">On Windows, the client logs file can be found via Windows Explorer at:</span></span>

```
%userprofile%\appdata\locallow\altspacevr\altspacevr\Player.log
%userprofile%\appdata\locallow\altspacevr\altspacevr\Player-prev.log
```

<span data-ttu-id="99fab-124">このファイルは、Altworkplace Evr を起動するたびに上書きされます。</span><span class="sxs-lookup"><span data-stu-id="99fab-124">This file is overwritten each time you launch AltspaceVR.</span></span> <span data-ttu-id="99fab-125">' Player .log ' は最新のセッションを表し、' Player-prev ' は前のセッションを表します。</span><span class="sxs-lookup"><span data-stu-id="99fab-125">'Player.log' represents your latest session, and 'Player-prev.log' represents the previous session.</span></span>

## <a name="via-powershell"></a><span data-ttu-id="99fab-126">PowerShell から</span><span class="sxs-lookup"><span data-stu-id="99fab-126">Via PowerShell</span></span>

<span data-ttu-id="99fab-127">上級ユーザーは、次のように PowerShell を使用して、この文字列のクライアントログを検索できます。</span><span class="sxs-lookup"><span data-stu-id="99fab-127">Advanced users can search the client logs for this string via PowerShell as follows:</span></span>

<span data-ttu-id="99fab-128">次の内容を入力します。</span><span class="sxs-lookup"><span data-stu-id="99fab-128">Input:</span></span>

```
gc $env:userprofile\appdata\locallow\altspacevr\altspacevr\Player.log | ? { $_ -match "Altspace Version" }
```

<span data-ttu-id="99fab-129">出力:</span><span class="sxs-lookup"><span data-stu-id="99fab-129">Output:</span></span>

<span data-ttu-id="99fab-130">[2.047] Alte66c2 Evr バージョン: 3.2.23。</span><span class="sxs-lookup"><span data-stu-id="99fab-130">[2.047] AltspaceVR Version: 3.2.23.e66c2</span></span>