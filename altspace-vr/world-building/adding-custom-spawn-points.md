---
title: カスタム生成ポイントの追加
description: カスタムの生成ポイントを作成、追加、およびトラブルシューティングする方法について説明します。
ms.date: 03/11/2021
ms.topic: article
keywords: spawnpoint, トラブルシューティング
ms.openlocfilehash: 0f53bdc229eb21e50edef34981c592556236fc55
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212818"
---
# <a name="adding-custom-spawn-points"></a><span data-ttu-id="ca05c-104">カスタム生成ポイントの追加</span><span class="sxs-lookup"><span data-stu-id="ca05c-104">Adding custom spawn points</span></span>

<span data-ttu-id="ca05c-105">世界に入るユーザーは、世界中の場所 (0, 0, 0) で **開始または** 表示されます。</span><span class="sxs-lookup"><span data-stu-id="ca05c-105">People entering your World will **spawn** or appear at the origin, position (0,0,0), when they enter your World.</span></span> <span data-ttu-id="ca05c-106">ただし、1つまたは複数の生成ポイントを追加することもできます。その場合は、ユーザーが城の入口から開始するようにします。</span><span class="sxs-lookup"><span data-stu-id="ca05c-106">However, you can add one or more Spawn Points if you want to, say, have people start at the entrance to your castle.</span></span> <span data-ttu-id="ca05c-107">複数の生成ポイントを指定すると、他のユーザーが入力し、オリジンが含まれない場合は、ランダムに選択されます。</span><span class="sxs-lookup"><span data-stu-id="ca05c-107">If you specify multiple Spawn Points, one will be randomly chosen whenever someone enters and the origin won't be included.</span></span> <span data-ttu-id="ca05c-108">世界中のエディターが有効になっている世界またはイベントへのポイントの生成を管理できます。</span><span class="sxs-lookup"><span data-stu-id="ca05c-108">You can manage Spawn Points to any World or Event where your World Editor is enabled.</span></span> <span data-ttu-id="ca05c-109">だれがどこにいるか (位置) とその方向 (回転) を制御します。</span><span class="sxs-lookup"><span data-stu-id="ca05c-109">You control where people spawn (position) and what direction they'll be facing (rotation).</span></span> <span data-ttu-id="ca05c-110">生成ポイントは編集モードでのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="ca05c-110">Spawn Points will only be visible in Edit Mode.</span></span> 

1. <span data-ttu-id="ca05c-111">どこにいるかについては、どこにいるかをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="ca05c-111">Go near the spot where you want people to spawn.</span></span> <span data-ttu-id="ca05c-112">**ワールドエディターを開き > 基本** を確認し、**ロックの回転** がチェックされることを確認します。</span><span class="sxs-lookup"><span data-stu-id="ca05c-112">Open **World Editor > Basics** and make sure **Lock Rotation** is checked.</span></span> <span data-ttu-id="ca05c-113">[ **生成ポイント** ] を選択して作成します。</span><span class="sxs-lookup"><span data-stu-id="ca05c-113">Select **Spawn Point** to create one.</span></span> <span data-ttu-id="ca05c-114">適切な位置に移動します。</span><span class="sxs-lookup"><span data-stu-id="ca05c-114">Move it to the exact position you want:</span></span>

![ワールドエディターの基本ウィンドウを開く](images/spawn-points-img-01.png)

2. <span data-ttu-id="ca05c-116">生成ポイントの設定アイコンを選択し、 **回転 > X** と **回転 > Z** の両方が **0** であることを確認します。</span><span class="sxs-lookup"><span data-stu-id="ca05c-116">Select on the settings icon for the Spawn Point and make sure **Rotation > X** and **Rotation > Z** are both **0**.</span></span> <span data-ttu-id="ca05c-117">**8.537777745 e-07** のような小さな数値の場合も問題ありません。</span><span class="sxs-lookup"><span data-stu-id="ca05c-117">If they are small numbers like **8.537777745E-07**, that's fine too.</span></span> <span data-ttu-id="ca05c-118">これは、浮動小数点数がどのように処理されるかということです。</span><span class="sxs-lookup"><span data-stu-id="ca05c-118">That's a quirk of how floating point numbers are handled:</span></span>

![ワールドエディター設定の更新プログラムの生成ポイント](images/spawn-points-img-02.png)

