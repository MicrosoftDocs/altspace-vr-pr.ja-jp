---
title: マルチメディアコンソールの使用
description: 職場でのマルチメディアコンソールの構成、発行、および管理を開始する方法について説明します。
ms.date: 03/11/2021
ms.topic: article
keywords: コンソール、マルチメディア
ms.openlocfilehash: 601328eb6f266dbcfc9d81fc4f1c2d09ac62b318
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212839"
---
# <a name="using-the-multimedia-console"></a><span data-ttu-id="bffae-104">マルチメディアコンソールの使用</span><span class="sxs-lookup"><span data-stu-id="bffae-104">Using the multimedia console</span></span>

<span data-ttu-id="bffae-105">マルチメディアコンソールは、イベントや世界でメディアの共有を可能にするツールです。</span><span class="sxs-lookup"><span data-stu-id="bffae-105">The Multimedia Console is a tool that enables media sharing in events and worlds.</span></span> <span data-ttu-id="bffae-106">この機能を使用して、イメージ、プレゼンテーションスライド、livestreams、ビデオ、再生リストなどの項目を共有できます。</span><span class="sxs-lookup"><span data-stu-id="bffae-106">You can use it to share things like images, presentation slides, livestreams, videos, playlists, and more.</span></span> <span data-ttu-id="bffae-107">マルチメディアコンソール **v 0.5.0 +** を使用する手順を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bffae-107">Below is a step-by-step instruction on how to use the Multimedia Console **v0.5.0+**.</span></span> 

## <a name="getting-started"></a><span data-ttu-id="bffae-108">作業の開始</span><span class="sxs-lookup"><span data-stu-id="bffae-108">Getting started</span></span>

<span data-ttu-id="bffae-109">マルチメディアコンソールの概要は、2つの部分で構成されています。</span><span class="sxs-lookup"><span data-stu-id="bffae-109">Getting started with the Multimedia Console is a two part process.</span></span>  <span data-ttu-id="bffae-110">まず、環境に配置するマルチメディアコンソールセッションの構成を生成して公開するために使用する web ポータルがあります。</span><span class="sxs-lookup"><span data-stu-id="bffae-110">First there's the web portal that you'll use to generate and publish a configuration for the Multimedia Console session you place in your environment.</span></span>  <span data-ttu-id="bffae-111">2つ目は、実際の環境における実際のマルチメディアコンソールアプリの配置と、使用する構成コードの設定です。</span><span class="sxs-lookup"><span data-stu-id="bffae-111">Second is the placement of the actual Multimedia Console app in your environment and setting the configuration code it should use.</span></span>

### <a name="configuring-the-multimedia-console-with-the-web-portal"></a><span data-ttu-id="bffae-112">Web ポータルを使用したマルチメディアコンソールの構成</span><span class="sxs-lookup"><span data-stu-id="bffae-112">Configuring the Multimedia console with the web portal</span></span>

