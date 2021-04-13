---
title: ワールドロールの付与
description: ロールおよび機能システムについて説明し、ユーザーロールをユーザーに提供するための詳細な手順について説明します。
ms.date: 03/11/2021
ms.topic: article
keywords: roles
ms.openlocfilehash: f8cd55fbd8ede6cedd199724a3e6b2413c5bc3e6
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212791"
---
# <a name="granting-world-roles"></a><span data-ttu-id="1d46e-104">ワールドロールの付与</span><span class="sxs-lookup"><span data-stu-id="1d46e-104">Granting world roles</span></span>

<span data-ttu-id="1d46e-105">Altspace には、役割と能力システムがあります。</span><span class="sxs-lookup"><span data-stu-id="1d46e-105">Altspace has a Roles and Abilities system.</span></span> <span data-ttu-id="1d46e-106">各担当者は複数のロールを持つことができ、そのロールは、どこにあるかによって異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="1d46e-106">Each person can have multiple roles and their roles can be different depending on where they are.</span></span> <span data-ttu-id="1d46e-107">各ロールは、1つ以上の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="1d46e-107">Each role, in turn, gives you one or more abilities.</span></span> <span data-ttu-id="1d46e-108">たとえば、独自のイベントを使用している場合は、 **プレゼンター** ロールと **モデレーター** ロールが自動的に受信されます。</span><span class="sxs-lookup"><span data-stu-id="1d46e-108">For example, when you're in your own event, you automatically receive the **presenter** and **moderator** roles.</span></span> <span data-ttu-id="1d46e-109">これら2つのロールを使用すると、unruly のユーザーを開始し、ステージに配置して、紙ふぶき (をリリースする可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1d46e-109">With those two roles you can kick unruly users, be on stage, and maybe release the confetti.</span></span> 

1. <span data-ttu-id="1d46e-110">世界を編集し、[ **VR** ] セクション (「[ワールドの管理方法](managing-worlds.md)」) まで下にスクロールします。</span><span class="sxs-lookup"><span data-stu-id="1d46e-110">Edit your World and scroll down to the **In VR** section ([How to manage Worlds](managing-worlds.md))</span></span>

![ワールドの VR セクションでのロールの変更](images/granting-roles.png)

2. <span data-ttu-id="1d46e-112">この世界の特定のユーザーに特定のロールを付与する場合は、[ **ロール** ] フィールドを編集します。</span><span class="sxs-lookup"><span data-stu-id="1d46e-112">Edit the **Roles** field if you want to grant specific roles to specific users just for this World.</span></span> <span data-ttu-id="1d46e-113">たとえば、担当 **者** にモデレーターを与え、モデレーターにモデレーターを与える場合は、次のように入力  +  し、[**保存**] を選択します。 </span><span class="sxs-lookup"><span data-stu-id="1d46e-113">For example, if you want to give me **presenter** + **moderator** and give Calen **moderator**, you would add the following and select **Save**.</span></span> <span data-ttu-id="1d46e-114">各行の形式は **{role}、{username または email}** です。</span><span class="sxs-lookup"><span data-stu-id="1d46e-114">The format is **{role},{username or email}** on each line.</span></span> <span data-ttu-id="1d46e-115">ユーザー名は大文字と小文字を区別しません。</span><span class="sxs-lookup"><span data-stu-id="1d46e-115">Username is case-insensitive.</span></span> 

```
presenter,jimmy
moderator,jimmy
moderator,calen
```

3. <span data-ttu-id="1d46e-116">もう一度 [ **編集** ] を選択すると、[ロール] フィールドの上に次のように表示されます。</span><span class="sxs-lookup"><span data-stu-id="1d46e-116">If you select **Edit** again, you should see the following above the Roles field.</span></span> <span data-ttu-id="1d46e-117">データベースで更新されたことがわかります。</span><span class="sxs-lookup"><span data-stu-id="1d46e-117">That's how you know updated in the database.</span></span>

```
Presenters: jimmy
Moderators: jimmy,calen
```

* <span data-ttu-id="1d46e-118">変更が Altspace で有効になるようにするには、世界をリセットし、すべてのユーザーに再参加を強制する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1d46e-118">In order for the change to take effect in Altspace, you should reset the world, forcing everyone to rejoin.</span></span> <span data-ttu-id="1d46e-119">以下のすべてのロールの一覧が表示されます。</span><span class="sxs-lookup"><span data-stu-id="1d46e-119">There's a full list of roles below.</span></span>

