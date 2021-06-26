---
title: ワールド ロールの付与
description: ロールと能力システムについて学習し、AltspaceVR の世界でユーザーにロールを与える手順を説明します。
ms.date: 04/14/2021
ms.topic: article
keywords: roles
ms.openlocfilehash: 3a1d0f138b29fe545f52d851ff00062f156a860e
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923196"
---
# <a name="granting-world-roles"></a><span data-ttu-id="c21c7-104">ワールド ロールの付与</span><span class="sxs-lookup"><span data-stu-id="c21c7-104">Granting world roles</span></span>

<span data-ttu-id="c21c7-105">Altspace には、Roles and Abilities システムがあります。</span><span class="sxs-lookup"><span data-stu-id="c21c7-105">Altspace has a Roles and Abilities system.</span></span> <span data-ttu-id="c21c7-106">各ユーザーは複数のロールを持つ可能性があります。ロールは、その場所によって異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="c21c7-106">Each person can have multiple roles and their roles can be different depending on where they are.</span></span> <span data-ttu-id="c21c7-107">各ロールは、1 つ以上の機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="c21c7-107">Each role, in turn, gives you one or more abilities.</span></span> <span data-ttu-id="c21c7-108">たとえば、独自のイベントに参加すると、ホストロールとモデレーター ロールが **自動的** に **受信** されます。</span><span class="sxs-lookup"><span data-stu-id="c21c7-108">For example, when you're in your own event, you automatically receive the **host** and **moderator** roles.</span></span> <span data-ttu-id="c21c7-109">この 2 つのロールを使用すると、ユーザーを解放し、ステージに立ち、おそらく confetti をリリースすることができます。</span><span class="sxs-lookup"><span data-stu-id="c21c7-109">With those two roles you can kick unruly users, be on stage, and maybe release the confetti.</span></span>

1. <span data-ttu-id="c21c7-110">ワールドを編集し、コンテキスト ロールの右側の列を確認 **します** ([ワールドを管理する方法](managing-worlds.md))</span><span class="sxs-lookup"><span data-stu-id="c21c7-110">Edit your World and look over to the right column for **Contextual Roles** ([How to manage Worlds](managing-worlds.md))</span></span>

![ワールドのコンテキスト ロール セクションでのロールの変更](images/granting-roles.png)

2. <span data-ttu-id="c21c7-112">この World **に対して** 特定の **ロールを** 特定のユーザーに付与する場合は、[コンテキスト ロール] フィールドの [ユーザーの追加] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="c21c7-112">Click **Add User** under the **Contextual Roles** field if you want to grant specific roles to specific users just for this World.</span></span> <span data-ttu-id="c21c7-113">たとえば、ホスト モデレーター を指定する場合は、上記を追加して [保存  +  ] を **選択します**。</span><span class="sxs-lookup"><span data-stu-id="c21c7-113">For example, if you want to give me **host** + **moderator**, you would add the above and select **Save**.</span></span> <span data-ttu-id="c21c7-114">形式は **ユーザー** 名、ユーザー名は大文字と小文字が区別されません。ドロップダウン メニュー **Terraformer** からロールを選択し、[ユーザーの追加] を複数回クリックしてユーザーを追加し続け、[更新] **をクリックします**。</span><span class="sxs-lookup"><span data-stu-id="c21c7-114">The format is **username**, username is case-insensitive, choose the role from the dropdown menu **Terraformer**, click Add User multiple times to keeping adding more users and then click **Update**.</span></span>

* <span data-ttu-id="c21c7-115">Altspace で変更を有効にするには、すべてのユーザーが新しいロールを持つユーザーに再び世界に再び追加したり、新しいロールを持つ各ユーザーに再び追加したりする必要があります。</span><span class="sxs-lookup"><span data-stu-id="c21c7-115">In order for the change to take effect in Altspace, you should Reset Space the world forcing everyone to rejoin or have each user with a new role rejoin the world.</span></span>

