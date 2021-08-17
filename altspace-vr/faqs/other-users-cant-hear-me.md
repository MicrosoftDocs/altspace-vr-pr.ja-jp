---
title: 私の声が他のユーザーに聞こえません
description: AltspaceVR で聞こえない他のユーザーに関連する問題を特定して修正する方法について説明します。
ms.date: 03/11/2021
ms.topic: article
keywords: faq
ms.openlocfilehash: 189d96790207085a2a2c47e964c0db8a08ed95a76d91d2ced3026ba3455b45e3
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "119128094"
---
# <a name="other-users-cant-hear-me"></a>私の声が他のユーザーに聞こえません

まず、AltspaceVR がマイクからのオーディオを検出しているかどうかを確認します。 これを確認するには、ビューの左下にあるマイク アイコンが話しているときに点滅するかどうかを確認します。 話をするときにアイコンが点滅すると、マイクが動作しています。 アイコンが赤の場合は、ミュートされます。 自分でミュートまたはミュート解除するには、アイコンを選択します。

ミュートを解除した後にマイク アイコンが点滅しない場合は、AltspaceVR でマイクの設定を調整する必要がある場合は、[メニュー] / [設定] / [オーディオ/ オーディオ入力の選択] に移動します。 次に、矢印ボタンを使用して、使用するマイクを選択します。
 
## <a name="oculus-quest"></a>Oculus Quest 

AltspaceVR をインストールするときに、マイク オーディオを使用するためのアクセス許可を付与してください。 実行できるもう 1 つのチェックは、Menu / 設定 / Audio / Audio Input Selection を調べたり、Android オーディオ入力 (Quest/Quest2 の既定のマイク) に設定されているのを確認する方法です。
 
## <a name="windows-mixed-reality-oculus-rift-htc-vive-or-2d-mode"></a>Windows Mixed Reality、Oculus Rift、HT Vive、または 2D モード

AltspaceVR: Menu / 設定 / Audio / Audio Input Selection で適切なマイク設定が設定されていることを確認します。 次に、矢印ボタンを使用して、使用するマイクを選択します。

AltspaceVR を開始する前に、適切なマイクが既定の録音デバイスとして設定Windows。 Oculus Rift と ALT Vive の両方にマイクが組み込まれているので、AltspaceVR に別のマイクが接続されている場合は、そのデバイスを使用しようとしている可能性があります。
 
デバイスの既定の記録デバイスを変更Windows。
* [デバイス] の [スピーカー] アイコンを右クリックWindowsデバイスの再生 **] を選択します。**
* [記録] タブ **に移動** します
* 使用するマイクを見つける。 [MICROPHONE - USB Audio **Device]/(マイク - USB オーディオ** デバイス)、[Oculus Rift Microphone]/(Oculus Rift マイク) というラベルが付いた [MICROPHONE - Rift Audio]/(マイク - リフト オーディオ)" というラベルが付いた[MICROPHONE Vive **microphone]を選択します**。
* そのマイクを右クリックし、 [既定のデバイス **に設定] を選択します**
* AltspaceVR を再起動すると、マイクが選択されます
 
これらの手順を実行した後も問題が発生している場合は、他にもいくつかの問題が発生し、影響を受ける可能性があります。
* 30 Alt-Tabを超える時間を超える場合は、AltspaceVR によって自動ミュートが実行されます。これを無効にするには、キーボード ショートカット space キーを使用して、ミュートをオフ/オンに切り替えます。
* AltspaceVR オーディオ システムには、以下のボリュームしきい値があります。 マイク レベルを max に設定し、マイクを口の近くに設定して、通常の音量で話します。
* VR を終了し、ヘッドセットから別の USB 3.0 ポートに USB コードを接続してみてください。 このエクスペリエンスでは、一部の USB 3.0 ポートで問題が発生します。

AltspaceVR では、ゲーム中に行われたサウンド設定の変更が認識されない場合があります。そのため、有効にするには、上記のマイク変更の AltspaceVR を再起動する必要がある場合があります。  ゲームを再入力するときに、マイク アイコンを見て、点滅を確認します。 アイコンが点滅すると、マイクが動作しています。