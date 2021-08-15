---
title: 概要
description: AltspaceVR、Mixed Reality 拡張機能、ワールド エディター、開発中にヘルプを表示する方法について学習します。
ms.date: 02/10/2021
ms.topic: article
keywords: world editor, unity uploader, forums
ms.openlocfilehash: 97003073facfa0f4135111fff0ed6128b42ca81b96a8a70fdebef22d8988f548
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "119126321"
---
# <a name="getting-started-with-altspacevr"></a>AltspaceVR の使用を開始する

AltspaceVR 開発者フォーラムへようこそ。 次のセクションでは、AltspaceVR にコンテンツを追加するさまざまな方法について説明します。

## <a name="mixed-reality-extension-mre-sdk"></a>Mixed Reality拡張機能 (MRE) SDK

MRE SDK は、 を使用して AltspaceVR 拡張機能をビルドする新しい SDK Node.JS。 作業を開始するには:

1. AltspaceVR (Steam または Oculus Store から) をインストールし、AltspaceVR アカウントを作成して、アプリについて理解します。
2. [Git コマンド ライン ツールをインストールする](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
3. [MRE SDK サンプル リポジトリ](https://github.com/Microsoft/mixed-reality-extension-sdk-samples)に移動し、詳細な手順に従ってサンプルをビルドして実行します

次のこともできます。

* [MRE SDK Discord Community](https://discord.com/invite/xyBcQec)参加して、他の MRE 開発者とチャットします。
* [Building Tic-Tac-Toe のビデオを見る](https://www.youtube.com/watch?v=DQHrdK9JSXI&ab_channel=AltspaceVR)
* アプリケーションを使用して MREs を編集[およびビルドする](https://github.com/Microsoft/mixed-reality-extension-sdk#using-visual-studio-code)方法Visual Studio Code
* ソース [コードHello World参照する](https://github.com/Microsoft/mixed-reality-extension-sdk-samples/tree/master/samples/hello-world)
* [AltspaceVR で毎週の開発者向け会議に参加する](https://account.altvr.com/channels/sdk)

その他のリソースは近日公開予定です。

## <a name="world-editor"></a>ワールド エディター

AltspaceVR 内では、組み込みのワールド エディターをホーム空間で使用できます。 これは、スペースの変更を開始する最も簡単な方法です。 ホームスペースを使用している場合は、右下にある [ワールド エディター] ボタンを選択します。 「ワールドビルディングはじめに[を使用する」ページを参照してください](../world-building/world-building-getting-started.md)。 ワールド エディターを使用すると、3D オブジェクト、テレポーターと拡張機能 (MRE) を配置し、ワールド Skybox を変更できます。

早期アクセス プログラム に[参加している場合は](../world-building/early-access.md)[、AltspaceVR の [My Worlds] ページでさらにワールドを作成できます](https://account.altvr.com/users/sign_in)。

また、Web サイト、ワールド エディター、Unity アップデータツールなど、世界を構築するエンドツーエンドのプロセスをカバーする [、Karnivore23](https://www.youtube.com/watch?v=G8xgR3cDMjk&ab_channel=MarkGill) によるすばらしいビデオも紹介されています。

## <a name="unity-uploader"></a>Unity アップアップロード

世界とカスタム キットの両方に Unity アップデータツールを提供しています。 この機能は開発の初期段階です。 詳細については、World [Builders Discord](https://discord.com/invite/Kp59Frb) チャネルに参加してチャットを行うか [、World Building](../world-building/getting-help.md)のヘルプ ページで確認してください。

Unity 2019.2 に更新するレガシ Unity 2018 キットまたはテンプレートがある場合は、アップグレード ガイド を [参照してください](https://developer.altvr.com/upgrade-2019-2/)。

## <a name="integrating-the-mre-sdk-into-your-own-app"></a>MRE SDK を独自のアプリに統合する

Unity3D で独自のアプリまたはゲームを作成し、アプリ内で MRE を実行する場合は [、MRE Unity クライアント](https://github.com/Microsoft/mixed-reality-extension-unity) ライブラリ リポジトリを参照してください。