1. <span data-ttu-id="bffae-113">まず、URL が必要になるので、コンテンツがオンラインでホストされていることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bffae-113">First, you'll need to make sure your content is hosted online because you'll need a URL.</span></span> <span data-ttu-id="bffae-114">(写真を altvr.com にアップロードしたり、ビデオ. mp4 ファイルをオンラインでホストしたり、Twitch ライブストリームリンクを使用したりすることができます。 https://www.twitch.tv/ninja)</span><span class="sxs-lookup"><span data-stu-id="bffae-114">(You can upload photos to altvr.com, host a video .mp4 file online or use Twitch live stream link: https://www.twitch.tv/ninja)</span></span> 
2. <span data-ttu-id="bffae-115">でマルチメディアコンソールの web ポータルに移動します。 [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)</span><span class="sxs-lookup"><span data-stu-id="bffae-115">Navigate to the web portal for the Multimedia Console at [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)</span></span>
3. <span data-ttu-id="bffae-116">Web ポータルから、マルチメディアコンソールの構成を生成して公開することができます。</span><span class="sxs-lookup"><span data-stu-id="bffae-116">From the web portal, you can generate and publish a configuration for the Multimedia Console.</span></span>  <span data-ttu-id="bffae-117">(さまざまなプロパティの詳細については、以下を参照してください)。</span><span class="sxs-lookup"><span data-stu-id="bffae-117">(See below for details about the various properties).</span></span>
4. <span data-ttu-id="bffae-118">メディアの一覧にメディアを入力し、全般設定を構成したら、アプリの右上にある [発行] ボタンを選択します。</span><span class="sxs-lookup"><span data-stu-id="bffae-118">Once you've entered the media into the media list and have configured the general settings, select the publish button in the top-right part of the app.</span></span>
5. <span data-ttu-id="bffae-119">発行が完了すると、ダイアログが表示され、配置したマルチメディアコンソールに入力する2つの単語のコードが表示されます。</span><span class="sxs-lookup"><span data-stu-id="bffae-119">Once the publish has completed, a dialog will pop up with a two word code for you to enter in to the Multimedia Console you placed.</span></span>
  
### <a name="placing-the-multimedia-console-in-your-environment"></a><span data-ttu-id="bffae-120">環境にマルチメディアコンソールを配置する</span><span class="sxs-lookup"><span data-stu-id="bffae-120">Placing the Multimedia console in your environment</span></span>

