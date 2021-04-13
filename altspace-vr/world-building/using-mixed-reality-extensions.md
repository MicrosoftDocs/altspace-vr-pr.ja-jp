---
title: Mixed Reality 拡張機能の使用
description: Mixed Reality 拡張機能を使用してトラブルシューティングを行って、Altの範囲を拡張して適応させる方法について説明します。
ms.date: 03/11/2021
ms.topic: article
keywords: mixed reality、拡張機能、トラブルシューティング
ms.openlocfilehash: 498e71c48f7c67abc40ce4f4667c9eeac4c4e73b
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212642"
---
# <a name="using-a-mixed-reality-extension"></a><span data-ttu-id="7b8ae-104">Mixed Reality 拡張機能の使用</span><span class="sxs-lookup"><span data-stu-id="7b8ae-104">Using a Mixed Reality Extension</span></span>

<span data-ttu-id="7b8ae-105">[Mixed Reality 拡張機能](https://developer.altvr.com/) (mres) は、 [ヘルメット](https://account.altvr.com/mres/1173667287173955931) から実用的な [stargate](https://account.altvr.com/mres/1152987031857529562)まで、世界で使用できるアプリです。</span><span class="sxs-lookup"><span data-stu-id="7b8ae-105">[Mixed Reality Extensions](https://developer.altvr.com/) (MREs) are apps you can use in your Worlds from [helmets](https://account.altvr.com/mres/1173667287173955931) to a working [Stargate](https://account.altvr.com/mres/1152987031857529562).</span></span> <span data-ttu-id="7b8ae-106">これは、プログラミングエクスペリエンスを持つコミュニティメンバーが、Altspace および一方向のビルダーを拡張して、世界の対話性を高めることができるようにする方法です。</span><span class="sxs-lookup"><span data-stu-id="7b8ae-106">This is how community members with programming experience can extend Altspace and one-way World Builders can make their Worlds more interactive.</span></span> <span data-ttu-id="7b8ae-107">MREs は世界中のだれでも使用できますが、世界で MREs を参照して起動できるのは、世界中のプログラムのユーザーだけです。</span><span class="sxs-lookup"><span data-stu-id="7b8ae-107">While MREs can be used by anyone in a World, only people in the World Building Program can browse and spawn MREs in their Worlds.</span></span> 

1. <span data-ttu-id="7b8ae-108">[Web サイト](https://account.altvr.com/mres)の mre セクションを参照します。</span><span class="sxs-lookup"><span data-stu-id="7b8ae-108">Browse the MRE section of our [website](https://account.altvr.com/mres).</span></span> <span data-ttu-id="7b8ae-109">既定では、独自の MREs が表示されるので、[ **Altspace** ] を選択して、コミュニティからの mres を確認するための正式な Mres と **おすすめ** を表示します。</span><span class="sxs-lookup"><span data-stu-id="7b8ae-109">By default you'll see your own MREs so select on **Altspace** to see official MREs and **Featured** to see MREs from the community.</span></span> <span data-ttu-id="7b8ae-110">お客様の世界で使用する前に、すべての MRE を使い始めることができます。</span><span class="sxs-lookup"><span data-stu-id="7b8ae-110">Get familiar with any MRE before you use it in your World.</span></span> 
2. <span data-ttu-id="7b8ae-111">[ [ヘルメット](https://account.altvr.com/mres/1173667287173955931) mre] に移動し、[ **クリップボードにコピー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b8ae-111">Navigate to the [Helmets](https://account.altvr.com/mres/1173667287173955931) MRE and select **Copy to Clipboard**.</span></span> 
3. <span data-ttu-id="7b8ae-112">世界を入力し、World Editor を開いて **> SDK アプリ** を作成します。</span><span class="sxs-lookup"><span data-stu-id="7b8ae-112">Enter your World and open the World Editor to **Basics > SDK App**.</span></span> <span data-ttu-id="7b8ae-113">[ターゲット URI] フィールドに [ヘルメット] の URL を貼り付け、[ **確認**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b8ae-113">Paste in the URL for Helmets into the Target URI field and select **Confirm**.</span></span> <span data-ttu-id="7b8ae-114">MRE オブジェクトが表示され、クラウドで実行されている MRE に接続しようとします。</span><span class="sxs-lookup"><span data-stu-id="7b8ae-114">The MRE Object should appear and attempt to connect to the MRE that's running in the cloud.</span></span> <span data-ttu-id="7b8ae-115">これで、クリックできるヘルメットが表示されます。</span><span class="sxs-lookup"><span data-stu-id="7b8ae-115">You should now see some helmets you can click on.</span></span>
4. <span data-ttu-id="7b8ae-116">他のワールドオブジェクトと同様に、MRE の移動/回転/拡大/縮小を行います。</span><span class="sxs-lookup"><span data-stu-id="7b8ae-116">Move/rotate/scale the MRE just as you would any other World Object.</span></span>

<span data-ttu-id="7b8ae-117">おめでとうございます。</span><span class="sxs-lookup"><span data-stu-id="7b8ae-117">Congratulations!</span></span> <span data-ttu-id="7b8ae-118">現在、MREs を使用しています。すばらしいですね。</span><span class="sxs-lookup"><span data-stu-id="7b8ae-118">You're using MREs now--you're so cool!</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="7b8ae-119">トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="7b8ae-119">Troubleshooting</span></span>

<span data-ttu-id="7b8ae-120">**MRE は不機嫌な絵文字を表示しています**</span><span class="sxs-lookup"><span data-stu-id="7b8ae-120">**MRE is showing a frowning emoji**</span></span> 
    * <span data-ttu-id="7b8ae-121">URL が正しいことを確認してください</span><span class="sxs-lookup"><span data-stu-id="7b8ae-121">Verify that the URL is correct</span></span>
    * <span data-ttu-id="7b8ae-122">オブジェクトの [**再生中**] オプションをオンにして、[**確認**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b8ae-122">Toggle **Is Playing** option on the Object and choose **confirm**</span></span>
    * <span data-ttu-id="7b8ae-123">再入</span><span class="sxs-lookup"><span data-stu-id="7b8ae-123">Try reentering</span></span>

<span data-ttu-id="7b8ae-124">**Mre は遅れている** MRE がホストされている場所によっては、ネットワーク待機時間が発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="7b8ae-124">**MRE is lagging** Depending on where an MRE is hosted you may experience some network latency</span></span>

<span data-ttu-id="7b8ae-125">**Url を貼り付ける必要があるのはなぜですか。**</span><span class="sxs-lookup"><span data-stu-id="7b8ae-125">**Why do we have to paste URLs?**</span></span>
<span data-ttu-id="7b8ae-126">今後、キットの成果物と同様に、MREs を管理して起動することができます。</span><span class="sxs-lookup"><span data-stu-id="7b8ae-126">In the future, you can manage and spawn MREs like you do Artifacts from Kits.</span></span> <span data-ttu-id="7b8ae-127">それまでは引き続き Url を使用します。</span><span class="sxs-lookup"><span data-stu-id="7b8ae-127">Until then, we'll continue using URLs</span></span>