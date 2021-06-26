---
title: マルチメディア コンソールの使用
description: AltspaceVR エクスペリエンスでマルチメディア コンソールの構成、発行、制御を開始する方法について説明します。
ms.date: 03/11/2021
ms.topic: article
keywords: コンソール、マルチメディア
ms.openlocfilehash: 4a51ff76e44d3870972bc17288ae77c1fa888922
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923009"
---
# <a name="using-the-multimedia-console"></a><span data-ttu-id="2c1e1-104">マルチメディア コンソールの使用</span><span class="sxs-lookup"><span data-stu-id="2c1e1-104">Using the multimedia console</span></span>

<span data-ttu-id="2c1e1-105">マルチメディア コンソールは、イベントや世界でのメディア共有を可能にするツールです。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-105">The Multimedia Console is a tool that enables media sharing in events and worlds.</span></span> <span data-ttu-id="2c1e1-106">画像、プレゼンテーション スライド、ライブストリーム、ビデオ、プレイリストなど、その他を共有するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-106">You can use it to share things like images, presentation slides, livestreams, videos, playlists, and more.</span></span> <span data-ttu-id="2c1e1-107">マルチメディア コンソール **v0.5.0+** の使い方の詳細な手順を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-107">Below is a step-by-step instruction on how to use the Multimedia Console **v0.5.0+**.</span></span> 

## <a name="getting-started"></a><span data-ttu-id="2c1e1-108">はじめに</span><span class="sxs-lookup"><span data-stu-id="2c1e1-108">Getting started</span></span>

<span data-ttu-id="2c1e1-109">マルチメディア コンソールの使用は、2 部構成のプロセスです。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-109">Getting started with the Multimedia Console is a two part process.</span></span>  <span data-ttu-id="2c1e1-110">まず、環境に配置するマルチメディア コンソール セッションの構成を生成して発行するために使用する Web ポータルがあります。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-110">First there's the web portal that you'll use to generate and publish a configuration for the Multimedia Console session you place in your environment.</span></span>  <span data-ttu-id="2c1e1-111">2 つ目は、実際のマルチメディア コンソール アプリを環境内に配置し、使用する必要がある構成コードを設定する方法です。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-111">Second is the placement of the actual Multimedia Console app in your environment and setting the configuration code it should use.</span></span>

### <a name="configuring-the-multimedia-console-with-the-web-portal"></a><span data-ttu-id="2c1e1-112">Web ポータルを使用したマルチメディア コンソールの構成</span><span class="sxs-lookup"><span data-stu-id="2c1e1-112">Configuring the Multimedia console with the web portal</span></span>

1. <span data-ttu-id="2c1e1-113">まず、URL が必要なので、コンテンツがオンラインでホストされている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-113">First, you'll need to make sure your content is hosted online because you'll need a URL.</span></span> <span data-ttu-id="2c1e1-114">(画像に写真をアップロード altvr.com、オンラインでビデオ .mp4ホストしたり、Dlive ライブ ストリーム リンクを使用することができます。 https://dlive.tv/yourlivestream)</span><span class="sxs-lookup"><span data-stu-id="2c1e1-114">(You can upload photos to altvr.com, host a video .mp4 file online or use a Dlive live stream link: https://dlive.tv/yourlivestream)</span></span> 
2. <span data-ttu-id="2c1e1-115">マルチメディア コンソールの Web ポータル () に移動します。 [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)</span><span class="sxs-lookup"><span data-stu-id="2c1e1-115">Navigate to the web portal for the Multimedia Console at [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)</span></span>
3. <span data-ttu-id="2c1e1-116">Web ポータルから、マルチメディア コンソールの構成を生成して発行できます。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-116">From the web portal, you can generate and publish a configuration for the Multimedia Console.</span></span>  <span data-ttu-id="2c1e1-117">(さまざまなプロパティの詳細については、以下を参照してください)。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-117">(See below for details about the various properties).</span></span>
4. <span data-ttu-id="2c1e1-118">メディアの一覧にメディアを入力し、全般設定を構成したら、アプリの上部にある [発行] ボタンを選択します。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-118">Once you've entered the media into the media list and have configured the general settings, select the publish button in the top-right part of the app.</span></span>
5. <span data-ttu-id="2c1e1-119">発行が完了すると、配置したマルチメディア コンソールに入力する 2 つの単語コードがダイアログに表示されます。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-119">Once the publish has completed, a dialog will pop up with a two word code for you to enter in to the Multimedia Console you placed.</span></span>
  
