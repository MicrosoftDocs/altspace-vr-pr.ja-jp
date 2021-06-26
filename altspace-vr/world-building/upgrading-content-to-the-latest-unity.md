---
title: 最新の Unity バージョンにコンテンツを更新しています
description: 最新バージョンの Unity にコンテンツを更新する方法について説明します。
ms.date: 06/4/2021
ms.topic: article
keywords: キット, ワールド, unity, 更新, シェーダー, アップローダー, トラブルシューティング
ms.openlocfilehash: f8a805c4b3350f2c97c43d3d48c35733ec7e9710
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2021
ms.locfileid: "112961254"
---
# <a name="updating-content-to-the-latest-unity-version"></a><span data-ttu-id="5c4e3-104">最新の Unity バージョンにコンテンツを更新しています</span><span class="sxs-lookup"><span data-stu-id="5c4e3-104">Updating Content to the Latest Unity Version</span></span>

## <a name="moving-to-unity-202039"></a><span data-ttu-id="5c4e3-105">Unity 2020.3.9 への移行</span><span class="sxs-lookup"><span data-stu-id="5c4e3-105">Moving to Unity 2020.3.9</span></span>

<span data-ttu-id="5c4e3-106">現時点では、Alt2020.3.9 Evr は最新バージョンの Unity () にアップグレードされています。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-106">Starting today, AltspaceVR has upgraded to a recent version of Unity (2020.3.9).</span></span> <span data-ttu-id="5c4e3-107">いくつかのパフォーマンスの向上に加えて、この更新プログラムは、今後導入される予定の機能を対象としています。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-107">In addition to some performance improvements, this update future-proofs us for forthcoming features that we're excited to incorporate.</span></span> <span data-ttu-id="5c4e3-108">この変更は、既存のすべてのコンテンツと互換性がある必要があります。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-108">This change should be compatible with all existing content.</span></span> <span data-ttu-id="5c4e3-109">そうでない場合は、サポートにお問い合わせください: altvr.com/support</span><span class="sxs-lookup"><span data-stu-id="5c4e3-109">If it isn't, feel free to contact support: altvr.com/support</span></span>

