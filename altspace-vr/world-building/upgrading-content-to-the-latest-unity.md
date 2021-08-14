---
title: 最新の Unity バージョンにコンテンツを更新しています
description: 最新バージョンの Unity にコンテンツを更新する方法について説明します。
ms.date: 06/4/2021
ms.topic: article
keywords: キット, ワールド, unity, 更新, シェーダー, アップローダー, トラブルシューティング
ms.openlocfilehash: a10e64b4dc19e256dcae9d61620de0140db60ccc0bf2a10dc864313f139bbd10
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "119126763"
---
# <a name="updating-content-to-the-latest-unity-version"></a>最新の Unity バージョンにコンテンツを更新しています

## <a name="moving-to-unity-202039"></a>Unity 2020.3.9 への移行

現時点では、Alt2020.3.9 Evr は最新バージョンの Unity () にアップグレードされています。 いくつかのパフォーマンスの向上に加えて、この更新プログラムは、今後導入される予定の機能を対象としています。 この変更は、既存のすべてのコンテンツと互換性がある必要があります。 そうでない場合は、サポートにお問い合わせください: altvr.com/support

この2020.3.9 への移行は、ユーザーが生成したコンテンツに影響を与えていませんが、数週間後に、 [ユーザーがコンテンツを更新する必要がある]( https://docs.unity3d.com/Manual/SinglePassStereoRendering.html)Alt evr のステレオレンダリングモードに変更を加えています。 この [1 回のパスのインスタンス](https://docs.unity3d.com/Manual/SinglePassInstancing.html) へのアップグレードにより、世界で大幅なパフォーマンス向上が可能になります。 この新しいビルドでは、2019.4 以前のコンテンツとの下位互換性がサポートされなくなることに注意してください。 すべての作成者が所有するコンテンツをできるだけ早く更新して、重大な変更を回避することは緊急です。 以下のガイドに従ってコンテンツを更新し、Unity 2020.3.9 でシングルパスのインスタンス化にスムーズに移行できるようにします。

> [!NOTE]
> 他のユーザーが所有しているコンテンツを定期的に使用していて、あなたと共有している場合は、世界/キットの所有者に連絡して、コンテンツの更新を計画していることを確認してください。

> コンテンツ作成者であり、不明な点やサポートが必要な場合は、サポートチーム () にお問い合わせください。 altvr.com/support

## <a name="testing-your-spi-content"></a>SPI コンテンツのテスト

次のプレビューバージョンの Altを使用して、VR で新しく更新されたコンテンツをテストします。 プレビューバージョンはテストのみを目的としており、プラットフォームの一般的な使用には使用しないでください。

* [Windows Mixed Reality の Altworkplace Evr SPI プレビュー](https://aka.ms/AvrSpiMr)
* [SteamVR の Altworkplace Evr SPI Preview](https://aka.ms/AvrSpiSteam)
* [Oculus Rift の Altworkplace Evr SPI Preview](https://aka.ms/AvrSpiRift)

> 注: PC VR のプレビュー版のみが提供されています。 シングルパスでインスタンス化されたレンダリングは Android では使用できません。 Mac などの VR 以外のプラットフォームでは必要ありません。 そのため、これらのデバイスをテストするには、一般リリースバージョンを使用できます。


## <a name="storecompatibilitycheck"></a>ストア互換性チェック

Unity 2020.3.9 へのアップグレードは、ヘッドセットとストアのビルドの互換性にも影響します。 これで、ヘッドセットと互換性のあるストアから Altをダウンロードする必要があります。 例として、winmr または Oculus のヘッドセットの場合は、それぞれ Windows ストアまたは Oculus ストアから alt をダウンロードします。 Windows Mixed Reality ユーザーは、Windows ストアから altOculus をダウンロードし、ストリームからのユーザーと Oculus Rift のユーザーをストアからダウンロードする必要があります。

## <a name="altspacevr-uploader-v090-upgrade-guide"></a>Alt0.9.0 Evr アップローダー v のアップグレードガイド 

アップローダー0.9 は、以前のバージョンのアップローダーとは異なる形でパッケージ化されています。 このパッケージの変更と同時に、新しいアップローダーには新しいバージョンの Unity が必要です。 このガイドは、関係するすべてのユーザーに対して、このアップグレードプロセスをより円滑かつ安全にすることを目的としています。

1. **プロジェクトのバックアップ** -プロジェクトディレクトリ全体のコピーを作成し、安全な場所に配置します。 このアップグレードは破壊的なアップグレードであるため、完了後に Unity 2019.4 のバンドルを作成またはアップロードすることはできません。 このアップグレード中に問題が発生した場合は、プロジェクトのクリーンコピーが必要になります。 また、2020.3.9 に正式にアップグレードする前に、ライブキットまたはテンプレートを更新する必要もあります。

2. **古いアップローダーを削除** します。 Unity が閉じている場合は、次のファイル/フォルダーを削除し、それに対応するメタファイルを削除します。

    ```console
    * Assets/Altspace

    * Assets/Plugins

    * Assets/Prefabs/test-folder, Readme.txt

    * Assets/Resources/bg.jpeg, bg2.jpeg, logo.png, UserPreferences.asset

    * Assets/DFloor_v004.fbx

    * Library (This is a Unity system folder, not an Uploader folder. Delete it anyway, and let it be rebuilt during the upgrade.)
    ```

3. [**エンジンバージョンのダウンロード**]-unity ハブを開き、unity 2020.3.9 をインストールします (または、[ここをクリックし](https://unity3d.com/ru/unity/whats-new/2020.3.9)て直接インストールします)。

4. [**プロジェクトのアップグレード**]: unity 2020.3.9 で、クリーンされたプロジェクトを開き、unity がプロジェクトをアップグレードできるようにします。

5. (PC のみ) **MIXED REALITY 機能ツールをダウンロード** する-手順に従って、アップローダーパッケージのインストールの管理に使用する [Mixed reality 機能ツール](/windows/mixed-reality/develop/unity/welcome-to-mr-feature-tool)をダウンロードします。

6. **アップローダーをインストール** します。 MR 機能ツールを使用して Unity プロジェクトを選択し、Alt Evr アップローダー機能を追加します (alt の見出しの下)。 ツールの指示に従います。

macOS では、[レジストリ](https://dev.azure.com/aipmr/MixedReality-Unity-Packages/_packaging?_a=package&feed=Unity-packages&package=com.microsoft.altspacevr_uploader&protocolType=Npm&version=0.9.0&view=versions)から最新バージョンを手動でダウンロードし、Unity エディターのパッケージマネージャー内からインストールします (Windows > パッケージマネージャー > + > [tar からパッケージを追加])。

パッケージのインポートが完了したら、使い慣れたアップローダーウィンドウを [Alt] メニュー項目で使用できるようになります。

## <a name="troubleshooting-tips"></a>トラブルシューティングのヒント

1. WinMR ヘッドセットでコントローラーまたは入力の問題が発生している場合は、プレゼンスセンサーに適切に参加するために、ヘッドに設置されていることを確認します。 これは既知の問題であり、マイクロソフトはその解決に積極的に取り組んでいます。

2. ヘッドセットとストアとビルドの互換性を確認します。 たとえば、winmr ヘッドセットを使用している場合は、Windows ストアを通じて altを取得したことを確認してください。

3. テスト中に、コンテンツが VR モードの1つ目にのみ表示されることが判明した場合は、使用するカスタムシェーダーで SPI レンダリングがサポートされていない可能性があります。 別のシェーダーを選択するか、 [Unity の SPI アップグレードガイド](https://docs.unity3d.com/Manual/SinglePassInstancing.html) に従ってシェーダーを手動で編集し、サポートを追加する必要があります。

4. WinMR の場合は、次のことを行う必要があることに注意してください。 
    1. Microsoft Store から Windows Mixed Reality 用の OpenXR をダウンロードしてインストールします。
        1. Mixed Reality ポータルアプリを開く
        2. アプリの左下隅にある [詳細を表示] を選択します。
        3. 表示されたメニューで、[Set Up OpenXR] を選択します。 これにより、ランタイムをインストールできる場所から Windows ストアが起動されます。 このメニュー項目が表示されない場合は、OpenXR が既に PC にインストールされている可能性があります。