### <a name="placing-the-multimedia-console-in-your-environment"></a><span data-ttu-id="2c1e1-120">環境にマルチメディア コンソールを配置する</span><span class="sxs-lookup"><span data-stu-id="2c1e1-120">Placing the Multimedia console in your environment</span></span>

1. <span data-ttu-id="2c1e1-121">[World **Editor]/(ワールド エディター> エディター パネル> SDK Apps > マルチメディア コンソール] を選択します**。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-121">Select on **World Editor > Editor Panel > SDK Apps > Multimedia Console**.</span></span> <span data-ttu-id="2c1e1-122">([World Editor > Basics > **SDK App(** 登録されていないアプリの場合) に移動しない。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-122">(Don't go to **World Editor > Basics > SDK App**--that's for unregistered apps.)</span></span>  
2. <span data-ttu-id="2c1e1-123">空間と対象ユーザーに最適なマルチメディア コンソールを配置します。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-123">Position the Multimedia Console to best suite your space and audience.</span></span>
3. <span data-ttu-id="2c1e1-124">オレンジ色の [編集モード] ボタンをクリックして、編集モードから抜け出します。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-124">Get out of Edit Mode by clicking the orange Edit Mode button.</span></span>
4. <span data-ttu-id="2c1e1-125">メディア プレーヤーの所有者ですか **? というメッセージが表示されます。**</span><span class="sxs-lookup"><span data-stu-id="2c1e1-125">You'll be prompted **Are you the media player owner?**</span></span> <span data-ttu-id="2c1e1-126">このマルチメディア コンソール セッションの正式な所有者である必要があるユーザーは、確認して続行します。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-126">If you're the person who should be the official owner of this Multimedia Console session, confirm and continue.</span></span> <span data-ttu-id="2c1e1-127">(その他のアクセス許可ロールも使用できます。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-127">(Other permissioned roles are available as well.</span></span> <span data-ttu-id="2c1e1-128">詳細な一覧については、以下を参照してください)。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-128">See below for a detailed list.)</span></span>
5. <span data-ttu-id="2c1e1-129">[はい] を選択して、プライマリ ホストを確認します。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-129">Select Yes to confirm that you are the primary host.</span></span>  
6. <span data-ttu-id="2c1e1-130">Web ポータルまたは有効な JSON からコードを入力するダイアログが表示されます。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-130">A dialog should pop up that asks you to enter a code from the web portal or valid JSON.</span></span>  <span data-ttu-id="2c1e1-131">Web ポータルからダッシュを含む 2 つの単語コードを入力し、[OK] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-131">Enter the two word code from the web portal including the dash and hit OK.</span></span> <span data-ttu-id="2c1e1-132">(JSON は、以下で説明する高度な構成です)</span><span class="sxs-lookup"><span data-stu-id="2c1e1-132">(JSON is an advanced configuration described below)</span></span>
7. <span data-ttu-id="2c1e1-133">マルチメディア コンソールは、Web ポータルで構築した構成で数秒後に読み込む必要があります。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-133">The Multimedia Console should load after a few seconds with the configuration you built in the web portal.</span></span>

### <a name="controlling-the-multimedia-console"></a><span data-ttu-id="2c1e1-134">マルチメディア コンソールの制御</span><span class="sxs-lookup"><span data-stu-id="2c1e1-134">Controlling the Multimedia console</span></span>

1. <span data-ttu-id="2c1e1-135">コードを入力して構成プロセスを完了すると、メディアディスプレイの下にコントロール ボタンが表示されます。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-135">After you input your code and complete the configuration process, you'll see control buttons appear below a media display.</span></span> 
    * <span data-ttu-id="2c1e1-136">**再生** によってメディア ビューアーが開始されます (または、以前に停止した場合は現在のエントリで再起動します)</span><span class="sxs-lookup"><span data-stu-id="2c1e1-136">**Play** starts the media viewer (or restarts at current entry, if previously stopped)</span></span> 
    * <span data-ttu-id="2c1e1-137">**[停止** ] を選択すると、メディア ビューアーが停止し、現在のメディアが非表示にされます。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-137">**Stop** stops the media viewer, and hides current media.</span></span>  
    * <span data-ttu-id="2c1e1-138">**Next/Prev は** 次のメディアまたは前のメディアにスキップします</span><span class="sxs-lookup"><span data-stu-id="2c1e1-138">**Next/Prev** skips to next or previous media</span></span> 
    * <span data-ttu-id="2c1e1-139">**x/x**  では、現在のインデックスがメディア リストに表示され、リスト内の任意のポイントにジャンプできます。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-139">**x/x** shows the current index into the media list, and allows you to jump to any point in the list</span></span>
    * <span data-ttu-id="2c1e1-140">**構成** を使用すると、Web ポータルから新しいコードを再入力して、コンソールで新しい構成を設定できます。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-140">**Config** allows reentering a new code from the web portal to set a new configuration in the console.</span></span> 

