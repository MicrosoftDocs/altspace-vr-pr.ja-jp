---
title: GlTF モデルのインポート
description: 3D glTF モデルを正常にインポートして、問題のトラブルシューティングを行う方法について説明します。
ms.date: 03/11/2021
ms.topic: article
keywords: モデル, glTF, インポート, sketchfab, トラブルシューティング
ms.openlocfilehash: 4489f90832bd1cf85ff161caed11684257cce6ab
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213258"
---
# <a name="importing-gltf-models"></a><span data-ttu-id="700ac-104">GlTF モデルのインポート</span><span class="sxs-lookup"><span data-stu-id="700ac-104">Importing glTF models</span></span>

> [!NOTE]
> <span data-ttu-id="700ac-105">この機能は、現時点では、早期アクセスプログラムのユーザーが選択できるようになっています。</span><span class="sxs-lookup"><span data-stu-id="700ac-105">This feature is available for select users in the Early Access program at this time.</span></span>

<span data-ttu-id="700ac-106">3D モデルとシーンを Altspace に取り込む1つの方法は、 [Gltf 標準](https://en.wikipedia.org/wiki/GlTF)を使用することです。</span><span class="sxs-lookup"><span data-stu-id="700ac-106">One way to bring 3D models and scenes into Altspace is using the [glTF standard](https://en.wikipedia.org/wiki/GlTF).</span></span> <span data-ttu-id="700ac-107">Glb ファイル (パックされた glTF) をアップロードして、後でワールドエディターで生成できるモデルを作成できます。</span><span class="sxs-lookup"><span data-stu-id="700ac-107">You can upload a .glb file (packed glTF) to create a Model that you can later spawn in the World Editor.</span></span> <span data-ttu-id="700ac-108">[独自のキットをアップロード](uploading-custom-kits.md)する代わりに使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="700ac-108">It's an alternative to [uploading your own Kits](uploading-custom-kits.md).</span></span> <span data-ttu-id="700ac-109">クイックデモ用のモデルを作成することをお勧めします。これは、Unity を使用する必要がなく、パフォーマンスと再利用性を最大化する場合にキットを使用する必要がないためです。</span><span class="sxs-lookup"><span data-stu-id="700ac-109">We recommend creating Models for quick demonstrations because you won't need to use Unity, and Kits when you want to maximize performance and reusability.</span></span> 

1. <span data-ttu-id="700ac-110">GlTF 3D アセットをいくつか検索します。</span><span class="sxs-lookup"><span data-stu-id="700ac-110">Find some glTF 3D assets.</span></span> <span data-ttu-id="700ac-111">検索する場所の1つは Sketchfab です ([この](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models)ような **ダウンロード** 可能なモデルをフィルター処理してみてください)。</span><span class="sxs-lookup"><span data-stu-id="700ac-111">One place to search is Sketchfab (try filtering for **Downloadable** models like [this](https://sketchfab.com/search?features=downloadable&q=low+poly+wolf&sort_by=-pertinence&type=models)).</span></span> <span data-ttu-id="700ac-112">見つかったら、[ **3D モデルのダウンロード**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="700ac-112">Once you find it, select **Download 3D Model**:</span></span>

![Sketchfab からの 3D dog モデル](images/importing-models-img-01.png)

2. <span data-ttu-id="700ac-114">モデルへのリンクをコピーし、ライセンス要件を確認します。</span><span class="sxs-lookup"><span data-stu-id="700ac-114">Copy the link to the model and read the licensing requirements.</span></span> 
3. <span data-ttu-id="700ac-115">**Autoconverted 形式 (glTF)** バージョンのダウンロード</span><span class="sxs-lookup"><span data-stu-id="700ac-115">Download the **Autoconverted Format (glTF)** version</span></span>

![自動変換形式が強調表示されている Sketchfab ダウンロードオプション](images/importing-models-img-02.png)

4. <span data-ttu-id="700ac-117">[GLB Packer](https://glb-packer.glitch.me)サイトを開き、[ **PNG を JPEG に変換する (ベータ版)** ] チェックボックスをオンにします。</span><span class="sxs-lookup"><span data-stu-id="700ac-117">Open the [GLB Packer](https://glb-packer.glitch.me) site and check the box **Convert PNG to JPEG (beta)**</span></span>
5. <span data-ttu-id="700ac-118">ダウンロードした glTF ファイルを圧縮解除し、[GLB Packer ブラウザー] タブに一度にドラッグします。</span><span class="sxs-lookup"><span data-stu-id="700ac-118">Uncompress the glTF files you downloaded and drag them all at once into the GLB Packer browser tab</span></span>

![モデルの圧縮解除を示すウィンドウ](images/importing-models-img-03.png)

6. <span data-ttu-id="700ac-120">ファイルの数とサイズによっては、処理に時間がかかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="700ac-120">Depending on the number and size of the files, it may take a while to process.</span></span> <span data-ttu-id="700ac-121">処理が完了すると、 **glb** ファイルがダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="700ac-121">When processing is done, an **out.glb** file will be downloaded.</span></span> <span data-ttu-id="700ac-122">このファイルの名前をわかりやすい名前に変更します。これは、世界中のオブジェクトの名前になります (例: **Poly glb)。**</span><span class="sxs-lookup"><span data-stu-id="700ac-122">Rename that file to something informative--this will be the name of the object in the world (e.g **Low Poly Wolf.glb**)</span></span>
7. <span data-ttu-id="700ac-123">Altvr.com に移動し [> モデルを >](https://account.altvr.com/users/sign_in)し、[**作成**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="700ac-123">Navigate to [altvr.com > More > Models](https://account.altvr.com/users/sign_in) and select **Create**</span></span>
8. <span data-ttu-id="700ac-124">Glb ファイルの場所を指定し、Sketchfab リンクを [属性] の [説明] にコピーします。</span><span class="sxs-lookup"><span data-stu-id="700ac-124">Specify the location of the .glb file and make sure you copy the Sketchfab link into the description for attribution.</span></span> <span data-ttu-id="700ac-125">必要に応じてプレビューイメージを指定し、[ **モデルの作成**] を選択できます。</span><span class="sxs-lookup"><span data-stu-id="700ac-125">You can specify a preview image if you want, then select **Create Model**:</span></span>

![Altworkplace Evr のモデルプレビュー](images/importing-models-img-04.png)

9. <span data-ttu-id="700ac-127">[**クリップボードにコピー** ] を選択</span><span class="sxs-lookup"><span data-stu-id="700ac-127">Select **Copy to Clipboard**</span></span>
10. <span data-ttu-id="700ac-128">**World Editor > > の基本 > GLTF** を開きます。</span><span class="sxs-lookup"><span data-stu-id="700ac-128">Open the **World Editor > Altspace > Basics > GLTF**</span></span>
11. <span data-ttu-id="700ac-129">Url を貼り付け、[**確認**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="700ac-129">Paste in your url and select **Confirm**</span></span>

<span data-ttu-id="700ac-130">おめでとうございます!</span><span class="sxs-lookup"><span data-stu-id="700ac-130">Congrats!</span></span> <span data-ttu-id="700ac-131">最初のモデルを生成しただけです。</span><span class="sxs-lookup"><span data-stu-id="700ac-131">You just spawned your first Model.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="700ac-132">トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="700ac-132">Troubleshooting</span></span>

<span data-ttu-id="700ac-133">**何も起こっていない **ことを確認** したとき**</span><span class="sxs-lookup"><span data-stu-id="700ac-133">**When I clicked **Confirm** nothing happened**</span></span>
    * <span data-ttu-id="700ac-134">現在、10万の多角形の制限があります。</span><span class="sxs-lookup"><span data-stu-id="700ac-134">We currently have a 100k polygon limit.</span></span> <span data-ttu-id="700ac-135">失敗した場合は、オブジェクトを削除して、世界中のユーザーによる潜在的な問題を回避します。</span><span class="sxs-lookup"><span data-stu-id="700ac-135">If it fails, delete the Object to avoid potential problems with users joining your World</span></span>
    * <span data-ttu-id="700ac-136">資産に他の問題がある可能性があります。</span><span class="sxs-lookup"><span data-stu-id="700ac-136">There may be other problems with the asset.</span></span> <span data-ttu-id="700ac-137">できるだけ少ない数のポリゴンでアセットを使用してみてください。</span><span class="sxs-lookup"><span data-stu-id="700ac-137">Try to use assets with as few polygons as possible.</span></span>
    * <span data-ttu-id="700ac-138">使用するモデルが小さいか、または大きい可能性があります。</span><span class="sxs-lookup"><span data-stu-id="700ac-138">The model you're bringing in may be small or large.</span></span> <span data-ttu-id="700ac-139">拡大/縮小するか、アバターを移動してみてください。モデル内に存在している可能性があります。</span><span class="sxs-lookup"><span data-stu-id="700ac-139">Try increasing/decreasing the Scale or move your avatar around, you might be standing inside the model!</span></span>

<span data-ttu-id="700ac-140">**読み込みに時間がかかる** 世界中の他のユーザーがどれだけ高速に負荷をかけるかは、接続速度によって異なります。</span><span class="sxs-lookup"><span data-stu-id="700ac-140">**It's slow to load** How quickly other users in the World load it will depend on their connection speeds.</span></span> <span data-ttu-id="700ac-141">また、キット資産と同様にキャッシュされません。</span><span class="sxs-lookup"><span data-stu-id="700ac-141">It's also not cached like Kit assets.</span></span> <span data-ttu-id="700ac-142">ホームに配置した場合は、結合するたびに同じモデルが再ダウンロードされますが、これはそれほど優れていません。</span><span class="sxs-lookup"><span data-stu-id="700ac-142">If you place one in your Home, you'll end up redownloading the same Model every time you join, which isn't great.</span></span>

<span data-ttu-id="700ac-143">**競合はありません** 既定では、この方法で発生するオブジェクトの競合は発生しません。</span><span class="sxs-lookup"><span data-stu-id="700ac-143">**There's no collision** By default there's no collision on the objects that are brought in this way</span></span>

<span data-ttu-id="700ac-144">**コントロールを生成すると、6度の自由にコントロールが失われるか、操作が困難** になります。はい、これらの問題について認識し、近日中に対応することを願っています。</span><span class="sxs-lookup"><span data-stu-id="700ac-144">**When I spawn it, I lose my controls on six DOF or I'm inside so it's hard to manipulate it** Yes, we're aware of these issues and hope to address them soon.</span></span>  