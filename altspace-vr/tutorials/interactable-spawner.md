---
title: Interactables Spawner の使用
description: Interactables spawner を作成、使用、カスタマイズする方法について説明します。これらの項目は、Altspaces Evr スペースに配置します。
ms.date: 02/10/2021
ms.topic: article
keywords: spawner、相互作用、カスタマイズ
ms.openlocfilehash: 7f4b87591b2e11b2084af4d2bf83748ed51fd193
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2021
ms.locfileid: "107213551"
---
# <a name="using-the-interactables-spawner"></a><span data-ttu-id="c3feb-104">Interactables Spawner の使用</span><span class="sxs-lookup"><span data-stu-id="c3feb-104">Using the Interactables Spawner</span></span>

<span data-ttu-id="c3feb-105">Interactables Spawner を使用すると、イベント、世界、またはホームスペースに対話型項目を配置できます。</span><span class="sxs-lookup"><span data-stu-id="c3feb-105">The Interactables Spawner allows you to place interactable items in your event, world, or home-space.</span></span> <span data-ttu-id="c3feb-106">この機能は、現在、 [早期アクセスプログラム](../world-building/early-access.md) の一部であり、メインメニューを使用して選択しない限り利用できません。</span><span class="sxs-lookup"><span data-stu-id="c3feb-106">This feature is currently part of our [Early Access Program](../world-building/early-access.md) and won't be available unless you've opted in through your Main Menu.</span></span>

> [!NOTE]
> <span data-ttu-id="c3feb-107">この機能のパイロット処理は継続していますが、内部のテーブルが多すぎると環境やイベントのパフォーマンスに影響する可能性があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="c3feb-107">While we continue to pilot this feature please be aware that spawning too many interactables may affect the performance of your environment or event.</span></span> 

## <a name="creating-an-interactable"></a><span data-ttu-id="c3feb-108">対話型の作成</span><span class="sxs-lookup"><span data-stu-id="c3feb-108">Creating an interactable</span></span>

<span data-ttu-id="c3feb-109">オブジェクトを対話型オブジェクトに変換するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="c3feb-109">To turn your object into an interactable object:</span></span>

1. <span data-ttu-id="c3feb-110">オブジェクトをスペースに配置します。</span><span class="sxs-lookup"><span data-stu-id="c3feb-110">Place the object in your space.</span></span>
2. <span data-ttu-id="c3feb-111">次に、[オブジェクト] ボックスの一覧でエントリを探し、その横にある **歯車アイコン** を選択して設定を開きます。</span><span class="sxs-lookup"><span data-stu-id="c3feb-111">Then, find the entry in the object list, and select the **gear icon** next to it to open its settings:</span></span>

![オブジェクトリストが強調表示された状態で開いているワールドエディター](images/interactables-spawner-img-01.png)

<span data-ttu-id="c3feb-113">[設定] ページで、 **"object spawner"** という新しいチェックボックスが表示されます。このチェックボックスを使用して、対話型オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c3feb-113">On the settings page you’ll find a new checkbox **“Object spawner“**, which is used to make it an interactable object.</span></span>

1. <span data-ttu-id="c3feb-114">チェックボックスをオンにして、[ **確認**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c3feb-114">Check the box and select **confirm**.</span></span>
2. <span data-ttu-id="c3feb-115">編集モードでは、空間内のオブジェクトの生成場所を移動できます。</span><span class="sxs-lookup"><span data-stu-id="c3feb-115">While in edit mode, you can move around the object’s spawn location in the space.</span></span>
3. <span data-ttu-id="c3feb-116">**編集モードを終了** して、項目の操作を有効にします。</span><span class="sxs-lookup"><span data-stu-id="c3feb-116">**Exit edit mode** to enable item interaction.</span></span>

![Altworkplace Evr アプリで開かれている [更新アイテム] ウィンドウ](images/interactables-spawner-img-02.png)

## <a name="other-customizations"></a><span data-ttu-id="c3feb-118">その他のカスタマイズ</span><span class="sxs-lookup"><span data-stu-id="c3feb-118">Other customizations</span></span>

<span data-ttu-id="c3feb-119">オブジェクトのプロパティに戻ったときに **"object spawner"** を有効にすると、生成されたオブジェクトの動作に適用できる追加の設定が表示されます。</span><span class="sxs-lookup"><span data-stu-id="c3feb-119">After enabling **“Object spawner”** when you go back into the properties for that object, there will be an extra setting you can apply to how the spawned object behaves.</span></span>

> [!NOTE]
> <span data-ttu-id="c3feb-120">対話型 object scale: オブジェクトの取得時にオブジェクトのスケールを設定します。 "Scale" と比較します。これは、オブジェクトを初めて選択する前に、世界でどのように表示するかのスケールです。</span><span class="sxs-lookup"><span data-stu-id="c3feb-120">Interactable object scale: This sets the scale of the object when it gets picked up, compared to “Scale” which is the scale of how the object appears in the world prior to picking it up for the first time.</span></span>

<span data-ttu-id="c3feb-121">キットの開発者は、altの実行中にキットに加えられた変更が有効にならないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="c3feb-121">Kit makers may notice that changes to your Kit while AltspaceVR is running won't take effect until you restart AltspaceVR.</span></span>

<span data-ttu-id="c3feb-122">最近、[**ワールドキットの再読み込み**] というボタンを [中 **程度の設定**] タブの下に追加しました。</span><span class="sxs-lookup"><span data-stu-id="c3feb-122">Recently we’ve added a button under the **Moderate Settings** tab called **Reload Worlds Kits**.</span></span> <span data-ttu-id="c3feb-123">このボタンをクリックすると、スペースを再入力するだけで、すべてのキットを再度読み込むことができます。これにより、Altspace Evr の間に更新された新しいバージョンのキットのみがダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="c3feb-123">Clicking this button causes (just you) to reenter the space, reloading all Kits again, which will download only new versions of the Kits that have been updated while you were in AltspaceVR.</span></span>

![[中程度の設定] パネルを [Altworkplace Evr] アプリで開く](images/interactables-spawner-img-03.png)