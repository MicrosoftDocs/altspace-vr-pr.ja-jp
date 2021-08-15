---
title: ユーザー機能の追加
description: AltspaceVR イベントで特別な機能をユーザーに提供する方法について学習します。
ms.date: 03/11/2021
ms.topic: article
keywords: 能力、ユーザー、ロール
ms.openlocfilehash: de03bcff2c0239ba5709e848523690c5fb5c85dc350661eca822094d21b87785
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "119126146"
---
# <a name="adding-user-abilities"></a>ユーザー機能の追加

イベントや Campfire では、中断が発生する可能性が高いので、飛ぶことはできない。 ただし、世界では、東部の部下のように人々を離れさせすることができます。 特殊な能力を付与する方法を次に示します。

![VR の既定のコンテキスト ロールが強調表示された Web サイトで開いている世界](images/contextual_roles.png)

1. Web サイトでワールドを編集します。 詳細については [操作方法の管理に関するページ](managing-worlds.md) を参照してください。
2. [In VR > **Default Contextual Roles] フィールドまで下にスクロール** します。 緑色の疑問符をポイントすると、詳細を表示できます。 すべての可能なロールが一覧表示されます。
3. World に入るすべてのユーザーが受け取るロールを指定します。 各ロールには独自の機能があります。
4. **[Update]** をクリックします。 ユーザーは、新しく見つかった機能を利用するには、ワールドを再入力する必要があります。

## <a name="roles-and-abilities"></a>ロールと能力

* **パイロット**- フライト ([Input > Fly] にアクセスして 設定 > VR でこれをアクティブにする必要があります)
* **megaphone_only** - 有効にした場合、すべてのユーザーが自分の耳の中で聞きます
* **musical_performer** - オーディオ品質と帯域幅の使用量の増加
* **Terraformer** - ワールド エディターへのアクセス
* **showcase_new_sdk** - 新しい SDK アプリを生成する
* もっとその。。。

## <a name="tips"></a>ヒント

* ユーザーを飛ばせそうになる場合は、アプリ **megaphone_only追加します** 。 人が飛び回っている世界の他の人を聞くのは難しい。
* **terraformer には注意してください**。 ユーザーはワールドを編集できます。 複数のユーザーが一緒にワールド ビルディングを行うのはまだ試験段階です。