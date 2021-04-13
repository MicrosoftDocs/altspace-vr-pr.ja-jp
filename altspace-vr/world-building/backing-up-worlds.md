---
title: ワールドをバックアップする
description: Altのバックアップスナップショットを作成、管理、トラブルシューティングする方法について説明します。
ms.date: 03/11/2021
ms.topic: article
keywords: 保存
ms.openlocfilehash: fdef692c737bf2f92db315e04556831d60c2f377
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212658"
---
# <a name="backing-up-your-worlds"></a><span data-ttu-id="28b8d-104">ワールドをバックアップする</span><span class="sxs-lookup"><span data-stu-id="28b8d-104">Backing up your worlds</span></span>

<span data-ttu-id="28b8d-105">バックアップは、特定の時点における世界中のすべてのオブジェクトの "スナップショット" またはレコードです。</span><span class="sxs-lookup"><span data-stu-id="28b8d-105">A Backup is a “snapshot” or record of all the objects in a World at a specific point in time.</span></span> <span data-ttu-id="28b8d-106">たとえば、夢の家を作り、1日でリビングルームを誤って削除したとします。</span><span class="sxs-lookup"><span data-stu-id="28b8d-106">Suppose you’re building your Dream House and one day you accidentally deleted the living room.</span></span> <span data-ttu-id="28b8d-107">1日前に世界のバックアップを作成したことがある場合は、特定のバックアップを復元し、世界をリセットし、パニック攻撃を回避することができます。</span><span class="sxs-lookup"><span data-stu-id="28b8d-107">If you had created a Backup of your World the day before, you could restore that particular backup, reset your World, and avoid a panic attack.</span></span> <span data-ttu-id="28b8d-108">または、季節ごとに woods のバージョンがあり、それらを切り替えることができるかもしれませんが、バックアップを使用してこれを行うことができます。</span><span class="sxs-lookup"><span data-stu-id="28b8d-108">Or perhaps you have a version of your cabin-in-the-woods for every season and you like to switch back and forth between them—you can do that with Backups.</span></span> <span data-ttu-id="28b8d-109">各バックアップは、1つの世界に固有であり、変換 (位置、回転、スケール) だけでなく、オブジェクトのその他の設定も含まれています。</span><span class="sxs-lookup"><span data-stu-id="28b8d-109">Each Backup is specific to a single World and contains not only the transforms (position, rotation, scale) but also other settings on the objects.</span></span> <span data-ttu-id="28b8d-110">1つの環境で作成できるバックアップの数に制限はありません。</span><span class="sxs-lookup"><span data-stu-id="28b8d-110">There's no limit to the number of Backups you can create for a World.</span></span>  

## <a name="whats-included-in-a-backup"></a><span data-ttu-id="28b8d-111">バックアップに含まれるもの</span><span class="sxs-lookup"><span data-stu-id="28b8d-111">What’s included in a Backup?</span></span>

<span data-ttu-id="28b8d-112">現在、バックアップには、ワールドエディターを使用して生成できるほとんどの項目が含まれています。</span><span class="sxs-lookup"><span data-stu-id="28b8d-112">A Backup currently includes most things you can spawn with the World Editor:</span></span>
* <span data-ttu-id="28b8d-113">成果物 (キットオブジェクト)</span><span class="sxs-lookup"><span data-stu-id="28b8d-113">Artifacts (Kit objects)</span></span>
* <span data-ttu-id="28b8d-114">ラベル</span><span class="sxs-lookup"><span data-stu-id="28b8d-114">Labels</span></span>
* <span data-ttu-id="28b8d-115">テレポーター</span><span class="sxs-lookup"><span data-stu-id="28b8d-115">Teleporters</span></span>
* <span data-ttu-id="28b8d-116">ポイントの生成</span><span class="sxs-lookup"><span data-stu-id="28b8d-116">Spawn Points</span></span>
* <span data-ttu-id="28b8d-117">Photos</span><span class="sxs-lookup"><span data-stu-id="28b8d-117">Photos</span></span>
* <span data-ttu-id="28b8d-118">MRE SDK アプリ</span><span class="sxs-lookup"><span data-stu-id="28b8d-118">MRE SDK Apps</span></span>
* <span data-ttu-id="28b8d-119">ネイティブアプリ (たとえば、現実に対するホログラム)</span><span class="sxs-lookup"><span data-stu-id="28b8d-119">Native Apps (for example, Holograms Against Reality)</span></span>

<span data-ttu-id="28b8d-120">次のものは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="28b8d-120">The following isn’t included:</span></span>