1. <span data-ttu-id="bffae-121">[ **ワールドエディター] > エディターパネル > [SDK アプリ > マルチメディアコンソール**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="bffae-121">Select on **World Editor > Editor Panel > SDK Apps > Multimedia Console**.</span></span> <span data-ttu-id="bffae-122">(登録されていないアプリの場合は、[ **> の基本] > [SDK アプリ**] を参照してください)。</span><span class="sxs-lookup"><span data-stu-id="bffae-122">(Don't go to **World Editor > Basics > SDK App**--that's for unregistered apps.)</span></span>  
2. <span data-ttu-id="bffae-123">スペースと対象ユーザーに最適なマルチメディアコンソールを配置します。</span><span class="sxs-lookup"><span data-stu-id="bffae-123">Position the Multimedia Console to best suite your space and audience.</span></span>
3. <span data-ttu-id="bffae-124">編集モードを終了するには、オレンジ色の編集モードボタンをクリックします。</span><span class="sxs-lookup"><span data-stu-id="bffae-124">Get out of Edit Mode by clicking the orange Edit Mode button.</span></span>
4. <span data-ttu-id="bffae-125">**Media player の所有者であるかどうか** を確認するメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="bffae-125">You'll be prompted **Are you the media player owner?**</span></span> <span data-ttu-id="bffae-126">このマルチメディアコンソールセッションの正式な所有者になるユーザーの方は、確認してから続行してください。</span><span class="sxs-lookup"><span data-stu-id="bffae-126">If you're the person who should be the official owner of this Multimedia Console session, confirm and continue.</span></span> <span data-ttu-id="bffae-127">(他の与えロールも利用できます。</span><span class="sxs-lookup"><span data-stu-id="bffae-127">(Other permissioned roles are available as well.</span></span> <span data-ttu-id="bffae-128">詳細な一覧については、以下を参照してください。)</span><span class="sxs-lookup"><span data-stu-id="bffae-128">See below for a detailed list.)</span></span>
5. <span data-ttu-id="bffae-129">[はい] を選択して、プライマリホストであることを確認します。</span><span class="sxs-lookup"><span data-stu-id="bffae-129">Select Yes to confirm that you are the primary host.</span></span>  
6. <span data-ttu-id="bffae-130">ダイアログがポップアップ表示され、web ポータルまたは有効な JSON からコードを入力するように求められます。</span><span class="sxs-lookup"><span data-stu-id="bffae-130">A dialog should pop up that asks you to enter a code from the web portal or valid JSON.</span></span>  <span data-ttu-id="bffae-131">ダッシュを含む2つの単語コードを web ポータルから入力し、[OK] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="bffae-131">Enter the two word code from the web portal including the dash and hit OK.</span></span> <span data-ttu-id="bffae-132">(JSON は、以下で説明する高度な構成です)</span><span class="sxs-lookup"><span data-stu-id="bffae-132">(JSON is an advanced configuration described below)</span></span>
7. <span data-ttu-id="bffae-133">マルチメディアコンソールは、web ポータルで作成した構成で数秒後にロードされます。</span><span class="sxs-lookup"><span data-stu-id="bffae-133">The Multimedia Console should load after a few seconds with the configuration you built in the web portal.</span></span>

### <a name="controlling-the-multimedia-console"></a><span data-ttu-id="bffae-134">マルチメディアコンソールの制御</span><span class="sxs-lookup"><span data-stu-id="bffae-134">Controlling the Multimedia console</span></span>

1. <span data-ttu-id="bffae-135">コードを入力して構成プロセスを完了すると、メディアディスプレイの下にコントロールボタンが表示されます。</span><span class="sxs-lookup"><span data-stu-id="bffae-135">After you input your code and complete the configuration process, you'll see control buttons appear below a media display.</span></span> 
    * <span data-ttu-id="bffae-136">**Play** はメディアビューアーを開始します (以前に停止した場合は、現在のエントリで再起動します)</span><span class="sxs-lookup"><span data-stu-id="bffae-136">**Play** starts the media viewer (or restarts at current entry, if previously stopped)</span></span> 
    * <span data-ttu-id="bffae-137">[**停止**] を行うと、メディアビューアーが停止し、現在のメディアは非表示になります。</span><span class="sxs-lookup"><span data-stu-id="bffae-137">**Stop** stops the media viewer, and hides current media.</span></span>  
    * <span data-ttu-id="bffae-138">**次** または前のメディアにスキップ</span><span class="sxs-lookup"><span data-stu-id="bffae-138">**Next/Prev** skips to next or previous media</span></span> 
    * <span data-ttu-id="bffae-139">**x/x**  メディア一覧の現在のインデックスを表示し、一覧内の任意のポイントに移動できるようにします。</span><span class="sxs-lookup"><span data-stu-id="bffae-139">**x/x** shows the current index into the media list, and allows you to jump to any point in the list</span></span>
    * <span data-ttu-id="bffae-140">**構成** を使用すると、web ポータルから新しいコードを再利用して、コンソールで新しい構成を設定できます。</span><span class="sxs-lookup"><span data-stu-id="bffae-140">**Config** allows reentering a new code from the web portal to set a new configuration in the console.</span></span> 

<span data-ttu-id="bffae-141">これで、マルチメディアコンソールを使用して共有を開始するように設定されました。</span><span class="sxs-lookup"><span data-stu-id="bffae-141">Now you're set to begin sharing via the Multimedia Console!</span></span>  
 
## <a name="working-with-the-web-portal"></a><span data-ttu-id="bffae-142">Web ポータルでの作業</span><span class="sxs-lookup"><span data-stu-id="bffae-142">Working with the web portal</span></span>

<span data-ttu-id="bffae-143">Web ポータルは、マルチメディアコンソールのさまざまな機能を構成できる web アプリです。</span><span class="sxs-lookup"><span data-stu-id="bffae-143">The web portal is a web app that enables configuring the various features of the Multimedia Console.</span></span>  <span data-ttu-id="bffae-144">これらの機能は2つのカテゴリに分類されます。一般的なメディアコンソール設定とメディア再生リスト。</span><span class="sxs-lookup"><span data-stu-id="bffae-144">These features fall in to two categories; general media console settings, and the media play list.</span></span>

### <a name="multimedia-console-general-settings"></a><span data-ttu-id="bffae-145">マルチメディアコンソールの全般設定</span><span class="sxs-lookup"><span data-stu-id="bffae-145">Multimedia console general settings</span></span>

<span data-ttu-id="bffae-146">**再生設定**</span><span class="sxs-lookup"><span data-stu-id="bffae-146">**Playback Settings**</span></span>

<span data-ttu-id="bffae-147">メディア一覧の全般的な再生設定</span><span class="sxs-lookup"><span data-stu-id="bffae-147">General playback settings for the media list</span></span>

* <span data-ttu-id="bffae-148">[**メディア一覧のループ]**-一覧の末尾に達すると、メディアリストをループするかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="bffae-148">**Loop Media List**- Determines whether the media list should loop around once you reach the end of the list.</span></span>
* <span data-ttu-id="bffae-149">**Start メソッド** -マルチメディアコンソールを起動する方法を選択します。</span><span class="sxs-lookup"><span data-stu-id="bffae-149">**Start Method** - Selects the method by which the multimedia console should start.</span></span>
    * <span data-ttu-id="bffae-150">Manual-メディアを開始する前に [再生] ボタンが押されるのを待ちます。</span><span class="sxs-lookup"><span data-stu-id="bffae-150">Manual - Waits for the play button to be pressed before starting the media</span></span>
    * <span data-ttu-id="bffae-151">[開始から自動開始]-一覧の先頭からメディアリストを自動的に開始します</span><span class="sxs-lookup"><span data-stu-id="bffae-151">Auto Start from Beginning - Auto start the media list from the beginning of the list</span></span>
    * <span data-ttu-id="bffae-152">自動開始ランダム-リスト内のランダムな開始位置からメディアを自動で開始します。</span><span class="sxs-lookup"><span data-stu-id="bffae-152">Auto Start Random - Auto starts the media from a random starting point in the list</span></span>

<span data-ttu-id="bffae-153">**ロール**</span><span class="sxs-lookup"><span data-stu-id="bffae-153">**Roles**</span></span>

<span data-ttu-id="bffae-154">マルチメディアコンソールを制御および構成するためのロールの割り当て。</span><span class="sxs-lookup"><span data-stu-id="bffae-154">Role assignments for controlling and configuring the Multimedia Console.</span></span>    <span data-ttu-id="bffae-155">これらのロールは、次のセットに分類されます。</span><span class="sxs-lookup"><span data-stu-id="bffae-155">These roles are broken down in to the following set:</span></span>

* <span data-ttu-id="bffae-156">**所有者のみ** -マルチメディアコンソールセッションの所有者であるユーザー</span><span class="sxs-lookup"><span data-stu-id="bffae-156">**Owner Only** - The user that is the owner of the Multimedia Console Session</span></span>
* <span data-ttu-id="bffae-157">**管理者特権** を持つユーザー-最初にマルチメディアコンソールが構成されている領域に、モデレーター、ホスト、またはプレゼンターの役割を持つユーザー</span><span class="sxs-lookup"><span data-stu-id="bffae-157">**Elevated Users** - Users that have moderator, host, or presenter roles in the space that the Multimedia Console is configured in originally</span></span>
* <span data-ttu-id="bffae-158">**すべてのユーザー** -すべてのユーザー</span><span class="sxs-lookup"><span data-stu-id="bffae-158">**All Users** - All users</span></span>

<span data-ttu-id="bffae-159">これらのロールは、この一覧で選択されたロールの上にあるすべてのロールにも、その機能を使用するためのアクセス許可が付与されるという意味でスタックします。</span><span class="sxs-lookup"><span data-stu-id="bffae-159">These roles stack in the sense that all roles above the one chosen in this list will also be granted permission to use that feature.</span></span>  <span data-ttu-id="bffae-160">例: **管理者特権** を持つユーザーには、メンバーがモデレーター、ホスト、または講師 \* \* でない場合でも、この **所有者** が含まれます。</span><span class="sxs-lookup"><span data-stu-id="bffae-160">Example: **Elevated Users** includes the **Owner** even if they aren't a moderator, host, or presenter\*\* in AltspaceVR.</span></span> <span data-ttu-id="bffae-161">ロールの割り当てによって制御される機能を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bffae-161">Features that are controlled by role assignments are as follows</span></span>

* <span data-ttu-id="bffae-162">**メディアプレーヤーを制御できる** -マルチメディアコンソールのメディア再生ボタンを制御できるロールを決定します。</span><span class="sxs-lookup"><span data-stu-id="bffae-162">**Can control media player** - Determines what roles can control the media playback buttons for the Multimedia Console</span></span>
* <span data-ttu-id="bffae-163">**メディアプレーヤーを構成できる** **-[構成] ボタン** へのアクセスが許可されている場合に、マルチメディアコンソールを構成できるロールを決定します。</span><span class="sxs-lookup"><span data-stu-id="bffae-163">**Can configure the media player** - Determines what roles can configure the Multimedia Console by being granted access to the **Config** button</span></span>

### <a name="adding-photos-and-videos-to-the-media-list"></a><span data-ttu-id="bffae-164">メディアリストへの写真とビデオの追加</span><span class="sxs-lookup"><span data-stu-id="bffae-164">Adding photos and videos to the media list</span></span>

<span data-ttu-id="bffae-165">メディアは、マルチメディアコンソールの中核です。</span><span class="sxs-lookup"><span data-stu-id="bffae-165">Media is the heart of the Multimedia Console.</span></span>  <span data-ttu-id="bffae-166">イメージとビデオリンクは、マルチメディアコンソール内でメディアの種類としてサポートされています。</span><span class="sxs-lookup"><span data-stu-id="bffae-166">Images and video links are supported as media types within the Multimedia Console.</span></span>  <span data-ttu-id="bffae-167">新しいメディアを追加するには、[ **イメージの追加** ] または [ビデオアイコンの **追加** ] を選択して、メディア情報と設定を入力するためのダイアログをポップアップ表示します。</span><span class="sxs-lookup"><span data-stu-id="bffae-167">To add new media, select either the **Add Image** or **Add Video** icons to have a dialog pop up to enter the media information and settings.</span></span>  <span data-ttu-id="bffae-168">メディアの種類と関連する設定の内訳を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bffae-168">Below is the breakdown of the media types and associated settings</span></span>

<span data-ttu-id="bffae-169">**イメージ**</span><span class="sxs-lookup"><span data-stu-id="bffae-169">**Image**</span></span>

<span data-ttu-id="bffae-170">画像は、jpeg、png、son などの標準のイメージの種類である必要があります。</span><span class="sxs-lookup"><span data-stu-id="bffae-170">Images should be a standard image type such as jpeg, png, and son on.</span></span> <span data-ttu-id="bffae-171">パブリックリンクを使用して、どこかにホストする必要があります。</span><span class="sxs-lookup"><span data-stu-id="bffae-171">They need to be hosted somewhere with a public link.</span></span>

* <span data-ttu-id="bffae-172">**Name** -(必須) イメージを識別する名前。</span><span class="sxs-lookup"><span data-stu-id="bffae-172">**Name** - (Required) Name that you wish to identify the image with.</span></span>
* <span data-ttu-id="bffae-173">**イメージの url** -(必須) イメージのパブリック URL</span><span class="sxs-lookup"><span data-stu-id="bffae-173">**Image URL** - (Required) The public url of the image</span></span>
* <span data-ttu-id="bffae-174">[**後にスキップ** する-イメージがスキップされるまでの秒数</span><span class="sxs-lookup"><span data-stu-id="bffae-174">**Skip After** - The number of seconds that the image should be skipped after</span></span>

<span data-ttu-id="bffae-175">**ビデオ**</span><span class="sxs-lookup"><span data-stu-id="bffae-175">**Video**</span></span>

<span data-ttu-id="bffae-176">ビデオは、Twitch と DLive を使用してビデオやライブストリームにすることができます。</span><span class="sxs-lookup"><span data-stu-id="bffae-176">Videos can be hosted videos or live streams through Twitch and DLive.</span></span>  <span data-ttu-id="bffae-177">(他のサポートが適切なストリーム url を取得するために余分な作業で機能する場合がありますが、マルチメディアコンソール内で完全にはサポートされていません)</span><span class="sxs-lookup"><span data-stu-id="bffae-177">(Other support may function with extra work to get the proper stream url, but aren't fully supported within the Multimedia Console)</span></span>

* <span data-ttu-id="bffae-178">**名前** -(必須) ビデオを識別する名前。</span><span class="sxs-lookup"><span data-stu-id="bffae-178">**Name** - (Required) Name that you wish to identify the video with.</span></span>
* <span data-ttu-id="bffae-179">**ビデオ url** -(必須) ビデオがホストされている、またはライブストリームが提供されるパブリック URL。</span><span class="sxs-lookup"><span data-stu-id="bffae-179">**Video URL** - (Required) The public url that the video is hosted at or the live stream is served from.</span></span>
* <span data-ttu-id="bffae-180">**スキップ後** -ビデオがスキップされるまでの秒数</span><span class="sxs-lookup"><span data-stu-id="bffae-180">**Skip After** - The number of seconds that the video should be skipped after</span></span>
* <span data-ttu-id="bffae-181">**Volume** -0 (最小)-1 (max) の値からのビデオのボリューム。</span><span class="sxs-lookup"><span data-stu-id="bffae-181">**Volume** - The volume of the video from 0 (min) - 1 (max) values.</span></span>
* <span data-ttu-id="bffae-182">**開始時刻** -ビデオの開始から開始するまでの秒数。</span><span class="sxs-lookup"><span data-stu-id="bffae-182">**Start Time** - The number of seconds from the beginning of the video start from.</span></span>
* <span data-ttu-id="bffae-183">[**開始距離のロールオフ**-マルチメディアコンソールから移動したときにボリュームがオフになる世界のメーターの距離。</span><span class="sxs-lookup"><span data-stu-id="bffae-183">**Roll Off Start Distance** - The distance in meters in world that the volume begins to fall off at as you move away from the Multimedia Console</span></span>
* <span data-ttu-id="bffae-184">**ビデオの終了操作** -ビデオの終わりに達したときに実行するアクション。</span><span class="sxs-lookup"><span data-stu-id="bffae-184">**End of Video Action** - The action to take once the end of the video is reached.</span></span>
    * <span data-ttu-id="bffae-185">[停止]-ビデオが終了した後、メディアの一覧が停止します。</span><span class="sxs-lookup"><span data-stu-id="bffae-185">Stop - The media list stops after the video has ended</span></span>
    * <span data-ttu-id="bffae-186">Loop-ビデオは手動でスキップされるまでループします。</span><span class="sxs-lookup"><span data-stu-id="bffae-186">Loop - The video will loop until manually skipped</span></span>
    * <span data-ttu-id="bffae-187">[次に再生]-現在のビデオが終了した後に、メディアリスト内の次のメディアが開始されます。</span><span class="sxs-lookup"><span data-stu-id="bffae-187">Play Next - The next media in the media list will be started after the current video ends.</span></span>

## <a name="working-with-json-directly-advancedoptional"></a><span data-ttu-id="bffae-188">JSON を直接操作する (詳細設定/省略可能)</span><span class="sxs-lookup"><span data-stu-id="bffae-188">Working with JSON directly (advanced/optional)</span></span>

<span data-ttu-id="bffae-189">マルチメディアコンソールでは、Altthe Console のプロンプトに直接、JSON を入力できます。</span><span class="sxs-lookup"><span data-stu-id="bffae-189">The Multimedia Console supports entering JSON directly in to the prompt of the console in AltspaceVR.</span></span>  <span data-ttu-id="bffae-190">JSON は、media player の構成を有効にするための内部メカニズムです。</span><span class="sxs-lookup"><span data-stu-id="bffae-190">JSON is the internal mechanism with which we enable media player configurations.</span></span> <span data-ttu-id="bffae-191">JSON を直接設定する機能を公開することは、より高度なユーザーが独自のワークフローを構築して、そのニーズを満たすと共に JSON を理解できるようにするものです。</span><span class="sxs-lookup"><span data-stu-id="bffae-191">Exposing the ability to set JSON directly is something that allows for more advanced users to build their own workflows that suites their needs and familiarity with JSON.</span></span>  <span data-ttu-id="bffae-192">Json の構造と JSON の検証に使用されるスキーマについての簡単な説明を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bffae-192">The following is a brief description of the JSON structure and the schema by which the JSON is validated.</span></span> <span data-ttu-id="bffae-193">以下のプロパティの詳細については、マルチメディアコンソールの構成について説明している上記のセクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="bffae-193">For more detailed descriptions of the properties below, see the above sections that talk about configuring the Multimedia Console.</span></span>  <span data-ttu-id="bffae-194">このセクションでは、主に、JSON データのスキーマの例と構造に焦点を絞って説明します。</span><span class="sxs-lookup"><span data-stu-id="bffae-194">This section is focused primarily on the schema examples and structuring for the JSON data.</span></span>

### <a name="global-media-settings"></a><span data-ttu-id="bffae-195">グローバルメディアの設定</span><span class="sxs-lookup"><span data-stu-id="bffae-195">Global media settings</span></span>

```json
{
  "loopMediaList": true | false
  "startMethod": "manual" | "autostart-beginning" | "autostart-random"
  "controlMediaPlayer": "everyone" | "elevated" | "owner"
  "configureMediaPlayer": "elevated" | "owner"
  ...
}
```

### <a name="media-list"></a><span data-ttu-id="bffae-196">メディア一覧</span><span class="sxs-lookup"><span data-stu-id="bffae-196">Media list</span></span>

<span data-ttu-id="bffae-197">メディアの一覧は、ロールや再生の設定など、JSON 構造のルートで設定されたプロパティです。</span><span class="sxs-lookup"><span data-stu-id="bffae-197">The media list is a property set at the root of the JSON structure like the Roles and Playback Settings.</span></span>  <span data-ttu-id="bffae-198">これは、次のいずれかのメディア構成構造を含むことができる単純な配列です。</span><span class="sxs-lookup"><span data-stu-id="bffae-198">It's a simple array that can contain one of the following media configuration structures.</span></span> <span data-ttu-id="bffae-199">(それぞれの機能の詳細については、上記のプロパティの説明を参照してください)。</span><span class="sxs-lookup"><span data-stu-id="bffae-199">(See property descriptions above for details on what each does.)</span></span>

<span data-ttu-id="bffae-200">**画像の例**</span><span class="sxs-lookup"><span data-stu-id="bffae-200">**Image example**</span></span>

<span data-ttu-id="bffae-201">*必須フィールド: "name" および "imageUrl"*</span><span class="sxs-lookup"><span data-stu-id="bffae-201">*Required fields: "name" and "imageUrl"*</span></span>

```json
{
    "name": "Altspace Screenshot",
    "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
    "skipAfter": 10
}
```

<span data-ttu-id="bffae-202">**ビデオの例**</span><span class="sxs-lookup"><span data-stu-id="bffae-202">**Video example**</span></span>

<span data-ttu-id="bffae-203">*必須フィールド: "name" および "videoUrl"*</span><span class="sxs-lookup"><span data-stu-id="bffae-203">*Required fields: "name" and "videoUrl"*</span></span>

```json
{
    "name": "Ninja Twitch Live Stream",
    "videoUrl":"https://www.twitch.tv/ninja",
    "volume":0.2,
    "startTime":0,
    "endOfVideoAction":"play-next"
}
```

### <a name="example-json"></a><span data-ttu-id="bffae-204">JSON の例</span><span class="sxs-lookup"><span data-stu-id="bffae-204">Example JSON</span></span>

```json
{
  "loopMediaList": false,
  "startMethod": "autostart-beginning",
  "controlMediaPlayer": "everyone",
  "configureMediaPlayer": "elevated",
  "mediaList": [
    {
      "videoUrl": "https://www.twitch.tv/ninja",
      "volume": 0.2,
      "startTime": 0,
      "endOfVideoAction": "play-next"
    },
    {
      "imageUrl": "http://www.hypergridbusiness.com/wp-content/uploads/2016/09/AltspaceVR-highrise.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://d1qb2nb5cznatu.cloudfront.net/startups/i/333629-6ffd7199b9bcf34d8957e8e09d974a38-medium_jpg.jpg?buster=1423092095",
      "skipAfter": 5
    },
    {
      "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://altvr-wpengine.netdna-ssl.com/wp-content/uploads/2019/05/Educators-in-VR-Social-VR-AltspaceVR.png",
      "skipAfter": 10
    },
    {
      "videoUrl": "https://www.twitch.tv/shroud",
      "volume": 1,
      "startTime": 0,
      "endOfVideoAction": "stop"
    }
  ]
}
```

### <a name="schema"></a><span data-ttu-id="bffae-205">スキーマ</span><span class="sxs-lookup"><span data-stu-id="bffae-205">Schema</span></span>

```json
{
  "$schema": "https://json-schema.org/draft-04/schema#",
  "type": "object",
  "required": [
    "mediaList"
  ],
  "properties": {
    "loopMediaList": {
      "type": "boolean",
      "description": "Whether to loop through the media list when reaching the beginning or end of the list."
    },
    "controlMediaPlayer": {
      "type": "string",
      "enum": [
        "everyone",
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are able to control the media player. (Owner can always control player)"
    },
    "configureMediaPlayer": {
      "type": "string",
      "enum": [
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are allowed to configure the media play list.  Note: This role needs to be able to control the media player in order to configure it. (Owner can always configure media)"
    },
    "startMethod": {
      "type": "string",
      "enum": [
        "manual",
        "autostart-beginning",
        "autostart-random"
      ],
      "default": "manual",
      "description": "The method by which the media player should start"
    },
    "mediaList": {
      "description": "A list of images or videos to configure the media player to operate on.",
      "type": "array",
      "items": {
        "oneOf": [
          {
            "title": "Image",
            "type": "object",
            "description": "Configuration for an image media.",
            "properties": {
              "imageUrl": {
                "type": "string",
                "description": "The url for the image to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              }
            },
            "required": [
              "imageUrl"
            ]
          },
          {
            "title": "Video",
            "type": "object",
            "description": "Configuration for a video media.",
            "properties": {
              "videoUrl": {
                "type": "string",
                "description": "The url of the video to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              },
              "volume": {
                "type": "number",
                "minimum": 0,
                "maximum": 1,
                "default": null,
                "description": "The volume to play the video at. (Minimum 0, maximum 1)"
              },
              "startTime": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The time in seconds from the start of the video to begin playing the video at. (Minimum of 0)"
              },
              "rolloffStartDistance": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The distance in meters away from the media player that the volume will begin to fall off. (Minimum 0)"
              },
              "endOfVideoAction": {
                "type": "string",
                "enum": [
                  "stop",
                  "loop",
                  "play-next"
                ],
                "default": null,
                "description": "The type of action to take at the end of the video."
              }
            },
            "required": [
              "videoUrl"
            ]
          }
        ]
      }
    }
  }
}
```

> [!NOTE]
> <span data-ttu-id="bffae-206">マルチメディアコンソール v 0.5.0 を使用した最新の状態</span><span class="sxs-lookup"><span data-stu-id="bffae-206">Up to date with Multimedia Console v0.5.0</span></span>