---
title: カスタム Skyboxes をアップロードしています
description: カスタム skyboxes のアップロードとトラブルシューティングに関する詳細な手順については、「Alt Evr エクスペリエンス」を参照してください。
ms.date: 03/11/2021
ms.topic: article
keywords: skyboxes, トラブルシューティング
ms.openlocfilehash: 02d5bc762dc36d4195100e8155d6250789e833f7
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213263"
---
# <a name="uploading-custom-skyboxes"></a><span data-ttu-id="ed77f-104">カスタム Skyboxes をアップロードしています</span><span class="sxs-lookup"><span data-stu-id="ed77f-104">Uploading custom Skyboxes</span></span>

<span data-ttu-id="ed77f-105">スカイボックスを使用すると、世界の **背景** を作成し、エクスペリエンスをさらにイマーシブにすることができます。</span><span class="sxs-lookup"><span data-stu-id="ed77f-105">A Skybox is a way to create a **background** for your World that makes the experience more immersive.</span></span> <span data-ttu-id="ed77f-106">さまざまな種類の Skyboxes がありますが、現在のところ、必要な **四角形** はサポートされています。</span><span class="sxs-lookup"><span data-stu-id="ed77f-106">There are different kinds of Skyboxes but we currently support **equirectangular**.</span></span> <span data-ttu-id="ed77f-107">360カメラを使用した例を次に示します ( [こちら](http://moments.mankindforward.com/)の例を参照)。</span><span class="sxs-lookup"><span data-stu-id="ed77f-107">Here's an example taken with a 360 camera (more example [here](http://moments.mankindforward.com/)):</span></span> 

![360生きた部屋を四角形で表示する](images/custom-skyboxes-img-01.jpeg)

<span data-ttu-id="ed77f-109">[Unity アップローダー](world-building-toolkit-getting-started.md)を使用することもできますが、この方法はより簡単です。</span><span class="sxs-lookup"><span data-stu-id="ed77f-109">You can also use the [Unity Uploader](world-building-toolkit-getting-started.md) but this approach is simpler.</span></span>

1. <span data-ttu-id="ed77f-110">[ [ワールド > Skyboxes](https://account.altvr.com/skyboxes) に移動し、右側にある [ **作成** ] ボタンを押します。</span><span class="sxs-lookup"><span data-stu-id="ed77f-110">Navigate to [Worlds > Skyboxes](https://account.altvr.com/skyboxes) and press the **Create** button on the right</span></span>

![Skyboxes パネルに開いているワールド web サイトページ](images/custom-skyboxes-img-02.png)

2. <span data-ttu-id="ed77f-112">名前を入力し、360イメージを指定します。</span><span class="sxs-lookup"><span data-stu-id="ed77f-112">Fill in a name and specify your 360 image.</span></span> <span data-ttu-id="ed77f-113">写真である必要はありません。独自に作成したり、オンラインで検索したりできるプログラムがあります。</span><span class="sxs-lookup"><span data-stu-id="ed77f-113">It doesn't have to be a photo, there are programs that let you draw your own or you can search for some online.</span></span> <span data-ttu-id="ed77f-114">準備ができたら、 **[作成]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ed77f-114">When you're ready, select **Create**.</span></span> 

![スカイボックス作成フォーム](images/custom-skyboxes-img-03.png)

3. <span data-ttu-id="ed77f-116">必要に応じて、このスカイボックスを簡単に識別できるように **プレビュー** イメージをアップロードすることができます。</span><span class="sxs-lookup"><span data-stu-id="ed77f-116">You can optionally upload a **preview** image so you can easily identify this skybox.</span></span> <span data-ttu-id="ed77f-117">また、WAV 形式でアンビエントオーディオをアップロードすることもできます。</span><span class="sxs-lookup"><span data-stu-id="ed77f-117">You can also upload ambient audio in WAV format.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="ed77f-118">360イメージをアップロードした後に、プレビューイメージとアンビエントオーディオを個別にアップロードすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="ed77f-118">We recommend you upload preview images and ambient audio separately, after you upload the 360 image.</span></span> <span data-ttu-id="ed77f-119">これらをまとめてアップロードすると、ファイルサイズが十分に大きくなり、プロセスが停止する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ed77f-119">If you upload them together the file sizes can be large enough to stall the process.</span></span> <span data-ttu-id="ed77f-120">[Jetsons World](https://account.altvr.com/worlds/1004174988393054363/spaces/1084431533181240311) は、スカイボックスをアンビエントオーディオと共に使用する方法の好例です。</span><span class="sxs-lookup"><span data-stu-id="ed77f-120">[Jetsons World](https://account.altvr.com/worlds/1004174988393054363/spaces/1084431533181240311) is a great example of how to use a Skybox with ambient audio.</span></span> <span data-ttu-id="ed77f-121">Annoyed が聞こえないように、世界のビルダーによってオーディオボリュームが低に保たれ、音が鳴ります。</span><span class="sxs-lookup"><span data-stu-id="ed77f-121">Notice how the World-Builder kept the audio volume low and sounds you hear are sporadic so people don't get annoyed.</span></span> 

4. <span data-ttu-id="ed77f-122">世界を入力して、世界のエディターを開きます。</span><span class="sxs-lookup"><span data-stu-id="ed77f-122">Enter your World and open the World Editor.</span></span> <span data-ttu-id="ed77f-123">[Skyboxes] で、新しいスカイボックスを選択します。</span><span class="sxs-lookup"><span data-stu-id="ed77f-123">Under Skyboxes, select your new Skybox.</span></span> <span data-ttu-id="ed77f-124">数秒で、空のままになります。</span><span class="sxs-lookup"><span data-stu-id="ed77f-124">In a few seconds, the sky will literally change.</span></span> <span data-ttu-id="ed77f-125">また、世界中の他のユーザーも、空の変更を見ることができます。</span><span class="sxs-lookup"><span data-stu-id="ed77f-125">Others in your World will also see the sky change.</span></span> <span data-ttu-id="ed77f-126">元に戻すには、同じリスト内の **既定** のスカイボックスを選択します。</span><span class="sxs-lookup"><span data-stu-id="ed77f-126">To switch back, choose the **default** skybox in that same list.</span></span> 

## <a name="troubleshooting"></a><span data-ttu-id="ed77f-127">トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="ed77f-127">Troubleshooting</span></span>

<span data-ttu-id="ed77f-128">**空の場合は、継ぎ目や線があります。**</span><span class="sxs-lookup"><span data-stu-id="ed77f-128">**There's a seam or line in the sky :-(.**</span></span> <span data-ttu-id="ed77f-129">間もなく修正されるバグです。</span><span class="sxs-lookup"><span data-stu-id="ed77f-129">It's a bug that we'll fix soon</span></span>

<span data-ttu-id="ed77f-130">**アップロード失敗**</span><span class="sxs-lookup"><span data-stu-id="ed77f-130">**Upload failed**</span></span>
    * <span data-ttu-id="ed77f-131">360イメージだけをアップロードしてみてください。</span><span class="sxs-lookup"><span data-stu-id="ed77f-131">try uploading just the 360 image on its own</span></span>
    * <span data-ttu-id="ed77f-132">テストとして別の小さいファイルを試してみる</span><span class="sxs-lookup"><span data-stu-id="ed77f-132">try with another, smaller file as a test</span></span>

<span data-ttu-id="ed77f-133">**360の写真が見つかりません**</span><span class="sxs-lookup"><span data-stu-id="ed77f-133">**I can't find a 360 photo**</span></span>
    * <span data-ttu-id="ed77f-134">Flickr は優れたソースです (creative commons を見つけるためのフィルターを変更してください)</span><span class="sxs-lookup"><span data-stu-id="ed77f-134">Flickr is a good source (change the filters to find creative commons ones)</span></span>
    * <span data-ttu-id="ed77f-135">ご自分でご利用ください。</span><span class="sxs-lookup"><span data-stu-id="ed77f-135">Take your own!</span></span> <span data-ttu-id="ed77f-136">Ricoh のカメラで成功しました。</span><span class="sxs-lookup"><span data-stu-id="ed77f-136">We've had success with Ricoh's cameras.</span></span> 
<span data-ttu-id="ed77f-137">**スカイスカイまたはむらが見て** くる高解像度のイメージを検索することが必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="ed77f-137">**The sky looks grainy or blocky** You may need to find a higher-resolution image.</span></span> <span data-ttu-id="ed77f-138">通常は約 2-5 MB、~ 5000 px x 2000 px</span><span class="sxs-lookup"><span data-stu-id="ed77f-138">Typically around 2-5 MB and ~5000 px x 2000 px</span></span>

<span data-ttu-id="ed77f-139">**世界のフレームレートが低下します。**</span><span class="sxs-lookup"><span data-stu-id="ed77f-139">**It hurts my World's framerate!**</span></span>
<span data-ttu-id="ed77f-140">画像が大きすぎる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ed77f-140">The image is probably too large.</span></span> <span data-ttu-id="ed77f-141">生成される skyboxes には、8k の場合もあります。</span><span class="sxs-lookup"><span data-stu-id="ed77f-141">Some generated skyboxes can be 8k.</span></span> <span data-ttu-id="ed77f-142">通常、モバイル対応の2k バージョンが付属しています。</span><span class="sxs-lookup"><span data-stu-id="ed77f-142">They usually come with mobile-friendly 2k versions--use that.</span></span>

<span data-ttu-id="ed77f-143">**アンビエントオーディオに関するヘルプ**</span><span class="sxs-lookup"><span data-stu-id="ed77f-143">**Help me with the ambient audio**</span></span>
    * <span data-ttu-id="ed77f-144">Audacity のような無料のソフトウェアを使用して、ボリュームを減らしたり、独自のループを作成したりします。</span><span class="sxs-lookup"><span data-stu-id="ed77f-144">Use free software like Audacity to lower the volume or create your own loops.</span></span> <span data-ttu-id="ed77f-145">オーディオは、人間の耳で繰り返されて再生されるので、邪魔にならないようにしてください。</span><span class="sxs-lookup"><span data-stu-id="ed77f-145">Remember that the audio will be repeated and playing in people's ears so keep it low and not annoying</span></span>
    * <span data-ttu-id="ed77f-146">[無料サウンド](https://freesound.org/) は、ロイヤリティフリーサウンドを利用するのに適しています。</span><span class="sxs-lookup"><span data-stu-id="ed77f-146">[Free Sound](https://freesound.org/) is a good source of royalty-free sounds</span></span>