* <span data-ttu-id="28b8d-121">レイアウトのオーバーライド</span><span class="sxs-lookup"><span data-stu-id="28b8d-121">Layout overrides</span></span>
* <span data-ttu-id="28b8d-122">Skyboxes とアンビエントサウンド</span><span class="sxs-lookup"><span data-stu-id="28b8d-122">Skyboxes and ambient sound</span></span>
* <span data-ttu-id="28b8d-123">テンプレート</span><span class="sxs-lookup"><span data-stu-id="28b8d-123">Templates</span></span>
* <span data-ttu-id="28b8d-124">手順</span><span class="sxs-lookup"><span data-stu-id="28b8d-124">Instructions</span></span>
* <span data-ttu-id="28b8d-125">ワールドロールとコンテキストロール</span><span class="sxs-lookup"><span data-stu-id="28b8d-125">World roles and contextual roles</span></span>

## <a name="managing-backups"></a><span data-ttu-id="28b8d-126">バックアップの管理</span><span class="sxs-lookup"><span data-stu-id="28b8d-126">Managing Backups</span></span>

<span data-ttu-id="28b8d-127">ワールドエディター/Altspace を開き、[バックアップ] をクリックして、バックアップを作成できます。</span><span class="sxs-lookup"><span data-stu-id="28b8d-127">You can create a Backup by opening your World Editor / Altspace and clicking on “Backups”.</span></span> <span data-ttu-id="28b8d-128">最初のボタンは、[新しいバックアップ] ボタンになります。</span><span class="sxs-lookup"><span data-stu-id="28b8d-128">The first button will be the “New Backup” button.</span></span> <span data-ttu-id="28b8d-129">バックアップを作成するときに、短い名前を入力するように求められます。</span><span class="sxs-lookup"><span data-stu-id="28b8d-129">When creating a Backup, you’ll be asked to provide a short name.</span></span> <span data-ttu-id="28b8d-130">これは省略可能ですが、非常に複雑になるため、強くお勧めします。</span><span class="sxs-lookup"><span data-stu-id="28b8d-130">This is optional but highly recommended because it will get confusing fast.</span></span> <span data-ttu-id="28b8d-131">既存のバックアップは、[作成] ボタンの後に一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="28b8d-131">Existing backups will be listed after the “Create” button.</span></span> <span data-ttu-id="28b8d-132">既存のバックアップをクリックすると、復元が開始されます。</span><span class="sxs-lookup"><span data-stu-id="28b8d-132">Clicking on an existing Backup will start a restore.</span></span> <span data-ttu-id="28b8d-133">バックアップを復元するとき、しばらくすると世界の状態がリセットされますが、変更が反映されていない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="28b8d-133">When restoring a Backup, your World will reset after a few moments but you may not see the changes reflected.</span></span> <span data-ttu-id="28b8d-134">1 ~ 2 分待ってから、もう一度ワールドをリセットします。</span><span class="sxs-lookup"><span data-stu-id="28b8d-134">Wait a minute or two and reset your World again.</span></span> <span data-ttu-id="28b8d-135">**現在、VR でバックアップを編集または削除する方法はありません**。</span><span class="sxs-lookup"><span data-stu-id="28b8d-135">**There's currently no way to edit or delete a Backup in VR**.</span></span> <span data-ttu-id="28b8d-136">現時点では、web サイトでバックアップを管理する必要があります。</span><span class="sxs-lookup"><span data-stu-id="28b8d-136">You'll need to manage your Backups on our website for now.</span></span> <span data-ttu-id="28b8d-137">(VR でのバックアップ管理が間もなく改善される予定です。</span><span class="sxs-lookup"><span data-stu-id="28b8d-137">(Backup management in VR will be improved soon.</span></span> <span data-ttu-id="28b8d-138">それまでの間、ぜひご連絡ください)。</span><span class="sxs-lookup"><span data-stu-id="28b8d-138">In the meantime, bear with us).</span></span>

<span data-ttu-id="28b8d-139">Web サイトでバックアップを管理するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="28b8d-139">To manage your Backups on our website:</span></span>