<span data-ttu-id="2c1e1-141">これで、マルチメディア コンソールを使用して共有を開始します。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-141">Now you're set to begin sharing via the Multimedia Console!</span></span>  
 
## <a name="working-with-the-web-portal"></a><span data-ttu-id="2c1e1-142">Web ポータルの操作</span><span class="sxs-lookup"><span data-stu-id="2c1e1-142">Working with the web portal</span></span>

<span data-ttu-id="2c1e1-143">Web ポータルは、マルチメディア コンソールのさまざまな機能を構成できる Web アプリです。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-143">The web portal is a web app that enables configuring the various features of the Multimedia Console.</span></span>  <span data-ttu-id="2c1e1-144">これらの機能は 2 つのカテゴリに分類されます。一般的なメディア コンソール設定とメディア 再生リスト。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-144">These features fall in to two categories; general media console settings, and the media play list.</span></span>

### <a name="multimedia-console-general-settings"></a><span data-ttu-id="2c1e1-145">マルチメディア コンソールの全般設定</span><span class="sxs-lookup"><span data-stu-id="2c1e1-145">Multimedia console general settings</span></span>

<span data-ttu-id="2c1e1-146">**再生設定**</span><span class="sxs-lookup"><span data-stu-id="2c1e1-146">**Playback Settings**</span></span>

<span data-ttu-id="2c1e1-147">メディア リストの一般的な再生設定</span><span class="sxs-lookup"><span data-stu-id="2c1e1-147">General playback settings for the media list</span></span>

* <span data-ttu-id="2c1e1-148">**[メディアリストの** ループ] - リストの末尾に到達したら、メディア リストをループ処理するかどうかを決定します。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-148">**Loop Media List**- Determines whether the media list should loop around once you reach the end of the list.</span></span>
* <span data-ttu-id="2c1e1-149">**Start メソッド** - マルチメディア コンソールを開始する方法を選択します。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-149">**Start Method** - Selects the method by which the multimedia console should start.</span></span>
    * <span data-ttu-id="2c1e1-150">手動 - メディアを起動する前に再生ボタンが押されるのを待ちます</span><span class="sxs-lookup"><span data-stu-id="2c1e1-150">Manual - Waits for the play button to be pressed before starting the media</span></span>
    * <span data-ttu-id="2c1e1-151">[開始から自動開始] - 一覧の先頭からメディア リストを自動開始します</span><span class="sxs-lookup"><span data-stu-id="2c1e1-151">Auto Start from Beginning - Auto start the media list from the beginning of the list</span></span>
    * <span data-ttu-id="2c1e1-152">自動開始ランダム - 一覧のランダムな開始点からメディアを自動開始します</span><span class="sxs-lookup"><span data-stu-id="2c1e1-152">Auto Start Random - Auto starts the media from a random starting point in the list</span></span>

<span data-ttu-id="2c1e1-153">**ロール**</span><span class="sxs-lookup"><span data-stu-id="2c1e1-153">**Roles**</span></span>

<span data-ttu-id="2c1e1-154">マルチメディア コンソールを制御および構成するためのロールの割り当て。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-154">Role assignments for controlling and configuring the Multimedia Console.</span></span>    <span data-ttu-id="2c1e1-155">これらのロールは、次のセットに分けらされます。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-155">These roles are broken down in to the following set:</span></span>

