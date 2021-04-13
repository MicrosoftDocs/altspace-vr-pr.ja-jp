---
title: World 建築ツールキットの概要
description: Unity シーンテンプレートを使用して、世界ビルのツールキットを使用して、AltspaceVR ワールドをセットアップしてアップロードする方法について説明します。
ms.date: 03/11/2021
ms.topic: article
keywords: toolkit
ms.openlocfilehash: cf4660f46d93ca5c5f23de3f567ff04b12519617
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212626"
---
# <a name="introducing-the-world-building-toolkit"></a><span data-ttu-id="3d2ca-104">World 建築ツールキットの概要</span><span class="sxs-lookup"><span data-stu-id="3d2ca-104">Introducing the World Building Toolkit</span></span>

> [!NOTE]
> <span data-ttu-id="3d2ca-105">World 建築ツールキットは、当社のすばらしい友人である [Anthony Madden](https://twitter.com/chigamesstudio)によって実行されるコミュニティプロジェクトです。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-105">The World Building Toolkit is a community project run by our awesome friend, [Anthony Madden](https://twitter.com/chigamesstudio), with support from us.</span></span> <span data-ttu-id="3d2ca-106">興味をお持ちの場合は、 [公式の Altspacevr Discord](https://discordapp.com/invite/altspacevr) に参加し、#world ビルディングチャネルにアクセスしてください。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-106">If you're interested, please join the [Official AltspaceVR Discord](https://discordapp.com/invite/altspacevr) and visit the #world-building channel.</span></span> <span data-ttu-id="3d2ca-107">現在、Mac 試用版ベータ版があります。詳細については、こちらを[参照](https://altvr.com/altspacevr-mac)してください。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-107">We currently have a Mac Trial Beta right now, [more details](https://altvr.com/altspacevr-mac)</span></span>

<span data-ttu-id="3d2ca-108">アップローダーでは、Unity シーンを世界のテンプレートとして使用することができます。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-108">The Uploader allows you to use a Unity scene as a Template for your Worlds.</span></span> <span data-ttu-id="3d2ca-109">満塁を使用すると、人気のあるハロウィーンやお気に入りの作成に使用することができます。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-109">You can bring in a haunted house for Halloween or your favorite creation from Minecraft.</span></span> <span data-ttu-id="3d2ca-110">Unity にインポートできる場合は、この方法で Altspace にアクセスできる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-110">If you can import it into Unity, you can probably get it into Altspace this way.</span></span> <span data-ttu-id="3d2ca-111">いくつかの [例](https://account.altvr.com/worlds/1046572460192825569)を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-111">Here are a few [example Worlds](https://account.altvr.com/worlds/1046572460192825569).</span></span>

![ワールドの例](images/unity-uploader-img-01.png)

## <a name="setup"></a><span data-ttu-id="3d2ca-113">セットアップ</span><span class="sxs-lookup"><span data-stu-id="3d2ca-113">Setup</span></span>

1. <span data-ttu-id="3d2ca-114">公式の [Altspacevr Discord](https://discordapp.com/invite/altspacevr) に参加して、#world ビルのチャネルにアクセスしてください。友人は、友人が自分だけをビルドすることはできません。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-114">Join the [Official AltspaceVR Discord](https://discordapp.com/invite/altspacevr) and visit the #world-building channel - Friends don't let friends build Worlds alone.</span></span>
2. <span data-ttu-id="3d2ca-115">基本については、 [世界ビルのはじめにガイド](world-building-getting-started.md) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-115">Read our [World-Building Getting Started Guide](world-building-getting-started.md) for the basics</span></span>
3. <span data-ttu-id="3d2ca-116">[Unity Hub をインストール](https://blogs.unity3d.com/2018/01/24/streamline-your-workflow-introducing-unity-hub-beta) し、 **unity 2019.4.2 f1** をインストールします。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-116">[Install Unity Hub](https://blogs.unity3d.com/2018/01/24/streamline-your-workflow-introducing-unity-hub-beta) and install **Unity 2019.4.2f1**.</span></span> <span data-ttu-id="3d2ca-117">このバージョンと正確に一致しない限り、アップローダーは機能しません。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-117">The Uploader won't work unless you match this version exactly.</span></span> <span data-ttu-id="3d2ca-118">お持ちでない場合は、無料の Unity アカウントが必要です 。このアカウントをお持ちでない場合は、無料でお試しください。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-118">You'll need a free Unity account if you don't have one and choose **Personal** since you're doing this for fun!</span></span> <span data-ttu-id="3d2ca-119">インストール中に、[ **Android のビルド** ] オプションをオンにして、自動更新を無効にしてください。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-119">During the install, make sure you check the **Android Builds** option and disable auto-update.</span></span>
4. [<span data-ttu-id="3d2ca-120">最新の Unity アップローダーをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="3d2ca-120">Download the latest Unity Uploader</span></span>](https://aka.ms/AsvrCommunityUploader)
5. <span data-ttu-id="3d2ca-121">Web サイトに[テンプレートを作成](https://account.altvr.com/space_templates/new)します。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-121">[Create a Template](https://account.altvr.com/space_templates/new) on our website.</span></span> <span data-ttu-id="3d2ca-122">**Hello World テンプレート** に名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-122">Name it **Hello World Template**.</span></span>
6. <span data-ttu-id="3d2ca-123">**Hello World** という名前を [作成](https://account.altvr.com/worlds/my)します。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-123">[Create a World](https://account.altvr.com/worlds/my) and name it **Hello World**.</span></span> <span data-ttu-id="3d2ca-124">テンプレートとして [ **Hello World テンプレート** ] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-124">Select **Hello World Template** as the Template.</span></span>

![作成されたワールド画面](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a><span data-ttu-id="3d2ca-126">シーンをアップロードする</span><span class="sxs-lookup"><span data-stu-id="3d2ca-126">Upload your scene</span></span>

> [!VIDEO https://channel9.msdn.com/Shows/Docs-Mixed-Reality/How-to-upload-a-Template/player]

1. <span data-ttu-id="3d2ca-127">Unity Hub を開き、新しい Unity 2019.4.2 f1 プロジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-127">Open Unity Hub and create a new Unity 2019.4.2f1 project.</span></span>
2. <span data-ttu-id="3d2ca-128">プロジェクトを開いた状態で、ダウンロードしたファイル (Unity パッケージ) をダブルクリックしてアップローダーをインポートします。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-128">With your project open, import the Uploader by double-clicking the file you downloaded (it's a Unity package).</span></span> <span data-ttu-id="3d2ca-129">これで、 **altと** いう新しいタブが表示されます。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-129">You should now see a new tab called **AltspaceVR**.</span></span> <span data-ttu-id="3d2ca-130">Altspace で使用するすべての Unity プロジェクトのパッケージをインポートする必要があります。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-130">You'll need to import the package for every Unity project you want to use with Altspace</span></span>
3. <span data-ttu-id="3d2ca-131">**メニュー > alt> ビルド設定** を開く</span><span class="sxs-lookup"><span data-stu-id="3d2ca-131">Open **Menu > AltspaceVR > Build Settings**</span></span>
4. <span data-ttu-id="3d2ca-132">Altspace アカウントの資格情報でサインインします</span><span class="sxs-lookup"><span data-stu-id="3d2ca-132">Sign in with your Altspace account credentials</span></span>
5. <span data-ttu-id="3d2ca-133">[**テンプレートの読み込み**] を選択し、[ **Hello World テンプレート**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-133">Select **Load Templates** and then select **Hello World Template**</span></span>
6. <span data-ttu-id="3d2ca-134">シーンにキューブを追加して保存します。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-134">Add a cube to your scene and save.</span></span>
7. <span data-ttu-id="3d2ca-135">**Windows のビルド** を確認し、 **Android の場合は [ビルド]** をオフにしますか?</span><span class="sxs-lookup"><span data-stu-id="3d2ca-135">Check **Build for Windows?** and uncheck **Build for Android?**</span></span>
8. <span data-ttu-id="3d2ca-136">**[アップロード]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-136">Select **Upload**.</span></span> <span data-ttu-id="3d2ca-137">約1分で [ **アップロード** が完了しました] と表示されます。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-137">In about a minute, you should see **Upload** complete.</span></span>
9. <span data-ttu-id="3d2ca-138">Altspace を起動して **メニュー > ワールド >** を入力して **Hello World** 参加する</span><span class="sxs-lookup"><span data-stu-id="3d2ca-138">Join **Hello World** by launching Altspace and entering from **Menu > Worlds > My Worlds**</span></span>
10. <span data-ttu-id="3d2ca-139">**メニュー > 設定 > 中程度の設定** にリセットして領域をリセット ></span><span class="sxs-lookup"><span data-stu-id="3d2ca-139">Reset the World from **Menu > Settings > Moderate > Reset Space**</span></span>
11. <span data-ttu-id="3d2ca-140">キューブが表示されます。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-140">You should see the cube.</span></span> <span data-ttu-id="3d2ca-141">上記のビデオのようにすばやく実行すると、10秒ほどではなく変更を確認できます。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-141">If you do it fast like in the video above, you can see changes within as little as 10 seconds.</span></span>

## <a name="whats-supported"></a><span data-ttu-id="3d2ca-142">サポートされる操作</span><span class="sxs-lookup"><span data-stu-id="3d2ca-142">What's supported</span></span>

* <span data-ttu-id="3d2ca-143">はい: モデル、競合、アニメーション、パーティクル効果、オーディオ、skyboxes など</span><span class="sxs-lookup"><span data-stu-id="3d2ca-143">Yes: models, collision, animations, particle effects, audio, skyboxes, and so on</span></span>
* <span data-ttu-id="3d2ca-144">いいえ: スクリプト。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-144">No: scripts.</span></span> <span data-ttu-id="3d2ca-145">セキュリティ上の理由から、スクリプトを含むアップロードは拒否されます</span><span class="sxs-lookup"><span data-stu-id="3d2ca-145">For security purposes, uploads containing scripts will be rejected</span></span>
* <span data-ttu-id="3d2ca-146">場合によっては、動的なグローバル照明のような凝った</span><span class="sxs-lookup"><span data-stu-id="3d2ca-146">Maybe: fancy stuff like dynamic global illumination</span></span>
* <span data-ttu-id="3d2ca-147">異なるプラットフォームのシーンを個別またはまとめてアップロードする</span><span class="sxs-lookup"><span data-stu-id="3d2ca-147">Upload scenes for different platforms separately or together</span></span>
* <span data-ttu-id="3d2ca-148">アップローダーを使用して構築された、 [おすすめの世界](https://account.altvr.com/worlds/featured)をご覧ください</span><span class="sxs-lookup"><span data-stu-id="3d2ca-148">See [Featured Worlds](https://account.altvr.com/worlds/featured), many were built using the Uploader</span></span>

## <a name="tips"></a><span data-ttu-id="3d2ca-149">ヒント</span><span class="sxs-lookup"><span data-stu-id="3d2ca-149">Tips</span></span>

* <span data-ttu-id="3d2ca-150">公式の [Altspacevr Discord](https://discordapp.com/invite/altspacevr)に参加します。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-150">Join the [Official AltspaceVR Discord](https://discordapp.com/invite/altspacevr).</span></span>
* <span data-ttu-id="3d2ca-151">左側の [テンプレート] ページに、プラットフォーム別の最新のアップロードが表示されます。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-151">On the Template page on the left side, we show you the latest uploads by platform.</span></span> <span data-ttu-id="3d2ca-152">成功した場合は、 **1-2 分前** に表示されます。Screen_Shot_2019-01-11 _at_1.21.04_AM.png</span><span class="sxs-lookup"><span data-stu-id="3d2ca-152">If it was successful, you'd see **1-2 mins ago**.Screen_Shot_2019-01-11 _at_1.21.04_AM.png</span></span>

![アップロードが強調表示された状態で開く [テンプレート] パネル](images/unity-uploader-img-03.png)

* <span data-ttu-id="3d2ca-154">を更新するときに、その中でも使用できます。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-154">You can be in-World when you update.</span></span> <span data-ttu-id="3d2ca-155">アップローダーが " **アップロード完了** " と表示されたら、世界をリセットして変更内容を確認できます。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-155">The moment the Uploader says **Upload Complete** you can reset the World to see the changes.</span></span>
* <span data-ttu-id="3d2ca-156">簡単なシーンを使用した PC 用のビルドでは、Altspace の変化を確認するために1分未満でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-156">Building for PC-only with a simple scene should take less than 1 minute to see a change in Altspace</span></span>
* <span data-ttu-id="3d2ca-157">取られるを避けるために、世界をプライベートに設定し、一覧から削除します。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-157">Set your World to be Private and Unlisted to avoid distractions.</span></span>
* <span data-ttu-id="3d2ca-158">既定でユーザーが生成する場所を確認できるように、キューブを配信元に配置します。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-158">Place a cube at the origin so you can see where people will spawn by default.</span></span> <span data-ttu-id="3d2ca-159">アップロード時にキューブを非表示にします。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-159">Hide the cube when uploading.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="3d2ca-160">トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="3d2ca-160">Troubleshooting</span></span>

<span data-ttu-id="3d2ca-161">**何かを挿入することはできません。** オブジェクトへの競合を追加して、それらにテレポートする必要があります。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-161">**I'm falling or can't teleport onto anything** You need to add collision to objects to teleport onto them.</span></span>

<span data-ttu-id="3d2ca-162">**何も変更されません**</span><span class="sxs-lookup"><span data-stu-id="3d2ca-162">**Nothing changed**</span></span>
    * <span data-ttu-id="3d2ca-163">Unity にシーンを保存しましたか?</span><span class="sxs-lookup"><span data-stu-id="3d2ca-163">Did you save the scene in Unity?</span></span>
    * <span data-ttu-id="3d2ca-164">テスト対象のプラットフォームを選択しましたか?</span><span class="sxs-lookup"><span data-stu-id="3d2ca-164">Did you choose the platform you're testing on?</span></span>
    * <span data-ttu-id="3d2ca-165">お持ちの方は、</span><span class="sxs-lookup"><span data-stu-id="3d2ca-165">Are you in the right World?</span></span> <span data-ttu-id="3d2ca-166">アップローダーと World 形式で適切なテンプレートを選択しましたか?</span><span class="sxs-lookup"><span data-stu-id="3d2ca-166">Did you choose the right Template in the Uploader AND in the World form?</span></span>
    * <span data-ttu-id="3d2ca-167">テンプレートページの統計情報を確認しましたか?</span><span class="sxs-lookup"><span data-stu-id="3d2ca-167">Did you check the Template page stats?</span></span>

<span data-ttu-id="3d2ca-168">**アップロードが失敗またはタイムアウトする**</span><span class="sxs-lookup"><span data-stu-id="3d2ca-168">**Upload fails or times out**</span></span>
    * <span data-ttu-id="3d2ca-169">最も一般的なアップロードエラーの Unity バージョンが間違っています。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-169">Most common upload error is having the wrong Unity version.</span></span> <span data-ttu-id="3d2ca-170">必要なバージョンと正確に一致している必要があります。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-170">It must match the required version exactly.</span></span>
    * <span data-ttu-id="3d2ca-171">アップロードが大きすぎる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-171">Your upload might be too large.</span></span> <span data-ttu-id="3d2ca-172">PC のシーン < 100 MB に保つようにしてください。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-172">Try to keep PC scenes < 100 MB.</span></span> <span data-ttu-id="3d2ca-173">小規模に開始し、構築します。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-173">Start small and build up.</span></span> <span data-ttu-id="3d2ca-174">Optimize、optimize、optimize。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-174">Optimize, optimize, optimize.</span></span>
    * <span data-ttu-id="3d2ca-175">単純なキューブを使用して、新しいプロジェクトを試してください。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-175">Try with a fresh project with a simple cube.</span></span>
    * <span data-ttu-id="3d2ca-176">ビルド中に強制的に終了しないでください。シーンを破損させることができます。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-176">Don't force quit during a build--it can corrupt your scene.</span></span> <span data-ttu-id="3d2ca-177">再アップロードをお試しください。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-177">Try reuploading.</span></span>

<span data-ttu-id="3d2ca-178">**処理速度が遅い**</span><span class="sxs-lookup"><span data-stu-id="3d2ca-178">**It's a slow process**</span></span>
    * <span data-ttu-id="3d2ca-179">後で Android を反復処理する場合にのみ、PC 用にビルドすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-179">We recommend building for PC only while iterating and for Android later.</span></span>
    * <span data-ttu-id="3d2ca-180">未使用のファイルを削除してみてください。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-180">Try removing unused files.</span></span> <span data-ttu-id="3d2ca-181">何らかの理由により、Unity は熱心になることがあります。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-181">For whatever reason Unity gets overzealous sometimes.</span></span>

<span data-ttu-id="3d2ca-182">**Altspace 資格情報でサインインできません**</span><span class="sxs-lookup"><span data-stu-id="3d2ca-182">**I can't sign in with my Altspace credentials**</span></span>
    * <span data-ttu-id="3d2ca-183">電子メールでは大文字と小文字が区別されます。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-183">Emails are case-sensitive.</span></span>
    * <span data-ttu-id="3d2ca-184">新しいプロジェクトを試してみてください。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-184">Try with a new project.</span></span>
    * <span data-ttu-id="3d2ca-185">Altspace アカウントが良好な場所にあることを確認します。</span><span class="sxs-lookup"><span data-stu-id="3d2ca-185">Make sure your Altspace account is in good standing.</span></span>

## <a name="see-also"></a><span data-ttu-id="3d2ca-186">こちらもご覧ください</span><span class="sxs-lookup"><span data-stu-id="3d2ca-186">See also</span></span>

* [<span data-ttu-id="3d2ca-187">Unity の学習</span><span class="sxs-lookup"><span data-stu-id="3d2ca-187">Unity Learn</span></span>](https://unity3d.com/learn)
* [<span data-ttu-id="3d2ca-188">Unity フォーラム</span><span class="sxs-lookup"><span data-stu-id="3d2ca-188">Unity Forums</span></span>](https://forum.unity.com)
