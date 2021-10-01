---
title: AltspaceVR オーディオに関してよく寄せられる質問
description: オーディオ関連の問題のトラブルシューティングとサポート。
ms.date: 8/23/2021
author: qianw211
ms.author: v-qianwen
ms.topic: article
keywords: vr, オーディオ, トラブルシューティング, サポート
ms.openlocfilehash: 05c8a477b9e50b5067e62b934fe2ff8bd656f06c
ms.sourcegitcommit: 5c452a9092297c0bfbc8efabebf395e7ee31853f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/30/2021
ms.locfileid: "129311910"
---
# <a name="frequently-asked-questions-about-audio"></a>オーディオに関してよく寄せられる質問

## <a name="does-my-vr-headset-have-a-built-in-mic"></a>VR ヘッドセットにマイクが組み込みですか?

### <a name="oculus-riftrift-s-oculus-questquest-2-windows-mixed-reality-and-htc-vive"></a>Oculus Rift/Rift S、Oculus Quest/Quest 2、Windows Mixed Reality、および QUEST Vive

はい。これらの VR ヘッドセットにはマイクが組み込みされています。

### <a name="windows"></a>Windows

Windows で使用されるヘッドセットの場合は、ヘッドセットを接続している間に、[記録デバイス] の下に一覧表示されているマイクを見つけられます。

### <a name="further-troubleshooting"></a>その他のトラブルシューティング

* [AltspaceVR のサポート - 他のユーザーに聞こえない](#what-do-i-do-if-other-users-cant-hear-me)
* [AltspaceVR のサポート - Oculus Quest のアクセス許可の管理](../getting-started/oculus-controls.md#managing-permissions)

## <a name="is-there-a-push-to-talk-button"></a>プッシュ ツー トーク ボタンはありますか?

プッシュ対トーク ボタンはありません。  ビューの左下を見た場合は、音声の切り替えに使用できるマイク アイコンがあります。 または、キーボード ショートカットのスペース バーを使用して、マイクのミュート/ミュート解除を行います。

話をするとアイコンが点滅する場合は、マイクが動作しています。
 
## <a name="what-do-i-do-if-my-audio-is-choppy"></a>オーディオが途切れ途切れな場合は、どうしますか?

一部のユーザーは、別のアバターが音声を話している場合に、途切れ途切れとして、または通常のドロップアウトが表示されるのを知っています。 他の場合、独自のオーディオが途切れやロボットを通じて聞こえてくると、他のユーザーから通知を受け取る場合があります。

最初に試すのは、常に自分が入っている領域を再入力するか、これが失敗した場合に AltspaceVR を再起動する方法です。 オーディオの問題は一般的な問題ではありません。ただし、発生した場合、これは多くの場合、簡単に修正できます。 

これが失敗した場合は、以下を調査できます。

#### <a name="cpu-performance-for-desktop-users"></a>デスクトップ ユーザーの CPU パフォーマンス

AltspaceVR [を実行する場合に](../getting-started/system-requirements.md) 推奨されるハードウェアの推奨システム仕様を確認してください。 i3 以下の CPU は、ビデオのフレーム レートだけでなく、ドロップアウトや品質の低下などのオーディオの問題の原因となる可能性があるという問題を引き起こす可能性がある点が判明しました。

#### <a name="internet-bandwidth-and-network-connection"></a>インターネット帯域幅とネットワーク接続

低速のインターネット接続 (5 mbps 未満) または WiFi 上のユーザーには、ドロップアウトなどのオーディオの問題が発生する可能性があります。 イーサネット ケーブルをコンピューターにハードライン接続し、接続を 5 mbps より速くすることをお勧めします。 バックグラウンドでインターネット接続を使用している可能性があるプログラムを終了することができます。

## <a name="what-do-i-do-if-other-users-cant-hear-me"></a>他のユーザーに聞こえない場合は、どうしますか?

まず、AltspaceVR がマイクからのオーディオを検出しているかどうかを確認します。 これを確認するには、ビューの左下にあるマイク アイコンが話しているときに点滅するかどうかを確認します。 話をするときにアイコンが点滅すると、マイクが動作しています。 アイコンが赤の場合は、ミュートされます。 自分でミュートまたはミュート解除するには、アイコンを選択します。

ミュートを解除した後にマイク アイコンが点滅しない場合は、AltspaceVR でマイクの設定を調整する必要がある場合は、[メニュー] / [設定] / [オーディオ/ オーディオ入力の選択] に移動します。 次に、矢印ボタンを使用して、使用するマイクを選択します。
 
### <a name="oculus-questquest-2"></a>Oculus Quest/Quest 2

AltspaceVR をインストールするときに、マイク オーディオを使用するためのアクセス許可を付与してください。 もう 1 つの確認は、Menu / 設定 / Audio / Audio Input Selection を参照し、Android オーディオ入力 (Quest/Quest2 の既定のマイク) に設定されています。
 
### <a name="windows-mixed-reality-oculus-riftrift-s-htc-vive-or-2d-mode"></a>Windows Mixed Reality、Oculus Rift/Rift S、HT Vive、または 2D モード

AltspaceVR: Menu / 設定 / Audio Input Selection で適切なマイク設定が設定されていることを確認します。 次に、矢印ボタンを使用して、使用するマイクを選択します。

AltspaceVR を開始する前に、適切なマイクが既定の録音デバイスとして設定Windows。 AltspaceVR に別のマイクが接続されている場合、Oculus Rift/Rift S と ALT Vive の両方にマイクが組み込まれている場合、そのデバイスを使用しようとしている可能性があります。
 
デバイスの既定の記録デバイスを変更Windows。

* アプリの [スピーカー] アイコンを右クリックしWindowsサウンド設定 **を開く] を選択します**。
* [入力 **]/[入力デバイスの選択] ドロップダウンに** 移動します。
* ドロップダウン メニューから使用するマイクを選択します。 
    * [MICROPHONE - USB Audio Device]/(マイク **- USB オーディオ** デバイス)、
    * Oculus Rift マイクには、ヘッドセット マイク **(Oculus Virtual Audio Device) というラベルが付けされます**。
* AltspaceVR を再起動すると、マイクが選択されます
 
これらの手順を実行した後も問題が発生している場合は、次のような影響を与える可能性があります。

* 30 Alt-Tab時間が切れた場合、AltspaceVR によって自動的にミュートされます。 これは、[メニュー] **-> 設定 -> [オーディオ] -> AltspaceVR** がアイドル状態のときに [ミュート] で無効にできます。
* AltspaceVR オーディオ システムには、以下のボリュームしきい値があります。 マイク レベルを max に設定し、マイクを口の近くに設定して、通常の音量で話します。
* VR を終了し、ヘッドセットから別の USB 3.0 ポートに USB コードを接続してみてください。 このエクスペリエンスでは、一部の USB 3.0 ポートで問題が発生します。

AltspaceVR では、ゲーム中に行われたサウンド設定の変更が認識されない場合があります。そのため、上記のマイクの変更を有効にするために AltspaceVR を再起動する必要がある場合があります。  ゲームに再び入った後、マイク アイコンを見て、話をすると点滅するのを確認します。 アイコンが点滅すると、マイクが動作しています。

## <a name="support"></a>サポート

AltspaceVR チームに関する質問またはフィードバック 

> [!div class="nextstepaction"]
> [ここをクリックしてサポート リクエストを送信する](https://help.altvr.com/hc/requests/new)