* <span data-ttu-id="2c1e1-156">**所有者のみ** - マルチメディア コンソール セッションの所有者であるユーザー</span><span class="sxs-lookup"><span data-stu-id="2c1e1-156">**Owner Only** - The user that is the owner of the Multimedia Console Session</span></span>
* <span data-ttu-id="2c1e1-157">**昇格されたユーザー** - マルチメディア コンソールが最初に構成されている領域にモデレーターまたはホスト ロールを持つユーザー</span><span class="sxs-lookup"><span data-stu-id="2c1e1-157">**Elevated Users** - Users that have moderator or host roles in the space that the Multimedia Console is configured in originally</span></span>
* <span data-ttu-id="2c1e1-158">**すべてのユーザー** - すべてのユーザー</span><span class="sxs-lookup"><span data-stu-id="2c1e1-158">**All Users** - All users</span></span>

<span data-ttu-id="2c1e1-159">これらのロールは、この一覧で選択したロールより上のすべてのロールにも、その機能を使用するためのアクセス許可が付与されるという意味でスタックします。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-159">These roles stack in the sense that all roles above the one chosen in this list will also be granted permission to use that feature.</span></span>  <span data-ttu-id="2c1e1-160">例:**管理者特権のユーザー** には、AltspaceVR のモデレーターまたはホストではない場合でも所有者が含まれます。 </span><span class="sxs-lookup"><span data-stu-id="2c1e1-160">Example: **Elevated Users** includes the **Owner** even if they aren't a moderator or host\*\* in AltspaceVR.</span></span> <span data-ttu-id="2c1e1-161">ロールの割り当てによって制御される機能は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-161">Features that are controlled by role assignments are as follows</span></span>

* <span data-ttu-id="2c1e1-162">**メディア プレーヤーを制御できる** - マルチメディア コンソールのメディア再生ボタンを制御できるロールを決定します</span><span class="sxs-lookup"><span data-stu-id="2c1e1-162">**Can control media player** - Determines what roles can control the media playback buttons for the Multimedia Console</span></span>
* <span data-ttu-id="2c1e1-163">**メディア プレーヤーを構成できる** - [構成] ボタンへのアクセスを許可することで、マルチメディア コンソールを構成できるロールを **決定** します</span><span class="sxs-lookup"><span data-stu-id="2c1e1-163">**Can configure the media player** - Determines what roles can configure the Multimedia Console by being granted access to the **Config** button</span></span>

### <a name="adding-photos-and-videos-to-the-media-list"></a><span data-ttu-id="2c1e1-164">メディア リストへの写真とビデオの追加</span><span class="sxs-lookup"><span data-stu-id="2c1e1-164">Adding photos and videos to the media list</span></span>

<span data-ttu-id="2c1e1-165">メディアはマルチメディア コンソールの中心です。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-165">Media is the heart of the Multimedia Console.</span></span>  <span data-ttu-id="2c1e1-166">画像とビデオ リンクは、マルチメディア コンソール内でメディアの種類としてサポートされています。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-166">Images and video links are supported as media types within the Multimedia Console.</span></span>  <span data-ttu-id="2c1e1-167">新しいメディアを追加するには、[イメージの追加]アイコンまたは [ビデオの追加] アイコンを選択して、メディア情報と設定を入力するダイアログ をポップアップ表示します。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-167">To add new media, select either the **Add Image** or **Add Video** icons to have a dialog pop up to enter the media information and settings.</span></span>  <span data-ttu-id="2c1e1-168">メディアの種類と関連する設定の内訳を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-168">Below is the breakdown of the media types and associated settings</span></span>

<span data-ttu-id="2c1e1-169">**Image**</span><span class="sxs-lookup"><span data-stu-id="2c1e1-169">**Image**</span></span>

<span data-ttu-id="2c1e1-170">画像は、jpeg、png、および子などの標準的な画像の種類である必要があります。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-170">Images should be a standard image type such as jpeg, png, and son on.</span></span> <span data-ttu-id="2c1e1-171">パブリック リンクを使用してどこかでホストする必要があります。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-171">They need to be hosted somewhere with a public link.</span></span>

* <span data-ttu-id="2c1e1-172">**名前** - (必須) イメージを識別する名前。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-172">**Name** - (Required) Name that you wish to identify the image with.</span></span>
* <span data-ttu-id="2c1e1-173">**イメージ URL** - (必須) イメージのパブリック URL</span><span class="sxs-lookup"><span data-stu-id="2c1e1-173">**Image URL** - (Required) The public url of the image</span></span>
* <span data-ttu-id="2c1e1-174">**Skip After** - イメージをスキップする必要がある時間 (秒)</span><span class="sxs-lookup"><span data-stu-id="2c1e1-174">**Skip After** - The number of seconds that the image should be skipped after</span></span>