3. <span data-ttu-id="ca05c-120">**メニュー > 設定 > 全般 > 再入力してスペースを再入力 > 再入力してください**。</span><span class="sxs-lookup"><span data-stu-id="ca05c-120">Reenter your World via **Menu > Settings > General > Reenter Space > Re-Enter**</span></span>
4. <span data-ttu-id="ca05c-121">新しい生成ポイントでを生成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ca05c-121">You should spawn at your new Spawn Point!</span></span>
5. <span data-ttu-id="ca05c-122">ユーザーが別の方向に表示されるようにするには、生成ポイントの設定を選択し、 **回転 > Y** のみを設定します。</span><span class="sxs-lookup"><span data-stu-id="ca05c-122">If you want people to face a different direction, select the settings for the Spawn Point and set **Rotation > Y** only.</span></span> <span data-ttu-id="ca05c-123">Y を180に設定し、X と Z を0に設定します (警告: X および Z は高度なので、人間が病気になる可能性があります)。</span><span class="sxs-lookup"><span data-stu-id="ca05c-123">Try setting Y to 180 and both X and Z to 0 (Warning: X and Z are advanced may make people sick).</span></span> <span data-ttu-id="ca05c-124">[ **確認** ] を選択し、世界を再入力します。</span><span class="sxs-lookup"><span data-stu-id="ca05c-124">Then select **Confirm** and reenter the World.</span></span> <span data-ttu-id="ca05c-125">これにより、逆方向の接続が発生します。</span><span class="sxs-lookup"><span data-stu-id="ca05c-125">That should spawn you facing the opposite direction.</span></span> 

## <a name="troubleshooting"></a><span data-ttu-id="ca05c-126">トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="ca05c-126">Troubleshooting</span></span>

<span data-ttu-id="ca05c-127">**まだ配信元での開発者の方は、**</span><span class="sxs-lookup"><span data-stu-id="ca05c-127">**People still spawning at the origin?**</span></span>
    * <span data-ttu-id="ca05c-128">生成ポイントが地表または表面より少し上にあることを確認します。</span><span class="sxs-lookup"><span data-stu-id="ca05c-128">Make sure your Spawn Points are slightly above the ground or surface.</span></span> <span data-ttu-id="ca05c-129">生成ポイントが他のオブジェクトと重なっている場合は、既定の場所であるオリジンでが生成されます。</span><span class="sxs-lookup"><span data-stu-id="ca05c-129">If the Spawn Point is overlapping other objects, people spawn at the default location, the origin.</span></span> <span data-ttu-id="ca05c-130">これは、オブジェクト内の生成ポイントとユーザーの高さが異なる場合に発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ca05c-130">This can happen if the Spawn Point inside an object and the height of person varies.</span></span> 
    * <span data-ttu-id="ca05c-131">**メニュー > 設定** を使用して世界をリセットしてみてください > > 中程度の領域をリセットしてください</span><span class="sxs-lookup"><span data-stu-id="ca05c-131">Try resetting your World via **Menu > Settings > Moderate > Reset Space**</span></span>

<span data-ttu-id="ca05c-132">**複数の生成ポイントがあっても、同じ場所に生成されていますか。**</span><span class="sxs-lookup"><span data-stu-id="ca05c-132">**Have multiple Spawn Points but still spawning in the same place?**</span></span>
<span data-ttu-id="ca05c-133">Unlucky があるかもしれません。</span><span class="sxs-lookup"><span data-stu-id="ca05c-133">You might be unlucky--it's random after all.</span></span> <span data-ttu-id="ca05c-134">エラーが発生したことを前提として、少なくとも5回の再入を試してください。</span><span class="sxs-lookup"><span data-stu-id="ca05c-134">Try a few reentering at least five times before assuming there's an error.</span></span> 

<span data-ttu-id="ca05c-135">**人間が不快になっているか、頭が傾いている\*\*\*\*ロックのローテーション** を確認するか、回転に X と Z の値を設定し忘れた可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ca05c-135">**People are uncomfortable or their head is tilted** You may have forgotten to check **Lock Rotation** or set the X and Z value for Rotation.</span></span> <span data-ttu-id="ca05c-136">通常は、風変わりな世界を構築する場合を除き、0に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ca05c-136">Those should usually be set to 0 unless you're building an exotic World.</span></span> 

<span data-ttu-id="ca05c-137">**ユーザーが起動すると、**</span><span class="sxs-lookup"><span data-stu-id="ca05c-137">**People falling when they spawn?**</span></span>
<span data-ttu-id="ca05c-138">オブジェクトの上にある、生成ポイントの位置が高すぎないように設定してください。</span><span class="sxs-lookup"><span data-stu-id="ca05c-138">Don't set the Spawn Point position too high above an object.</span></span> <span data-ttu-id="ca05c-139">非常に大きくなると、元の位置に戻ります。</span><span class="sxs-lookup"><span data-stu-id="ca05c-139">If they fall too far, they'll be respawned at the origin.</span></span>