---
title: Mixed Reality拡張機能の使用
description: 拡張機能を使用してトラブルシューティングを行Mixed Reality AltspaceVR の世界を拡張および適応する方法について説明します。
ms.date: 03/11/2021
ms.topic: article
keywords: Mixed Reality, 拡張機能, トラブルシューティング
ms.openlocfilehash: 1439ca76eaf4e0235c6552d037e55b6151e08407871bf470b3011b6cf8cbccd5
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "119125359"
---
# <a name="using-a-mixed-reality-extension"></a>Mixed Reality拡張機能の使用

[Mixed Reality拡張機能](https://developer.altvr.com/)(MREs) は、世界で使用できるアプリです。このアプリは[](https://account.altvr.com/mres/1173667287173955931)、実際に動作する[Stargate](https://account.altvr.com/mres/1152987031857529562)に対して、 プログラミングエクスペリエンスを持つコミュニティ メンバーは、Altspace を拡張し、一方通行の World Builder を使用してワールドをより対話的に行う方法です。 世界の誰でも MREs を使用できる一方で、ワールド ビルディング プログラムのユーザーだけが自分の世界で MREs を参照して生成できます。 

1. Web サイトの MRE セクションを [参照します](https://account.altvr.com/mres)。 既定では、独自の MREs が表示されます。 **そのため、Altspace** を選択して公式の MREs と **おすすめ** を表示し、コミュニティからの MREs を表示します。 世界中で使用する前に、MRE について理解してください。 
2. [[Clipboards MRE] に移動](https://account.altvr.com/mres/1173667287173955931)し、[クリップボードに **コピー] を選択します**。 
3. [ワールド] を入力し、[ワールド エディター] を開き **、[基本] > SDK アプリを開きます**。 [Target URI]/(ターゲット URI)フィールドに [下向き URL] を貼り付け、[確認] を **選択します**。 MRE オブジェクトが表示され、クラウドで実行されている MRE への接続が試行されます。 これで、クリックできるいくつかの保護機能が表示されます。
4. 他のワールド オブジェクトと同様に、MRE を移動/回転/スケーリングします。

おめでとうございます。 これで MREs を使用しています。これで非常にクールです。

## <a name="troubleshooting"></a>トラブルシューティング

**MRE に、顔をしかめかしている絵文字が表示されている** 
    * URL が正しいか確認する
    * オブジェクトの **[再生中の** 切り替え] オプションを選択し、[確認] を **選択します**
    * 再入力を試す

**MRE が遅い** MRE がホストされている場所によっては、ネットワーク待機時間が発生する可能性があります

**URL を貼り付ける必要がある理由**
今後は、Kits から作成する場合と同様に、MREs をArtifacts生成できます。 それまでは、URL を引き続き使用します