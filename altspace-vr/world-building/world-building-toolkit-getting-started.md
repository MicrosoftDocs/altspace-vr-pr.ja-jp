---
title: Altspace アップローダーの概要
description: Altspace アップローダーを使用して Unity シーンテンプレートを使用して、Altspace Evr ワールドを設定し、アップロードする方法について説明します。
ms.date: 09/29/2021
ms.author: v-vtieto
ms.topic: article
keywords: toolkit、Altspace、アップローダー
ms.openlocfilehash: 8d71551fe552159c0078105307802774f44c0d47
ms.sourcegitcommit: 8c58f9f9ad1a3f9534141dee2c78e32792d0db7a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/25/2021
ms.locfileid: "130298815"
---
# <a name="introducing-the-altspace-uploader"></a>Altspace アップローダーの概要

> [!NOTE]
> - 興味をお持ちの場合は、 [公式の Altspacevr Discord](https://discordapp.com/invite/altspacevr) に参加し、#world ビルディングチャネルにアクセスしてください。  
> - 古い領域を回復する場合は、 [アップグレードガイド](upgrading-old-unity-projects.md)を参照してください。 

アップローダーを使用すると、Unity シーンを世界のテンプレートとして使用できます。 Minecraft から、満塁の家にハロウィーンやお気に入りの作成を持ち込むことができます。 Unity にインポートできる場合は、この方法で Altspace にアクセスできる可能性があります。 いくつかの [例](https://account.altvr.com/worlds/1046572460192825569)を次に示します。

![ワールドの例](images/unity-uploader-img-01.png)

## <a name="setup"></a>セットアップ

1. 公式の [Altspacevr Discord](https://discordapp.com/invite/altspacevr) に参加し、#world ビルディングチャネルにアクセスします。 友人は、友人が自分だけをビルドすることはできません。
2. 基本については、 [世界ビルのはじめにガイド](world-building-getting-started.md) を参照してください。
3. [Unity Hub](https://unity3d.com/get-unity/download) と **Unity 2020.3.9** をインストールします。 このバージョンと正確に一致しない限り、アップローダーは機能しません。 お持ちでない場合は、無料の Unity アカウントが必要になります。 インストール中に、(楽しいものにするために) **個人** バージョンを選択し、次のことを確認します。
    * **Android ビルドサポート** モジュールを含めます。
    * Windows には、 **Mac ビルドサポート (Mono)** モジュールを含めます。
    * Mac では、 **Windows ビルドサポート (Mono)** モジュールを追加します。
4. [Altアップローダー Evr をダウンロードする](https://aka.ms/AvrUrpUploader)
5. Web サイトに[テンプレートを作成](https://account.altvr.com/space_templates/new)します。 **Hello World テンプレート** に名前を指定します。
6. **Hello World** という名前を [作成](https://account.altvr.com/worlds/my)します。 テンプレートとして [ **Hello World テンプレート** ] を選択します。

![作成されたワールド画面](images/unity-uploader-img-02.png)

## <a name="upload-your-scene"></a>シーンのアップロード

> [!NOTE]
> 詳細なステップバイステップガイドについては、 [こちら](https://buildingthemetaverse.medium.com/how-to-make-your-own-altspace-templates-and-kits-unity-2020-3-9-uploader-2-x-5b40e92bb759)を参照してください。

1. Unity Hub を開き、新しい Unity 2020.3.9 プロジェクトを作成します。 テンプレートについては、[ **ユニバーサルレンダリングパイプライン**] を選択します。

    ![URP Unity テンプレートを選択する](images/001-unity-templates.png)

1. Altspace アップローダーをダウンロードしたフォルダーに移動し、そのフォルダーから新しい Unity プロジェクトのルートフォルダーにコピーまたは移動します。
1. Unity のメニューバーで、[ **Window** パッケージマネージャー] を選択し  >  **ます。**
1. パッケージマネージャーのメニューバーで、プラス記号ドロップダウン ("+") を選択し、[ **tar からパッケージを追加**] を選択します。
1. Altspace アップローダーが格納されているフォルダーに移動し、アップローダーを選択して、[ **開く**] をクリックします。  パッケージが読み込まれると、メニューバーに [ **altspace Evr** ] が表示されます。

    ![メニューバーの Altspace Evr](images/002-altspacevr-on-menu-bar.png)

> [!NOTE]
> Altspace アップローダーパッケージは、Altspace で使用するすべての Unity プロジェクトにインポートする必要があります。
1. メニューバーで、[ **Altspace Evr > Templates**] を選択します。
1. [ **ALTSPACE VR Templates** ] ダイアログボックスで、altspace アカウントの資格情報を使用してサインインします。 (MSA ログインはまもなく利用可能になります。 Microsoft アカウントで Altspace にログインしたことがない場合は、web サイトの [パスワードを忘れた場合] オプションを使用してパスワードを作成する必要があります)。
1. [ **テンプレートの選択** ] ドロップダウンをクリックし、[ **Hello World テンプレート**] を選択します。
1. シーンを選択する: [ **unity ファイルを選択します**] の省略記号ボタン (3 つの点) をクリックし、プロジェクトの [**アセット**] シーンフォルダーに移動して、  >   **SampleScene** を選択して開きます。
1. [**プラットフォーム用のビルド**] で、 **Windows** が選択されていることを確認します。 ここでは、他の2つのオプションである **Android** と **Mac** を **選択しないでください。** ユーザーがアクセスできるようにするには、すべてのプラットフォームに対してビルドとアップロードを行う必要があります。 "
1. [**ビルド & アップロード**] ボタンを選択します。 このプロセスには 1 ~ 2 分かかることがあります。
1. [Altspace] を起動し、 **メインメニュー** を選択してから、メニューバーで [ **マイワールド**] を選択します。
1. **Hello World** に移動して開きます。

    シーンは、Unity エディターで表示されているものと似ている必要があります。

## <a name="whats-supported"></a>サポートされる操作

* はい: モデル、競合、アニメーション、パーティクル効果、オーディオ、skyboxes など。
* いいえ: スクリプト。 セキュリティ上の理由から、スクリプトを含むアップロードは拒否されます。
* 場合によっては、動的なグローバル照明のような凝ったものです。
* 異なるプラットフォームのシーンを個別またはまとめてアップロードます。
* [おすすめのワールド](https://account.altvr.com/worlds/featured)をご覧ください。 多くはアップローダーを使用して構築されています。

## <a name="tips"></a>ヒント

* 公式の [Altspacevr Discord](https://discordapp.com/invite/altspacevr)に参加します。
* 左側の [テンプレート] ページに、プラットフォーム別の最新のアップロードが表示されます。 成功した場合は、 **1-2 分前** に表示されます。 

![アップロードが強調表示された状態で開く [テンプレート] パネル](images/template-upload-list.png)

* を更新するときに、その中でも使用できます。 アップローダーが **完了アップロード** と表示されたら、世界をリセットして変更を確認することができます。
* 単純なシーンでのみ PC 用にビルドする場合、Altspace の変化を確認するには1分未満である必要があります。
* 取られるを避けるために、世界をプライベートに設定し、一覧から削除します。
* 既定でユーザーが生成する場所を確認できるように、キューブを配信元に配置します。 アップロード時にキューブを非表示にします。

## <a name="troubleshooting"></a>トラブルシューティング

**何かを挿入することはできません。** オブジェクトへの競合を追加して、それらにテレポートする必要があります。

**何も変更されません**
    * Unity にシーンを保存しましたか?
    * テスト対象のプラットフォームを選択しましたか?
    * お持ちの方は、 アップローダーと World 形式で適切なテンプレートを選択しましたか?
    * テンプレートページの統計情報を確認しましたか?

**アップロードの失敗またはタイムアウト**
    * 最も一般的なアップロードエラーは、Unity バージョンが正しくないことが原因です。 必要なバージョンと正確に一致させる必要があります。
    * アップロードが大きすぎる可能性があります。 PC のシーン < 100 MB に保つようにしてください。 小規模に開始し、構築します。 Optimize、optimize、optimize。
    * 単純なキューブを含む新しいプロジェクトを試してみてください。
    * ビルド中に強制的に終了しないでください。シーンを破損させることができます。 再アップロードしてみてください。

**処理速度が遅い**
    * 後で Android を反復処理する場合にのみ、PC 用にビルドすることをお勧めします。
    * 未使用のファイルを削除してみてください。 何らかの理由により、Unity は熱心になることがあります。

**Altspace 資格情報でサインインできません**
    * 電子メールでは大文字と小文字が区別されます。
    * 新しいプロジェクトを試してみてください。
    * Altspace アカウントが良好な場所にあることを確認します。

## <a name="see-also"></a>こちらもご覧ください

* [Unity Learn](https://unity3d.com/learn)
* [Unity フォーラム](https://forum.unity.com)  