1. <span data-ttu-id="28b8d-140">自分のワールド [>](https://account.altvr.com/users/sign_in)に移動し、世界を見つけて、管理者コントロールで [バックアップ] を押します。</span><span class="sxs-lookup"><span data-stu-id="28b8d-140">Navigate to [Worlds > Mine](https://account.altvr.com/users/sign_in), find your World, and press “Backups” in the Administrator Controls:</span></span>

![[バックアップ] パネルが開いているワールド web サイトの管理者コントロール](images/world-backup-img-01.png)

2. <span data-ttu-id="28b8d-142">バックアップを作成、編集、および削除したり、オブジェクトの数を確認したり、プレビューイメージをアップロードしたりすることもできます。</span><span class="sxs-lookup"><span data-stu-id="28b8d-142">You can create, edit, and delete your Backups, check how many objects are inside, and even upload a preview image:</span></span> 

![Create、edit、および delete コマンドが強調表示されている [バックアップ] ウィンドウ](images/world-backup-img-02.png)

<span data-ttu-id="28b8d-144">バックアップの数に制限はなく、バックアップが多くなると、世界のパフォーマンスに影響を与えることはありません。</span><span class="sxs-lookup"><span data-stu-id="28b8d-144">There's no limit to the number of Backups and having more Backups won't impact the performance of your World.</span></span>

## <a name="other-ways-to-back-up-your-worlds"></a><span data-ttu-id="28b8d-145">お客様のワールドをバックアップするその他の方法</span><span class="sxs-lookup"><span data-stu-id="28b8d-145">Other ways to back up your Worlds</span></span>

* <span data-ttu-id="28b8d-146">別の世界を作成し、詳細オプションを表示して、世界からインポートします。</span><span class="sxs-lookup"><span data-stu-id="28b8d-146">Create another World, Show Advanced Options, and Import from World.</span></span> <span data-ttu-id="28b8d-147">ドロップダウンメニューから、バックアップを作成する世界を選択します。</span><span class="sxs-lookup"><span data-stu-id="28b8d-147">Choose the World you want to back up from the dropdown menu into the new one.</span></span> <span data-ttu-id="28b8d-148">インポートには制限がありません。</span><span class="sxs-lookup"><span data-stu-id="28b8d-148">There no limit for imports.</span></span>
* <span data-ttu-id="28b8d-149">Unity アップローダーを使用している場合は、バージョン管理を使用することを強くお勧めします。</span><span class="sxs-lookup"><span data-stu-id="28b8d-149">If you’re using the Unity Uploader, we strongly recommend you use version control.</span></span> <span data-ttu-id="28b8d-150">たとえば、 [Unity の Github](https://unity.github.com)などです。</span><span class="sxs-lookup"><span data-stu-id="28b8d-150">For example, [Github for Unity](https://unity.github.com).</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="28b8d-151">トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="28b8d-151">Troubleshooting</span></span>

<span data-ttu-id="28b8d-152">**ヘルプ誤ってバックアップを復元しても、作業が失われることは** 心配ありません。</span><span class="sxs-lookup"><span data-stu-id="28b8d-152">**Help! I accidentally restored a Backup and my work is gone** Don’t worry.</span></span> <span data-ttu-id="28b8d-153">古いバックアップを復元する前に、新しいバックアップを自動的に作成します。</span><span class="sxs-lookup"><span data-stu-id="28b8d-153">We automatically create a new Backup before restoring old one.</span></span> <span data-ttu-id="28b8d-154">名前に " **auto** " が付いているものを探し、そのタイムスタンプを復元します (たとえば、 **auto 2019-01-14t08:23:33-08:00**)。</span><span class="sxs-lookup"><span data-stu-id="28b8d-154">Look for one with a name starting with **Auto** with the right timestamp and restore that one (for example, **Auto 2019-01-14T08:23:33-08:00**).</span></span>  <span data-ttu-id="28b8d-155">これが機能しない場合は[Support request](https://help.altvr.com/hc/requests/new)を送信します</span><span class="sxs-lookup"><span data-stu-id="28b8d-155">If that doesn’t work submit a [Support request](https://help.altvr.com/hc/requests/new)</span></span>

<span data-ttu-id="28b8d-156">**バックアップを復元しましたが、一部のオブジェクトが不足してい** ます写真がある場合、その写真は削除されていますか。</span><span class="sxs-lookup"><span data-stu-id="28b8d-156">**I restored a Backup and some objects are missing** If any were photos, were those photos deleted?</span></span> <span data-ttu-id="28b8d-157">プライバシー上の理由から、削除された写真を復元することはできません。</span><span class="sxs-lookup"><span data-stu-id="28b8d-157">We can’t restore deleted photos for privacy reasons.</span></span> <span data-ttu-id="28b8d-158">調査できるように [Support request](https://help.altvr.com/hc/requests/new) を送信する</span><span class="sxs-lookup"><span data-stu-id="28b8d-158">Submit a [Support request](https://help.altvr.com/hc/requests/new) so we can investigate</span></span>

<span data-ttu-id="28b8d-159">**変更がまったく表示** されないバックアップは非同期に復元されます。つまり、オブジェクトの数によっては、復元に数分かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="28b8d-159">**I don’t see any changes** Backups are restored asynchronously meaning they can take a few minutes to restore depending on the number of objects.</span></span> <span data-ttu-id="28b8d-160">しばらく待ってから、もう一度リセットしてみてください。</span><span class="sxs-lookup"><span data-stu-id="28b8d-160">Remember to reset your World and if you don’t see anything after a few minutes try resetting again.</span></span> <span data-ttu-id="28b8d-161">今後は、復元プロセスの状態に関するフィードバックをさらに提供することができます。</span><span class="sxs-lookup"><span data-stu-id="28b8d-161">In the future, we can provide more feedback on the status of the restoration process</span></span>