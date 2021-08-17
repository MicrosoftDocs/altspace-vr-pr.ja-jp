---
title: Interactables Spawner の使用
description: Interactables spawner を作成、使用、カスタマイズする方法について説明します。これらの項目は、Altspaces Evr スペースに配置します。
ms.date: 02/10/2021
ms.topic: article
keywords: spawner、相互作用、カスタマイズ
ms.openlocfilehash: abeddec5c2b50e0612db5efb6bc2e3c5bd9de4a8b67c50b19afee18b17c5e746
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127402"
---
# <a name="using-the-interactables-spawner"></a>Interactables Spawner の使用

Interactables Spawner を使用すると、イベント、世界、またはホームスペースに対話型項目を配置できます。 この機能は、現在、 [早期アクセスプログラム](../world-building/early-access.md) の一部であり、メインメニューを使用して選択しない限り利用できません。

> [!NOTE]
> この機能のパイロット処理は継続していますが、内部のテーブルが多すぎると環境やイベントのパフォーマンスに影響する可能性があることに注意してください。 

## <a name="creating-an-interactable"></a>対話型の作成

オブジェクトを対話型オブジェクトに変換するには、次のようにします。

1. オブジェクトをスペースに配置します。
2. 次に、[オブジェクト] ボックスの一覧でエントリを探し、その横にある **歯車アイコン** を選択して設定を開きます。

![オブジェクトリストが強調表示された状態で開いているワールドエディター](images/interactables-spawner-img-01.png)

[設定] ページで、 **"object spawner"** という新しいチェックボックスが表示されます。このチェックボックスを使用して、対話型オブジェクトを作成します。

1. チェックボックスをオンにして、[ **確認**] を選択します。
2. 編集モードでは、空間内のオブジェクトの生成場所を移動できます。
3. **編集モードを終了** して、項目の操作を有効にします。

![Altworkplace Evr アプリで開かれている [更新アイテム] ウィンドウ](images/interactables-spawner-img-02.png)

## <a name="other-customizations"></a>その他のカスタマイズ

オブジェクトのプロパティに戻ったときに **"object spawner"** を有効にすると、生成されたオブジェクトの動作に適用できる追加の設定が表示されます。

> [!NOTE]
> 対話型 object scale: オブジェクトの取得時にオブジェクトのスケールを設定します。 "Scale" と比較します。これは、オブジェクトを初めて選択する前に、世界でどのように表示するかのスケールです。

キットの開発者は、altの実行中にキットに加えられた変更が有効にならないことに注意してください。

最近、[**ワールドキットの再読み込み**] というボタンを [中 **程度の設定**] タブに追加しました。 このボタンをクリックすると、スペースを再入力するだけで、すべてのキットを再度読み込むことができます。これにより、Altspace Evr の間に更新された新しいバージョンのキットのみがダウンロードされます。

![[中程度の設定] パネルを [Altworkplace Evr] アプリで開く](images/interactables-spawner-img-03.png)