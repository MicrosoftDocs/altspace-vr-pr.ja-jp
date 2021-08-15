---
title: コンテンツを最新の Unity バージョンに更新する
description: コンテンツを最新バージョンの Unity に更新する方法について学習します。
ms.date: 06/4/2021
ms.topic: article
keywords: kits, worlds, unity, 更新, シェーダー, アップデータツール, トラブルシューティング
ms.openlocfilehash: a10e64b4dc19e256dcae9d61620de0140db60ccc0bf2a10dc864313f139bbd10
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "119126763"
---
# <a name="updating-content-to-the-latest-unity-version"></a>コンテンツを最新の Unity バージョンに更新する

## <a name="moving-to-unity-202039"></a>Unity 2020.3.9 への移行

今日から、AltspaceVR は最新バージョンの Unity (2020.3.9) にアップグレードされました。 パフォーマンスの向上に加えて、この更新プログラムは今後、組み込む予定の機能を証明します。 この変更は、既存のすべてのコンテンツと互換性がある必要があります。 サポートされていない場合は、サポートにお問い合わせください:altvr.com/support

この 2020.3.9 への移行はユーザーが生成したコンテンツには影響しませんが、数週間後に AltspaceVR のステレオ レンダリング モードに変更を行い、ユーザーがコンテンツ を更新する必要[があります。]( https://docs.unity3d.com/Manual/SinglePassStereoRendering.html) この Single [Pass Instancing へのアップグレードにより](https://docs.unity3d.com/Manual/SinglePassInstancing.html) 、世界のパフォーマンスが大幅に向上します。 この新しいビルドでは、2019.4 以前のコンテンツとの下位互換性はサポートされなくなったので、ご安心ください。 壊れた変更を回避するために、作成者が所有するコンテンツはすべてできるだけ早く更新する必要があります。 以下のガイドに従ってコンテンツを更新し、Unity 2020.3.9 でシングル パス の作成にスムーズに移行します。

> [!NOTE]
> 他のユーザーが所有し、自分と共有されているコンテンツを定期的に使用している場合は、ワールド/キットの所有者に問い合わせ、コンテンツの更新を計画している必要があります。

> コンテンツ作成者が質問 altvr.com/support がある場合、またはサポートが必要な場合は、サポート チームにお問い合わせください。

## <a name="testing-your-spi-content"></a>SPI コンテンツのテスト

次のプレビュー バージョンの AltspaceVR を使用して、VR で新しく更新されたコンテンツをテストします。 プレビュー バージョンはテストのみを目的とします。プラットフォームの一般的な使用には使用できません。

* [AltspaceVR SPI Preview for Windows Mixed Reality](https://aka.ms/AvrSpiMr)
* [AltspaceVR SPI Preview for SteamVR](https://aka.ms/AvrSpiSteam)
* [Oculus Rift の AltspaceVR SPI プレビュー](https://aka.ms/AvrSpiRift)

> 注: PC VR プレビューだけが提供されています。 シングル パス インスタンス化レンダリングは Android では使用できません。Mac のような VR 以外のプラットフォームでは必要ではありません。 そのため、一般的なリリース バージョンを使用して、これらのデバイスをテストできます。


## <a name="storecompatibilitycheck"></a>ストアの互換性チェック

Unity 2020.3.9 へのアップグレードは、ヘッドセットとストアビルドの互換性にも影響します。 これで、ヘッドセットと互換性のあるストアから AltspaceVR をダウンロードする必要があります。 例: WinMR または Oculus ヘッドセットの場合は、それぞれ Windows Store または Oculus Store から AltspaceVR をダウンロードします。 Windows Mixed Realityユーザーは、Windows Store から AltspaceVR、Steam から SteamVR ユーザー、Oculus Store から Oculus Rift ユーザーをダウンロードする必要があります。

## <a name="altspacevr-uploader-v090-upgrade-guide"></a>AltspaceVR Uploader v0.9.0 アップグレード ガイド 

Uploader 0.9 は、以前のバージョンの Uploader とは異なる方法でパッケージ化されています。 このパッケージ化の変更と同時に、新しい Uploader には新しいバージョンの Unity が必要です。 このガイドは、このアップグレード プロセスを、関係するすべてのユーザーに対してスムーズかつ安全にすることを目的にしています。

1. **プロジェクトのバックアップ** - プロジェクト ディレクトリ全体のコピーを作成し、安全な場所に置きます。 このアップグレードは破壊的なアップグレードなので、完了した後に Unity 2019.4 のバンドルを作成またはアップロードする機能は使用できます。 このアップグレード中に問題が発生した場合は、プロジェクトのクリーン コピーが必要です。 AltspaceVR が Unity 2020.3.9 に正式にアップグレードされる前に、ライブ キットまたはテンプレートを更新する必要があります。

2. **REMOVE OLD UPLOADER** - Unity を閉じた状態で、次のファイル/フォルダーを削除します。これは対応する .meta ファイルです。

    ```console
    * Assets/Altspace

    * Assets/Plugins

    * Assets/Prefabs/test-folder, Readme.txt

    * Assets/Resources/bg.jpeg, bg2.jpeg, logo.png, UserPreferences.asset

    * Assets/DFloor_v004.fbx

    * Library (This is a Unity system folder, not an Uploader folder. Delete it anyway, and let it be rebuilt during the upgrade.)
    ```

3. **エンジンバージョンのダウンロード**- Unity Hub を開き、Unity 2020.3.9 をインストールします (または、ここをクリックして直接インストールします)。 [](https://unity3d.com/ru/unity/whats-new/2020.3.9)

4. **UPGRADE PROJECT** - Unity 2020.3.9 でクリーンアップしたプロジェクトを開き、Unity でプロジェクトをアップグレードできます。

5. (PC のみ) **MIXED REALITY FEATURE TOOL** のダウンロード - 手順に従って Mixed Reality [Feature Tool](/windows/mixed-reality/develop/unity/welcome-to-mr-feature-tool)をダウンロードします。これは、Uploader パッケージのインストールを管理するために使用します。

6. **UPLOADER のインストール** - MR 機能ツールを使用して Unity プロジェクトを選択し、AltspaceVR Uploader 機能 (AltspaceVR 見出しの下) を追加します。 ツールの指示に従います。

macOS では、レジストリから最新バージョンを手動[](https://dev.azure.com/aipmr/MixedReality-Unity-Packages/_packaging?_a=package&feed=Unity-packages&package=com.microsoft.altspacevr_uploader&protocolType=Npm&version=0.9.0&view=versions)でダウンロードし、Unity エディターのパッケージ マネージャー (Windows > パッケージ マネージャー > + > Add package from tarball) 内からインストールします。

パッケージのインポートが完了すると、AltspaceVR メニュー項目で使い慣れた [Uploader] ウィンドウが表示されます。

## <a name="troubleshooting-tips"></a>トラブルシューティングのヒント

1. WinMR ヘッドセットでコントローラーまたは入力の問題が発生している場合は、プレゼンス センサーを適切に接続するために頭の上に配置されていることを確認します。 これは既知の問題であり、Microsoft は積極的に解決に取り組しています。

2. ヘッドセットとストア ビルドの互換性を確認します。 たとえば、WinMR ヘッドセットを使用している場合は、AltspaceVR ビルドが Windows Store を通じて取得済みWindowsしてください。

3. テスト中に、VR モードでコンテンツが 1 つの目にしか表示されない場合は、使用するカスタム シェーダーが SPI レンダリングをサポートしていない可能性があります。 シェーダーを手動で編集してサポートを追加するには、別のシェーダーを選択するか [、Unity](https://docs.unity3d.com/Manual/SinglePassInstancing.html) の SPI アップグレード ガイドに従う必要があります。

4. WinMR の場合は、AltspaceVR で VR モードにアクセスする前に、次のことを行う必要があります。 
    1. OpenXR for Windows Mixed RealityをダウンロードしてインストールMicrosoft Store。
        1. アプリを開Mixed Reality ポータルする
        2. アプリの左下隅にある [詳細を表示] を選択します
        3. 表示されるメニューで、[OpenXR のセットアップ] を選択します。 これにより、ランタイムをインストールWindowsストアが起動します。 このメニュー項目が表示されない場合は、OpenXR が PC に既にインストールされている可能性があります。