4. <span data-ttu-id="1d46e-120">世界に参加するロールをすべてに付与する場合は、[ **コンテキストロール** ] フィールドを編集します。</span><span class="sxs-lookup"><span data-stu-id="1d46e-120">Edit the **Contextual Roles** field if you want to grant a role to every one that joins your World.</span></span> <span data-ttu-id="1d46e-121">たとえば、ユーザーがメガホンを使用して、遠くにいる間に聞くことができるようにするには、次のように追加します。</span><span class="sxs-lookup"><span data-stu-id="1d46e-121">For example, if you want to let people fly and use the megaphone so they can hear each other while far part, add the following:</span></span>

```
pilot,megaphone_only
```

<span data-ttu-id="1d46e-122">[ **更新**] を選択した後、世界をリセットします。</span><span class="sxs-lookup"><span data-stu-id="1d46e-122">After you select **Update**, reset the World.</span></span> <span data-ttu-id="1d46e-123">これは、この世界にのみ影響します。</span><span class="sxs-lookup"><span data-stu-id="1d46e-123">This will only affect this World.</span></span> <span data-ttu-id="1d46e-124">領域全体にロールを付与する場合は、Universe の同じフィールドを編集します。</span><span class="sxs-lookup"><span data-stu-id="1d46e-124">If you want to grant roles to an entire Universe, edit the same fields on the Universe.</span></span> 

## <a name="roles"></a><span data-ttu-id="1d46e-125">ロール</span><span class="sxs-lookup"><span data-stu-id="1d46e-125">Roles</span></span> 

* <span data-ttu-id="1d46e-126">段階で実行できるような **プレゼンター** の機能</span><span class="sxs-lookup"><span data-stu-id="1d46e-126">**Presenter** - abilities like being able to be on stage</span></span>
* <span data-ttu-id="1d46e-127">Decorum の管理を **開始** するような **モデレーター** の能力</span><span class="sxs-lookup"><span data-stu-id="1d46e-127">**Moderator** - abilities like **kick** to maintain decorum</span></span>
* <span data-ttu-id="1d46e-128">**Terraformer** -ワールドエディターを使用する機能</span><span class="sxs-lookup"><span data-stu-id="1d46e-128">**Terraformer** - ability to use the World Editor</span></span>
* <span data-ttu-id="1d46e-129">**パイロット** -水平モードを切り替えて、6dof フライトツールを生成する機能</span><span class="sxs-lookup"><span data-stu-id="1d46e-129">**Pilot** - ability to toggle fly mode and spawn the 6DOF flight tool</span></span>
* <span data-ttu-id="1d46e-130">**Megaphone_only** -世界中のどこでもユーザーの耳に話す機能</span><span class="sxs-lookup"><span data-stu-id="1d46e-130">**Megaphone_only** - ability to speak into users' ears wherever they are in the World</span></span>
* <span data-ttu-id="1d46e-131">**Showcase_new_sdk** -MRE sdk アプリを生成する機能</span><span class="sxs-lookup"><span data-stu-id="1d46e-131">**Showcase_new_sdk** - ability to spawn MRE SDK apps</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="1d46e-132">トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="1d46e-132">Troubleshooting</span></span>

<span data-ttu-id="1d46e-133">**ロールを削除できますか。**</span><span class="sxs-lookup"><span data-stu-id="1d46e-133">**Can I delete roles?**</span></span>
<span data-ttu-id="1d46e-134">ここではフォームからではなく、help.altvr.com でファイルを作成して Support request、自動的に処理します。</span><span class="sxs-lookup"><span data-stu-id="1d46e-134">Not from the form right now so file a Support request at help.altvr.com and we'll take care of it for you</span></span>

<span data-ttu-id="1d46e-135">**別の環境からインポートしている場合、役割はコピーされますか。**</span><span class="sxs-lookup"><span data-stu-id="1d46e-135">**Are roles copied when a World is importing from another?**</span></span>
<span data-ttu-id="1d46e-136">いいえ、ロールはコピーされません</span><span class="sxs-lookup"><span data-stu-id="1d46e-136">No, roles aren't copied</span></span>