<span data-ttu-id="2c1e1-175">**ビデオ**</span><span class="sxs-lookup"><span data-stu-id="2c1e1-175">**Video**</span></span>

<span data-ttu-id="2c1e1-176">ビデオは、Twitch と DLive を介してビデオまたはライブ ストリームをホストできます。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-176">Videos can be hosted videos or live streams through Twitch and DLive.</span></span>  <span data-ttu-id="2c1e1-177">(その他のサポートは、適切なストリーム URL を取得するために追加の作業で機能する場合がありますが、マルチメディア コンソール内では完全にはサポートされていません)</span><span class="sxs-lookup"><span data-stu-id="2c1e1-177">(Other support may function with extra work to get the proper stream url, but aren't fully supported within the Multimedia Console)</span></span>

* <span data-ttu-id="2c1e1-178">**名前** - (必須) ビデオを識別する名前。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-178">**Name** - (Required) Name that you wish to identify the video with.</span></span>
* <span data-ttu-id="2c1e1-179">**ビデオ URL** - (必須) ビデオがホストされているパブリック URL。またはライブ ストリームが提供されます。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-179">**Video URL** - (Required) The public url that the video is hosted at or the live stream is served from.</span></span>
* <span data-ttu-id="2c1e1-180">**Skip After** - ビデオのスキップ後にスキップする必要がある時間 (秒)</span><span class="sxs-lookup"><span data-stu-id="2c1e1-180">**Skip After** - The number of seconds that the video should be skipped after</span></span>

> [!NOTE]
> <span data-ttu-id="2c1e1-181">必須: ビデオの長さと一致する時間を入力して、ビデオを正しく転送します。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-181">REQUIRED: Put in the time that matches the length of the video to enable videos to properly forward.</span></span> <span data-ttu-id="2c1e1-182">たとえば、ビデオの長さ 5 分が 300 秒の場合、ビデオは次のコンテンツにスキップされます。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-182">For example, if your video is 5 minutes long put 300 seconds, otherwise your video won't skip to the next piece of content.</span></span>

* <span data-ttu-id="2c1e1-183">**ボリューム** - 0 (分) から 1 (最大) の値のビデオのボリューム。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-183">**Volume** - The volume of the video from 0 (min) - 1 (max) values.</span></span>
* <span data-ttu-id="2c1e1-184">**[開始時刻** ] - ビデオの開始から開始する時間 (秒)。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-184">**Start Time** - The number of seconds from the beginning of the video start from.</span></span>
* <span data-ttu-id="2c1e1-185">**Roll Off Start Distance** (開始距離のロールオフ) - マルチメディア コンソールから離れるとボリュームが落ち始める世界のメートルの距離</span><span class="sxs-lookup"><span data-stu-id="2c1e1-185">**Roll Off Start Distance** - The distance in meters in world that the volume begins to fall off at as you move away from the Multimedia Console</span></span>
* <span data-ttu-id="2c1e1-186">**[End of Video Action]/(** ビデオの終了アクション)- ビデオの末尾に到達したら実行するアクション。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-186">**End of Video Action** - The action to take once the end of the video is reached.</span></span>
    * <span data-ttu-id="2c1e1-187">[停止] - ビデオが終了した後にメディアリストが停止します</span><span class="sxs-lookup"><span data-stu-id="2c1e1-187">Stop - The media list stops after the video has ended</span></span>
    * <span data-ttu-id="2c1e1-188">ループ - ビデオは手動でスキップされるまでループします</span><span class="sxs-lookup"><span data-stu-id="2c1e1-188">Loop - The video will loop until manually skipped</span></span>
    * <span data-ttu-id="2c1e1-189">[次へ再生] - メディアリスト内の次のメディアは、現在のビデオが終了した後に開始されます。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-189">Play Next - The next media in the media list will be started after the current video ends.</span></span>

## <a name="working-with-json-directly-advancedoptional"></a><span data-ttu-id="2c1e1-190">JSON を直接操作する (詳細/省略可能)</span><span class="sxs-lookup"><span data-stu-id="2c1e1-190">Working with JSON directly (advanced/optional)</span></span>

