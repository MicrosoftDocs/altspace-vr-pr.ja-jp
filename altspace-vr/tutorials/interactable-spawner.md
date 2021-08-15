---
title: Interactables Spawner の使用
description: 対話可能なスポーナーを作成、使用、カスタマイズして、AltspaceVR スペースに項目を配置する方法について学習します。
ms.date: 02/10/2021
ms.topic: article
keywords: spawner, 相互作用, カスタマイズ
ms.openlocfilehash: abeddec5c2b50e0612db5efb6bc2e3c5bd9de4a8b67c50b19afee18b17c5e746
ms.sourcegitcommit: b248ba2a6da7d669b430581fc3a1544413b2e9c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "119127402"
---
# <a name="using-the-interactables-spawner"></a>Interactables Spawner の使用

Interactables Spawner を使用すると、イベント、ワールド、またはホーム空間に対話可能な項目を配置できます。 この機能は現在、早期アクセス[](../world-building/early-access.md)プログラムの一部であり、メイン メニューを使用してオプトインしない限り使用できません。

> [!NOTE]
> 引き続きこの機能のパイロットを行っていますが、対話可能な操作が多すぎると、環境またはイベントのパフォーマンスに影響を与える可能性があります。 

## <a name="creating-an-interactable"></a>対話可能なを作成する

オブジェクトを対話可能なオブジェクトに変換するには:

1. オブジェクトをスペースに配置します。
2. 次に、オブジェクトの一覧でエントリを探し、その横にある歯車アイコンを選択して設定を開きます。

![オブジェクト一覧が強調表示されたワールド エディターを開く](images/interactables-spawner-img-01.png)

設定ページには、対話可能なオブジェクトにするための新しいチェック ボックス **"Object spawner"** が表示されます。

1. チェック ボックスをオンにし、 の確認を **選択します**。
2. 編集モードでは、空間内のオブジェクトの生成位置を移動できます。
3. **項目の操作を有効** にするには、編集モードを終了します。

![AltspaceVR アプリで成果物ウィンドウを開く更新](images/interactables-spawner-img-02.png)

## <a name="other-customizations"></a>その他のカスタマイズ

そのオブジェクトのプロパティに戻って "Object **spawner"** を有効にした後、生成されたオブジェクトの動作に適用できる追加の設定があります。

> [!NOTE]
> 対話可能なオブジェクト スケール: これは、オブジェクトを初めて選択する前に、オブジェクトが世界でどのように表示されるかのスケールである "スケール" と比較して、取得時のオブジェクトのスケールを設定します。

AltspaceVR の実行中にキットが変更された場合、AltspaceVR を再起動するまで、キットの変更は有効にならならない場合があります。

最近、[Reload Worlds Kits] (ワールド キットの再読み込み)**設定**[中程度] タブに **ボタンを追加しました**。 このボタンをクリックすると (自分だけが) スペースを再入力し、すべてのキットを再度再読み込みします。これにより、AltspaceVR の間に更新された新しいバージョンのキットだけがダウンロードされます。

![AltspaceVR アプリで [中程度の設定] パネルが開きます](images/interactables-spawner-img-03.png)