3. <span data-ttu-id="c21c7-116">World に **参加しているすべてのロールに** ロールを付与する場合は、[ **In VR** ] セクションの [既定のコンテキスト ロール] フィールドを編集します。</span><span class="sxs-lookup"><span data-stu-id="c21c7-116">Edit the **Default Contextual Roles** field, under the **In VR** section, if you want to grant a role to every one that joins your World.</span></span> <span data-ttu-id="c21c7-117">たとえば、ユーザーが離れた場所で互いに聞こえ合うので、ユーザーが移動してメガフォンを使用する場合は、次のコードを追加します。</span><span class="sxs-lookup"><span data-stu-id="c21c7-117">For example, if you want to let people fly and use the megaphone so they can hear each other while far part, add the following:</span></span>

```
pilot,megaphone_only
```

<span data-ttu-id="c21c7-118">[更新] を **選択した** 後、[世界の領域のリセット] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c21c7-118">After you select **Update**, Reset Space in the World.</span></span> <span data-ttu-id="c21c7-119">これは、このワールドにのみ影響します。</span><span class="sxs-lookup"><span data-stu-id="c21c7-119">This will only affect this World.</span></span> <span data-ttu-id="c21c7-120">ロールを Universe 全体に付与する場合は、宇宙で同じフィールドを編集します。</span><span class="sxs-lookup"><span data-stu-id="c21c7-120">If you want to grant roles to an entire Universe, edit the same fields on the Universe.</span></span> <span data-ttu-id="c21c7-121">イベントの場合も同様です。イベント内のすべてのユーザーにこれらのロールを割り当てる場合は、これをイベント自体の既定のコンテックス ロールに追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c21c7-121">The same goes for events, if you want everyone in your event to have these roles you'll need to add this to the **Default Contexual Roles** of the event itself.</span></span>

## <a name="roles"></a><span data-ttu-id="c21c7-122">ロール</span><span class="sxs-lookup"><span data-stu-id="c21c7-122">Roles</span></span>

* <span data-ttu-id="c21c7-123">**Megaphone_only** - 世界中のどこからでもユーザーの耳を聞く機能</span><span class="sxs-lookup"><span data-stu-id="c21c7-123">**Megaphone_only** - ability to speak into users' ears wherever they are in the World</span></span>
* <span data-ttu-id="c21c7-124">**Moderator** - オバム **を維持するための kick** のような機能</span><span class="sxs-lookup"><span data-stu-id="c21c7-124">**Moderator** - abilities like **kick** to maintain decorum</span></span>
* <span data-ttu-id="c21c7-125">**パイロット** - フライ モードを切り替え、6DOF フライト ツールを生成する機能</span><span class="sxs-lookup"><span data-stu-id="c21c7-125">**Pilot** - ability to toggle fly mode and spawn the 6DOF flight tool</span></span>
* <span data-ttu-id="c21c7-126">**ホスト** - ステージに立つ、メガフォンを持つなど、機能</span><span class="sxs-lookup"><span data-stu-id="c21c7-126">**Host** - abilities like being able to be on stage, have megaphone</span></span>
* <span data-ttu-id="c21c7-127">**Terraformer** - ワールド エディターを使用する機能に関する詳細 ( イベント、ワールド、グループ、[および AltspaceVR](../getting-started/roles.md)のロール)</span><span class="sxs-lookup"><span data-stu-id="c21c7-127">**Terraformer** - ability to use the World Editor More information about ([Roles in events, worlds, groups, and in AltspaceVR](../getting-started/roles.md))</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="c21c7-128">トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="c21c7-128">Troubleshooting</span></span>

<span data-ttu-id="c21c7-129">**ロールを削除できますか?**</span><span class="sxs-lookup"><span data-stu-id="c21c7-129">**Can I delete roles?**</span></span>
<span data-ttu-id="c21c7-130">はい、ワールドを編集し **、削除する** ロールの下にある [削除] をクリックして、[更新] をクリック **します**</span><span class="sxs-lookup"><span data-stu-id="c21c7-130">Yes, edit your world, click **Remove** below the role you'd like to delete and click **Update**</span></span>

<span data-ttu-id="c21c7-131">**World が別のワールドからインポートするときにロールはコピーされますか?**</span><span class="sxs-lookup"><span data-stu-id="c21c7-131">**Are roles copied when a World is importing from another?**</span></span>
<span data-ttu-id="c21c7-132">いいえ、ロールはコピーされません</span><span class="sxs-lookup"><span data-stu-id="c21c7-132">No, roles aren't copied</span></span>