<span data-ttu-id="2c1e1-191">マルチメディア コンソールでは、AltspaceVR でコンソールのプロンプトに直接 JSON を入力できます。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-191">The Multimedia Console supports entering JSON directly in to the prompt of the console in AltspaceVR.</span></span>  <span data-ttu-id="2c1e1-192">JSON は、メディア プレーヤーの構成を有効にする内部メカニズムです。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-192">JSON is the internal mechanism with which we enable media player configurations.</span></span> <span data-ttu-id="2c1e1-193">JSON を直接設定する機能を公開することで、より高度なユーザーは、JSON に対するニーズと使い慣れた独自のワークフローを構築できます。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-193">Exposing the ability to set JSON directly is something that allows for more advanced users to build their own workflows that suites their needs and familiarity with JSON.</span></span>  <span data-ttu-id="2c1e1-194">JSON 構造と JSON の検証に使用されるスキーマの簡単な説明を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-194">The following is a brief description of the JSON structure and the schema by which the JSON is validated.</span></span> <span data-ttu-id="2c1e1-195">以下のプロパティの詳細については、マルチメディア コンソールの構成に関する上記のセクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-195">For more detailed descriptions of the properties below, see the above sections that talk about configuring the Multimedia Console.</span></span>  <span data-ttu-id="2c1e1-196">このセクションでは、主に JSON データのスキーマの例と構造化に重点を置いて説明します。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-196">This section is focused primarily on the schema examples and structuring for the JSON data.</span></span>

### <a name="global-media-settings"></a><span data-ttu-id="2c1e1-197">グローバル メディア設定</span><span class="sxs-lookup"><span data-stu-id="2c1e1-197">Global media settings</span></span>

```json
{
  "loopMediaList": true | false
  "startMethod": "manual" | "autostart-beginning" | "autostart-random"
  "controlMediaPlayer": "everyone" | "elevated" | "owner"
  "configureMediaPlayer": "elevated" | "owner"
  ...
}
```

### <a name="media-list"></a><span data-ttu-id="2c1e1-198">メディア一覧</span><span class="sxs-lookup"><span data-stu-id="2c1e1-198">Media list</span></span>

<span data-ttu-id="2c1e1-199">メディア リストは、JSON 構造のルート (ロールや再生設定など) に設定されたプロパティです。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-199">The media list is a property set at the root of the JSON structure like the Roles and Playback Settings.</span></span>  <span data-ttu-id="2c1e1-200">これは、次のいずれかのメディア構成構造を含む単純な配列です。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-200">It's a simple array that can contain one of the following media configuration structures.</span></span> <span data-ttu-id="2c1e1-201">(それぞれの機能の詳細については、上記のプロパティの説明を参照してください)。</span><span class="sxs-lookup"><span data-stu-id="2c1e1-201">(See property descriptions above for details on what each does.)</span></span>

<span data-ttu-id="2c1e1-202">**画像の例**</span><span class="sxs-lookup"><span data-stu-id="2c1e1-202">**Image example**</span></span>

<span data-ttu-id="2c1e1-203">*必須フィールド: "name" および "imageUrl"*</span><span class="sxs-lookup"><span data-stu-id="2c1e1-203">*Required fields: "name" and "imageUrl"*</span></span>

```json
{
    "name": "Altspace Screenshot",
    "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
    "skipAfter": 10
}
```

<span data-ttu-id="2c1e1-204">**ビデオの例**</span><span class="sxs-lookup"><span data-stu-id="2c1e1-204">**Video example**</span></span>

<span data-ttu-id="2c1e1-205">*必須フィールド: "name" および "videoUrl"*</span><span class="sxs-lookup"><span data-stu-id="2c1e1-205">*Required fields: "name" and "videoUrl"*</span></span>

```json
{
    "name": "Ninja Twitch Live Stream",
    "videoUrl":"https://www.twitch.tv/ninja",
    "volume":0.2,
    "startTime":0,
    "endOfVideoAction":"play-next"
}
```

### <a name="example-json"></a><span data-ttu-id="2c1e1-206">JSON の例</span><span class="sxs-lookup"><span data-stu-id="2c1e1-206">Example JSON</span></span>

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

### <a name="schema"></a><span data-ttu-id="2c1e1-207">スキーマ</span><span class="sxs-lookup"><span data-stu-id="2c1e1-207">Schema</span></span>

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
> <span data-ttu-id="2c1e1-208">マルチメディアコンソール v 0.5.0 を使用した最新の状態</span><span class="sxs-lookup"><span data-stu-id="2c1e1-208">Up to date with Multimedia Console v0.5.0</span></span>