<span data-ttu-id="5c4e3-110">この2020.3.9 への移行は、ユーザーが生成したコンテンツに影響を与えていませんが、数週間後に、 [ユーザーがコンテンツを更新する必要がある]( https://docs.unity3d.com/Manual/SinglePassStereoRendering.html)Alt evr のステレオレンダリングモードに変更を加えています。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-110">Though this move to 2020.3.9 hasn't affected user-generated content, in a few weeks we're making a change to AltspaceVR's [stereo rendering mode that will require users to update their content]( https://docs.unity3d.com/Manual/SinglePassStereoRendering.html).</span></span> <span data-ttu-id="5c4e3-111">この [1 回のパスのインスタンス](https://docs.unity3d.com/Manual/SinglePassInstancing.html) へのアップグレードにより、世界で大幅なパフォーマンス向上が可能になります。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-111">This upgrade to [Single Pass Instancing](https://docs.unity3d.com/Manual/SinglePassInstancing.html) will allow for significant performance improvements in your worlds.</span></span> <span data-ttu-id="5c4e3-112">この新しいビルドでは、2019.4 以前のコンテンツとの下位互換性がサポートされなくなることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-112">Keep in mind that this new build will no longer support backwards-compatibility with content from 2019.4 and older.</span></span> <span data-ttu-id="5c4e3-113">すべての作成者が所有するコンテンツをできるだけ早く更新して、重大な変更を回避することは緊急です。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-113">It's urgent that all creator-owned content is updated as soon as possible to avoid breaking changes.</span></span> <span data-ttu-id="5c4e3-114">以下のガイドに従ってコンテンツを更新し、Unity 2020.3.9 でシングルパスのインスタンス化にスムーズに移行できるようにします。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-114">Follow the guide below to update your content and ensure a smooth transition to Single Pass Instancing on Unity 2020.3.9.</span></span>

> [!NOTE]
> <span data-ttu-id="5c4e3-115">他のユーザーが所有しているコンテンツを定期的に使用していて、あなたと共有している場合は、世界/キットの所有者に連絡して、コンテンツの更新を計画していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-115">If you are regularly using content that is owned by someone else and has been shared with you, contact the world/kit owner and make sure they are planning to update their content.</span></span>

> <span data-ttu-id="5c4e3-116">コンテンツ作成者であり、不明な点やサポートが必要な場合は、サポートチーム () にお問い合わせください。 altvr.com/support</span><span class="sxs-lookup"><span data-stu-id="5c4e3-116">If you are a content creator and you have questions or require assistance, please contact our support team for help: altvr.com/support</span></span>

## <a name="testing-your-spi-content"></a><span data-ttu-id="5c4e3-117">SPI コンテンツのテスト</span><span class="sxs-lookup"><span data-stu-id="5c4e3-117">Testing your SPI content</span></span>

<span data-ttu-id="5c4e3-118">次のプレビューバージョンの Altを使用して、VR で新しく更新されたコンテンツをテストします。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-118">Use the following preview versions of AltspaceVR to test your newly updated content in VR.</span></span> <span data-ttu-id="5c4e3-119">プレビューバージョンはテストのみを目的としており、プラットフォームの一般的な使用には使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-119">The preview versions are for testing purposes only, and shouldn't be used for a general use of the platform.</span></span>

* [<span data-ttu-id="5c4e3-120">Windows Mixed Reality の Altworkplace Evr SPI Preview</span><span class="sxs-lookup"><span data-stu-id="5c4e3-120">AltspaceVR SPI Preview for Windows Mixed Reality</span></span>](https://aka.ms/AvrSpiMr)
* [<span data-ttu-id="5c4e3-121">SteamVR の Altworkplace Evr SPI Preview</span><span class="sxs-lookup"><span data-stu-id="5c4e3-121">AltspaceVR SPI Preview for SteamVR</span></span>](https://aka.ms/AvrSpiSteam)
* [<span data-ttu-id="5c4e3-122">Oculus Rift の Altworkplace Evr SPI Preview</span><span class="sxs-lookup"><span data-stu-id="5c4e3-122">AltspaceVR SPI Preview for Oculus Rift</span></span>](https://aka.ms/AvrSpiRift)

> <span data-ttu-id="5c4e3-123">注: PC VR のプレビュー版のみが提供されています。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-123">Note: Only PC VR previews have been provided.</span></span> <span data-ttu-id="5c4e3-124">シングルパスでインスタンス化されたレンダリングは Android では使用できません。 Mac などの VR 以外のプラットフォームでは必要ありません。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-124">Single pass instanced rendering is not available on Android, and is not needed on non-VR platforms like Mac.</span></span> <span data-ttu-id="5c4e3-125">そのため、これらのデバイスをテストするには、一般リリースバージョンを使用できます。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-125">Thus, you can use the general release version to test these devices.</span></span>


## <a name="storecompatibilitycheck"></a><span data-ttu-id="5c4e3-126">ストア互換性チェック</span><span class="sxs-lookup"><span data-stu-id="5c4e3-126">Store Compatibility Check</span></span>

<span data-ttu-id="5c4e3-127">Unity 2020.3.9 へのアップグレードは、ヘッドセットとストアのビルドの互換性にも影響します。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-127">The upgrade to Unity 2020.3.9 will also affect headset and store-build compatibility.</span></span> <span data-ttu-id="5c4e3-128">これで、ヘッドセットと互換性のあるストアから Altをダウンロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-128">It's now a requirement that you download AltspaceVR from the store that is compatible with your headset.</span></span> <span data-ttu-id="5c4e3-129">例として、WinMR または Oculus のヘッドセットの場合は、Windows ストアまたは Oculus ストアから、それぞれ Alt をダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-129">As an example: For a WinMR or Oculus headset, download AltspaceVR from the Windows Store or Oculus Store, respectively.</span></span> <span data-ttu-id="5c4e3-130">Windows Mixed Reality ユーザーは、Windows ストアから AltOculus をダウンロードし、ストリームからのユーザーの SteamVR ユーザーと、Oculus ストアの Rift ユーザーをダウンロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-130">Windows Mixed Reality users should download AltspaceVR from the Windows Store, SteamVR users from Steam, and Oculus Rift users from the Oculus Store.</span></span>

## <a name="altspacevr-uploader-v090-upgrade-guide"></a><span data-ttu-id="5c4e3-131">Alt0.9.0 Evr アップローダー v のアップグレードガイド</span><span class="sxs-lookup"><span data-stu-id="5c4e3-131">AltspaceVR Uploader v0.9.0 Upgrade Guide</span></span> 

<span data-ttu-id="5c4e3-132">アップローダー0.9 は、以前のバージョンのアップローダーとは異なる形でパッケージ化されています。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-132">Uploader 0.9 is packaged differently than previous versions of the Uploader.</span></span> <span data-ttu-id="5c4e3-133">このパッケージの変更と同時に、新しいアップローダーには新しいバージョンの Unity が必要です。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-133">Simultaneous with this packaging change, the new Uploader requires a new version of Unity.</span></span> <span data-ttu-id="5c4e3-134">このガイドは、関係するすべてのユーザーに対して、このアップグレードプロセスをより円滑かつ安全にすることを目的としています。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-134">This guide is intended to make this upgrade process smoother and safer for all who are involved.</span></span>

1. <span data-ttu-id="5c4e3-135">**プロジェクトのバックアップ** -プロジェクトディレクトリ全体のコピーを作成し、安全な場所に配置します。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-135">**BACK UP YOUR PROJECT** - Create a copy of your entire project directory, and put it somewhere safe.</span></span> <span data-ttu-id="5c4e3-136">このアップグレードは破壊的なアップグレードであるため、完了後に Unity 2019.4 のバンドルを作成またはアップロードすることはできません。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-136">This upgrade is a destructive upgrade, so you won't be able to create or upload bundles for Unity 2019.4 after you complete it.</span></span> <span data-ttu-id="5c4e3-137">このアップグレード中に問題が発生した場合は、プロジェクトのクリーンコピーが必要になります。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-137">If you come across any problems during this upgrade, you'll NEED a clean copy of your project to fall back on.</span></span> <span data-ttu-id="5c4e3-138">また、2020.3.9 に正式にアップグレードする前に、ライブキットまたはテンプレートを更新する必要もあります。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-138">You'll also need it to update any live kits or templates before AltspaceVR officially upgrades to Unity 2020.3.9.</span></span>

2. <span data-ttu-id="5c4e3-139">**古いアップローダーを削除** します。 Unity が閉じている場合は、次のファイル/フォルダーを削除し、それに対応するメタファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-139">**REMOVE OLD UPLOADER** - With Unity closed, delete the following files/folders, and it's corresponding .meta files:</span></span>

    ```console
    * Assets/Altspace

    * Assets/Plugins

    * Assets/Prefabs/test-folder, Readme.txt

    * Assets/Resources/bg.jpeg, bg2.jpeg, logo.png, UserPreferences.asset

    * Assets/DFloor_v004.fbx

    * Library (This is a Unity system folder, not an Uploader folder. Delete it anyway, and let it be rebuilt during the upgrade.)
    ```

3. <span data-ttu-id="5c4e3-140">[**エンジンバージョンのダウンロード**]-unity ハブを開き、unity 2020.3.9 をインストールします (または、[ここをクリックし](https://unity3d.com/ru/unity/whats-new/2020.3.9)て直接インストールします)。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-140">**DOWNLOAD ENGINE VERSION** - Open the Unity Hub, and install Unity 2020.3.9 (or [click here](https://unity3d.com/ru/unity/whats-new/2020.3.9) to install directly).</span></span>

4. <span data-ttu-id="5c4e3-141">[**プロジェクトのアップグレード**]: unity 2020.3.9 で、クリーンされたプロジェクトを開き、unity がプロジェクトをアップグレードできるようにします。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-141">**UPGRADE PROJECT** - Open your cleaned project in Unity 2020.3.9, and allow Unity to upgrade your project.</span></span>

5. <span data-ttu-id="5c4e3-142">(PC のみ) **MIXED REALITY 機能ツールをダウンロード** する-手順に従って、アップローダーパッケージのインストールの管理に使用する [Mixed reality 機能ツール](/windows/mixed-reality/develop/unity/welcome-to-mr-feature-tool)をダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-142">(PC Only) **DOWNLOAD MIXED REALITY FEATURE TOOL** - Follow the instructions to download the [Mixed Reality Feature Tool](/windows/mixed-reality/develop/unity/welcome-to-mr-feature-tool), which you'll use to manage the installation of the Uploader package.</span></span>

6. <span data-ttu-id="5c4e3-143">**アップローダーをインストール** します。 MR 機能ツールを使用して Unity プロジェクトを選択し、Alt Evr アップローダー機能を追加します (alt の見出しの下)。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-143">**INSTALL THE UPLOADER** - Use the MR Feature Tool to select your Unity project, and add the AltspaceVR Uploader feature (under the AltspaceVR heading).</span></span> <span data-ttu-id="5c4e3-144">ツールの指示に従います。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-144">Follow the instructions in the tool.</span></span>

<span data-ttu-id="5c4e3-145">MacOS では、 [レジストリ](https://dev.azure.com/aipmr/MixedReality-Unity-Packages/_packaging?_a=package&feed=Unity-packages&package=com.microsoft.altspacevr_uploader&protocolType=Npm&version=0.9.0&view=versions)から最新バージョンを手動でダウンロードし、Unity エディターのパッケージマネージャー内からインストールします (Windows > パッケージマネージャー > + > パッケージを Tar から追加します)。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-145">On macOS, manually download the latest version from the [registry](https://dev.azure.com/aipmr/MixedReality-Unity-Packages/_packaging?_a=package&feed=Unity-packages&package=com.microsoft.altspacevr_uploader&protocolType=Npm&version=0.9.0&view=versions), and install it from within the Unity Editor's package manager (Windows > Package Manager > + > Add package from tarball).</span></span>

<span data-ttu-id="5c4e3-146">パッケージのインポートが完了したら、使い慣れたアップローダーウィンドウを [Alt] メニュー項目で使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-146">Once the package finishes importing, the familiar Uploader window should be available in the AltspaceVR menu item.</span></span>

## <a name="troubleshooting-tips"></a><span data-ttu-id="5c4e3-147">トラブルシューティングのヒント</span><span class="sxs-lookup"><span data-stu-id="5c4e3-147">Troubleshooting Tips</span></span>

1. <span data-ttu-id="5c4e3-148">WinMR ヘッドセットでコントローラーまたは入力の問題が発生している場合は、プレゼンスセンサーに適切に参加するために、ヘッドに設置されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-148">If you're having controller or input issues on your WinMR headset, ensure it's positioned on your head to properly engage the presence sensor.</span></span> <span data-ttu-id="5c4e3-149">これは既知の問題であり、マイクロソフトはその解決に積極的に取り組んでいます。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-149">This is a known issue and Microsoft is actively working to resolve it.</span></span>

2. <span data-ttu-id="5c4e3-150">ヘッドセットとストアとビルドの互換性を確認します。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-150">Check your headset and store-build compatibility.</span></span> <span data-ttu-id="5c4e3-151">たとえば、WinMR ヘッドセットを使用している場合は、Windows ストアを通じて Altを取得したことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-151">If you're using a WinMR headset, for example, make sure that your AltspaceVR build was acquired through the Windows Store.</span></span>

3. <span data-ttu-id="5c4e3-152">テスト中に、コンテンツが VR モードの1つ目にのみ表示されることが判明した場合は、使用するカスタムシェーダーで SPI レンダリングがサポートされていない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-152">If during testing you discover that your content only appears in one eye in VR mode, it is likely that the custom shaders you use do not support SPI rendering.</span></span> <span data-ttu-id="5c4e3-153">別のシェーダーを選択するか、 [Unity の SPI アップグレードガイド](https://docs.unity3d.com/Manual/SinglePassInstancing.html) に従ってシェーダーを手動で編集し、サポートを追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-153">You’ll need to choose a different shader, or follow [Unity’s SPI upgrade guide](https://docs.unity3d.com/Manual/SinglePassInstancing.html) to manually edit the shader and add support.</span></span>

4. <span data-ttu-id="5c4e3-154">WinMR の場合は、次のことを行う必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-154">For those on WinMR, please remember that before you can access VR mode in AltspaceVR, you must:</span></span> 
    1. <span data-ttu-id="5c4e3-155">Microsoft Store から Windows Mixed Reality の OpenXR をダウンロードしてインストールします。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-155">Download and install OpenXR for Windows Mixed Reality from the Microsoft Store.</span></span>
        1. <span data-ttu-id="5c4e3-156">Mixed Reality ポータルアプリを開く</span><span class="sxs-lookup"><span data-stu-id="5c4e3-156">Open the Mixed Reality Portal app</span></span>
        2. <span data-ttu-id="5c4e3-157">アプリの左下隅にある [詳細を表示] を選択します。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-157">On the lower-left corner of the app select "See More"</span></span>
        3. <span data-ttu-id="5c4e3-158">表示されたメニューで、[Set Up OpenXR] を選択します。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-158">In the menu that appears select Set Up OpenXR.</span></span> <span data-ttu-id="5c4e3-159">これにより、ランタイムをインストールできる Windows ストアが起動されます。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-159">Doing this will cause the Windows Store to launch from where you can install the runtime.</span></span> <span data-ttu-id="5c4e3-160">このメニュー項目が表示されない場合は、OpenXR が既に PC にインストールされている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="5c4e3-160">If this menu item does not appear, OpenXR may already be installed on your PC.</span></span>