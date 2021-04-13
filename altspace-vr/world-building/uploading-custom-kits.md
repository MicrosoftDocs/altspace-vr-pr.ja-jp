---
title: カスタムキットのアップロード
description: 独自のカスタムキットを Altworkplace Evr でセットアップ、生成、アップロードする方法、およびトラブルシューティングのヘルプについて説明します。
ms.date: 03/11/2021
ms.topic: article
keywords: キット, アップロード, トラブルシューティング
ms.openlocfilehash: e5a1b9c2ef5339db0cb821cb6f7d21a930416451
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213506"
---
# <a name="uploading-custom-kits"></a><span data-ttu-id="cd258-104">カスタムキットのアップロード</span><span class="sxs-lookup"><span data-stu-id="cd258-104">Uploading custom kits</span></span>

<span data-ttu-id="cd258-105">世界中のエディターには、世界中に生成可能な成果物を含むキットがあります。</span><span class="sxs-lookup"><span data-stu-id="cd258-105">The World Editor has Kits containing Artifacts that you can spawn into your World.</span></span> <span data-ttu-id="cd258-106">たとえば、 [Campfire Kit](https://account.altvr.com/kits/993516233267609824) にはさまざまな種類のツリーがあります。ツリーの各種類は成果物です。</span><span class="sxs-lookup"><span data-stu-id="cd258-106">For example, the [Campfire Kit](https://account.altvr.com/kits/993516233267609824) has many types of trees--each type of tree is an Artifact.</span></span> <span data-ttu-id="cd258-107">独自のキットを作成するには、Unity AssetBundles を作成し、各アーティファクトの Unity Prefab を含む .zip ファイルをアップロードして、web サイトに各アイテムを登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="cd258-107">To create your own Kit, you have to create Unity AssetBundles and upload a .zip file containing a Unity Prefab for each Artifact and register each Artifact on our website.</span></span> <span data-ttu-id="cd258-108">幸いなことに、コミュニティ主導の Unity アップローダーは、ほとんどのワークフローを自動化しています。</span><span class="sxs-lookup"><span data-stu-id="cd258-108">Fortunately, the community-driven Unity Uploader automates most of the workflow.</span></span> <span data-ttu-id="cd258-109">アップロードが完了すると、世界中のキットからオブジェクトを生成し、他のユーザーがそれらを自動的に確認できるようになります。</span><span class="sxs-lookup"><span data-stu-id="cd258-109">Once uploaded, you can spawn objects from your own Kits in your Worlds and other users can automatically see them.</span></span> <span data-ttu-id="cd258-110">その後、キットを友人と共有したり、コミュニティ全体を利用したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="cd258-110">Later, you can share your Kit with your friends or even with the entire Community by being featured.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd258-111">前提条件</span><span class="sxs-lookup"><span data-stu-id="cd258-111">Prerequisites</span></span>

1. [<span data-ttu-id="cd258-112">Unity Hub と Unity のインストール</span><span class="sxs-lookup"><span data-stu-id="cd258-112">Install Unity Hub and Unity</span></span>](world-building-toolkit-getting-started.md)
2. <span data-ttu-id="cd258-113">[Unity アップローダー](https://altvr.com/download-latest-unity-uploader/)の最新バージョンをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="cd258-113">Download the latest version of the [Unity Uploader](https://altvr.com/download-latest-unity-uploader/)</span></span>

## <a name="setup"></a><span data-ttu-id="cd258-114">セットアップ</span><span class="sxs-lookup"><span data-stu-id="cd258-114">Setup</span></span> 

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-1-Setup/player]

1. <span data-ttu-id="cd258-115">世界中の web サイトでキットを作成する [> キット](https://account.altvr.com/kits)</span><span class="sxs-lookup"><span data-stu-id="cd258-115">Create a Kit on our website at [Worlds > Kits](https://account.altvr.com/kits)</span></span>
2. <span data-ttu-id="cd258-116">ブラウザーのアドレスバーのキット ID をクリップボードにコピーします (この手順はアップローダーバージョン0.9 以降では簡単です)。</span><span class="sxs-lookup"><span data-stu-id="cd258-116">Copy the Kit ID from your browser's address bar to your clipboard (this step will be easier in Uploader versions 0.9+)</span></span>
3. <span data-ttu-id="cd258-117">新しい Unity プロジェクトを作成する</span><span class="sxs-lookup"><span data-stu-id="cd258-117">Create a new Unity Project</span></span>
4. <span data-ttu-id="cd258-118">パッケージをダブルクリックして Unity アップローダーをインポートする</span><span class="sxs-lookup"><span data-stu-id="cd258-118">Import the Unity Uploader by double-clicking the package</span></span>

![インポートされた unity アップローダーパッケージ](images/custom-kits-img-01.png)

5. <span data-ttu-id="cd258-120">アップローダーに、Altspace 電子メールとパスワードを使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="cd258-120">Sign in to the Uploader with your Altspace email and password</span></span>

![Unity の Altworkplace Evr サインインインターフェイス](images/custom-kits-img-02.png)

## <a name="generate-and-upload-your-kit"></a><span data-ttu-id="cd258-122">キットの生成とアップロード</span><span class="sxs-lookup"><span data-stu-id="cd258-122">Generate and upload your kit</span></span>

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-my-own-Kits-Part-2/player]

1. <span data-ttu-id="cd258-123">キットの **フォルダー名** をプレフィックスとテーマとしてキット id ( **1137484494681408069_pirates** など) に入力し、キットの **資産名** をプレフィックスとしてキット id に入力します。</span><span class="sxs-lookup"><span data-stu-id="cd258-123">Fill in **Kit Folder Name** with your Kit ID as the prefix and a theme (for example, **1137484494681408069_pirates**) and fill in **Kit Asset Name** with your Kit ID as the prefix.</span></span> <span data-ttu-id="cd258-124">すべての資産にこのプレフィックスを付ける必要があります。</span><span class="sxs-lookup"><span data-stu-id="cd258-124">All the assets will need to have this prefix.</span></span>

![Unity での、Kit フォルダー名を使用した Altて Evr インターフェイス](images/custom-kits-img-03.png)

2. <span data-ttu-id="cd258-126">各アイテムまたはアイテムのセットについて、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="cd258-126">For each Artifact or set of Artifacts:</span></span>
* <span data-ttu-id="cd258-127">ソース Prefab を [階層] タブにドラッグします。</span><span class="sxs-lookup"><span data-stu-id="cd258-127">Drag your source Prefab(s) into the Hierarchy tab</span></span>
* <span data-ttu-id="cd258-128">セットに含めるものを選択します。たとえば、5種類のバレル</span><span class="sxs-lookup"><span data-stu-id="cd258-128">Select the ones you want to include in a set, say five types of barrels</span></span>
* <span data-ttu-id="cd258-129">キットの **資産名** を **バレル** で更新する</span><span class="sxs-lookup"><span data-stu-id="cd258-129">Update the **Kit Asset Name** with **barrel**</span></span>
* <span data-ttu-id="cd258-130">[**複数のオブジェクトを Kit Prefab に変換する**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="cd258-130">Select **Convert GameObject(s) to Kit Prefab**</span></span>
* <span data-ttu-id="cd258-131">Assets/Prefabs フォルダーに新しい Prefabs とスクリーンショットが作成されたことを確認します。</span><span class="sxs-lookup"><span data-stu-id="cd258-131">Verify that new Prefabs and Screenshots were created in the Assets/Prefabs folder</span></span>

![Unity でアーティファクトが選択されている場合は、Altて Evr インターフェイス](images/custom-kits-img-04.png)

> [!NOTE]
> <span data-ttu-id="cd258-133">生成された Prefab を変更する場合は、階層にドラッグして変更を加え、[インスペクター] タブの [ **適用** ] をクリックして、prefab を更新します。</span><span class="sxs-lookup"><span data-stu-id="cd258-133">If you want to make any modifications to a generated Prefab, drag it back into the Hierarchy, make changes, and then click **Apply** in the Inspector tab to update the Prefab.</span></span> 

3. <span data-ttu-id="cd258-134">準備ができたら、[アップローダー] タブを下にスクロールして、アセットバンドルを含む zip ファイルを生成する準備をします。</span><span class="sxs-lookup"><span data-stu-id="cd258-134">When you're ready, scroll down the Uploader tab and let's prepare to generate a zip file with the Asset Bundle</span></span>
4. <span data-ttu-id="cd258-135">より迅速なイテレーションを行うには、 **Android 用のビルドキット** のチェックボックスをオフにします。</span><span class="sxs-lookup"><span data-stu-id="cd258-135">For faster iteration, uncheck the **Build Kit for Android?**.</span></span> <span data-ttu-id="cd258-136">反復処理が完了した後、またはキットを共有または機能させたい場合は、後で Android 用のバージョンをビルドしてアップロードしてください。</span><span class="sxs-lookup"><span data-stu-id="cd258-136">Remember to build and upload a version for Android later when you're done iterating or want to share/feature your Kit.</span></span> 
5. <span data-ttu-id="cd258-137">**ロードキットの Prefab ディレクトリ** の選択</span><span class="sxs-lookup"><span data-stu-id="cd258-137">Select **Load Kit Prefab Directories**</span></span>
6. <span data-ttu-id="cd258-138">キットフォルダー名と一致するものの横にある [ **ビルド** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="cd258-138">Choose **Build** next to the one matching your Kit Folder Name.</span></span> <span data-ttu-id="cd258-139">同じ Unity プロジェクトから複数のキットを生成するのが一般的です。</span><span class="sxs-lookup"><span data-stu-id="cd258-139">It's common to produce multiple Kits from the same Unity project.</span></span> <span data-ttu-id="cd258-140">キットのサイズによっては、しばらく時間がかかることがあります。</span><span class="sxs-lookup"><span data-stu-id="cd258-140">This may take a while depending on the size of your Kit.</span></span> <span data-ttu-id="cd258-141">完了すると、zip ファイルを含むフォルダーが自動的に開きます。</span><span class="sxs-lookup"><span data-stu-id="cd258-141">When it's done, the folder containing your zip file will open automatically.</span></span> 
7. <span data-ttu-id="cd258-142">Web サイトにアクセスし、前の手順で作成したキットを編集して、作成した zip ファイルをアップロードします。</span><span class="sxs-lookup"><span data-stu-id="cd258-142">Go to the website, edit the Kit you created earlier, and upload the zip file you produced.</span></span> <span data-ttu-id="cd258-143">ファイルのサイズによっては、アップロードに時間がかかることがあります。</span><span class="sxs-lookup"><span data-stu-id="cd258-143">This upload may take a while depending on the file size.</span></span>
    * <span data-ttu-id="cd258-144">正常に実行された場合は、ファイルサイズと PC および Android の [アップロード] の下に、最後に更新された日時が表示されます。</span><span class="sxs-lookup"><span data-stu-id="cd258-144">If successful, you’ll see on the left side under “Uploads” the file sizes and for PC and Android and when they were last updated</span></span>
    * <span data-ttu-id="cd258-145">失敗した場合は、スクリプトがないことを確認し、スクリプトをサポートしていないことを確認して、セキュリティを確認してから、もう一度やり直してください。</span><span class="sxs-lookup"><span data-stu-id="cd258-145">If unsuccessful, make sure you don't have any scripts, we don't support scripts, we check for those for security and try again.</span></span>

<span data-ttu-id="cd258-146">おめでとうございます。</span><span class="sxs-lookup"><span data-stu-id="cd258-146">Congratulations!</span></span> <span data-ttu-id="cd258-147">独自のキットを使用して、世界を構築する準備ができました。</span><span class="sxs-lookup"><span data-stu-id="cd258-147">You're ready to build Worlds with your own Kit!</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="cd258-148">トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="cd258-148">Troubleshooting</span></span> 

<span data-ttu-id="cd258-149">**制限はありますか。**</span><span class="sxs-lookup"><span data-stu-id="cd258-149">**Are there limits?**</span></span>
<span data-ttu-id="cd258-150">ハード制限はまだありませんが、1つの成果物のみが使用されている場合でも、ユーザーはキット全体のプラットフォームの AssetBundle をダウンロードする必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="cd258-150">There are no hard limits yet but remember that users need to download the AssetBundle for their platform for the entire Kit even if only one Artifact is used.</span></span> <span data-ttu-id="cd258-151">プラットフォームごとのダウンロードを 5 MB 以下にしてください。</span><span class="sxs-lookup"><span data-stu-id="cd258-151">Try to keep the download per-platform to 5 MB or less.</span></span> <span data-ttu-id="cd258-152">これを行う1つの方法は、小さなキットに分割することです。</span><span class="sxs-lookup"><span data-stu-id="cd258-152">One way to do that is to split up things into smaller Kits.</span></span> <span data-ttu-id="cd258-153">たとえば、200 props は半分に分割する必要があります。</span><span class="sxs-lookup"><span data-stu-id="cd258-153">For example, 200 props should split in half.</span></span> 

<span data-ttu-id="cd258-154">**"スプリットアイ"**</span><span class="sxs-lookup"><span data-stu-id="cd258-154">**Seeing “split eye”?**</span></span>
<span data-ttu-id="cd258-155">最新のアップローダーを再インポートして、適切なレンダリング設定を取得します</span><span class="sxs-lookup"><span data-stu-id="cd258-155">Reimport the latest Uploader to get the right rendering settings</span></span>

<span data-ttu-id="cd258-156">**更新/変更は反映されませんか?**</span><span class="sxs-lookup"><span data-stu-id="cd258-156">**Updates/changes not reflected?**</span></span>
    * <span data-ttu-id="cd258-157">キットページの更新時刻を確認する</span><span class="sxs-lookup"><span data-stu-id="cd258-157">Check the updated time on the Kit page</span></span>
    * <span data-ttu-id="cd258-158">クライアントを再起動しても機能しません。</span><span class="sxs-lookup"><span data-stu-id="cd258-158">Reentering the World will not work-- restart client.</span></span> <span data-ttu-id="cd258-159">それでも、更新には数分かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="cd258-159">Even then it may take a few minutes to update</span></span>
    * <span data-ttu-id="cd258-160">フォルダー名または prefab 名にスペースがないことを確認してください。**たとえば、' party_favors ' と ' パーティを優先 ' とします**。</span><span class="sxs-lookup"><span data-stu-id="cd258-160">Make sure there are no spaces in your folder names or prefab names **for example, 'party_favors' vs 'party favors'**</span></span>

<span data-ttu-id="cd258-161">**私はスクリプトを持っていますが** 、AssetBundle ブラウザーには、場合によっては自動的にファイルが含まれます。</span><span class="sxs-lookup"><span data-stu-id="cd258-161">**It keeps saying I have a script but I don't** The AssetBundle Browser automatically includes files sometimes.</span></span> <span data-ttu-id="cd258-162">導入しているモデルを分離してみてください。</span><span class="sxs-lookup"><span data-stu-id="cd258-162">Try to isolate the model you're bringing in.</span></span> <span data-ttu-id="cd258-163">たとえば、既に別の Prefab の一部である場合は、ここでドラッグしないでください。</span><span class="sxs-lookup"><span data-stu-id="cd258-163">For example, don't drag it in when it's part of another Prefab already</span></span>

<span data-ttu-id="cd258-164">**パーティクルシステムとアニメーションについて**</span><span class="sxs-lookup"><span data-stu-id="cd258-164">**What about Particle Systems and Animations?**</span></span>
<span data-ttu-id="cd258-165">これらの場合、メッシュレンダリングと競合が無効になっている原点に位置する1x1x1 キューブの下に配置されます。</span><span class="sxs-lookup"><span data-stu-id="cd258-165">For these, next them under a 1x1x1 Cube positioned at the origin with Mesh Rendering and Collision disabled.</span></span> <span data-ttu-id="cd258-166">パーティクルシステムではループが有効になっている必要があります。また、 **調整** は、altspace で適切に拡張できるように、 **階層** に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="cd258-166">Particle Systems should have looping enabled and **Scaling** should be set to **Hierarchy** so that we can scale them in Altspace properly.</span></span> <span data-ttu-id="cd258-167">すべてのアニメーションの prefabs を生成したら、それぞれの **競合** オブジェクトの競合を無効にします。</span><span class="sxs-lookup"><span data-stu-id="cd258-167">After you generate the prefabs for all the animations, disable the collisions on the **collision** objects for each.</span></span>

<span data-ttu-id="cd258-168">**アイテムがダーク** モデルのマテリアルシェーダーを、 **モバイル/頂点点灯のみのライト** に設定しましたか。</span><span class="sxs-lookup"><span data-stu-id="cd258-168">**The Artifacts are dark** Did you set the model's material shader to **Mobile/Vertex lit-only directional lights**?</span></span>

<span data-ttu-id="cd258-169">**成果物が適切な方法で接続されていません\*\*\*\*モデル** と **collider** を回転させ、prefab を更新します。</span><span class="sxs-lookup"><span data-stu-id="cd258-169">**The Artifact isn't facing the right way** Rotate the **model** and **collider** and update the Prefab.</span></span> <span data-ttu-id="cd258-170">親を回転しても何も実行されません。これは無視されます。</span><span class="sxs-lookup"><span data-stu-id="cd258-170">Rotating the parent won't do anything--that's ignored.</span></span> <span data-ttu-id="cd258-171">この操作を簡単に行うには、[ **回転の上書き** ] フィールドを使用します。</span><span class="sxs-lookup"><span data-stu-id="cd258-171">You can use the **Rotation Override** field to do this easily.</span></span>

<span data-ttu-id="cd258-172">**これらの成果物は、SDK の **Createfromlibrary** 関数と共に使用できますか。**</span><span class="sxs-lookup"><span data-stu-id="cd258-172">**Can these Artifacts be used with the SDK's **CreateFromLibrary** function?**</span></span>
<span data-ttu-id="cd258-173">はい</span><span class="sxs-lookup"><span data-stu-id="cd258-173">Yes</span></span>