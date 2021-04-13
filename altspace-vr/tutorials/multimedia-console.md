---
title: マルチメディアコンソールの使用
description: 職場でのマルチメディアコンソールの構成、発行、および管理を開始する方法について説明します。
ms.date: 03/11/2021
ms.topic: article
keywords: コンソール、マルチメディア
ms.openlocfilehash: 601328eb6f266dbcfc9d81fc4f1c2d09ac62b318
ms.sourcegitcommit: d84a6adf631ff02b106e682238f2861477caef1e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2021
ms.locfileid: "107212839"
---
# <a name="using-the-multimedia-console"></a>マルチメディアコンソールの使用

マルチメディアコンソールは、イベントや世界でメディアの共有を可能にするツールです。 この機能を使用して、イメージ、プレゼンテーションスライド、livestreams、ビデオ、再生リストなどの項目を共有できます。 マルチメディアコンソール **v 0.5.0 +** を使用する手順を次に示します。 

## <a name="getting-started"></a>作業の開始

マルチメディアコンソールの概要は、2つの部分で構成されています。  まず、環境に配置するマルチメディアコンソールセッションの構成を生成して公開するために使用する web ポータルがあります。  2つ目は、実際の環境における実際のマルチメディアコンソールアプリの配置と、使用する構成コードの設定です。

### <a name="configuring-the-multimedia-console-with-the-web-portal"></a>Web ポータルを使用したマルチメディアコンソールの構成

1. まず、URL が必要になるので、コンテンツがオンラインでホストされていることを確認する必要があります。 (写真を altvr.com にアップロードしたり、ビデオ. mp4 ファイルをオンラインでホストしたり、Twitch ライブストリームリンクを使用したりすることができます。 https://www.twitch.tv/ninja) 
2. でマルチメディアコンソールの web ポータルに移動します。 [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)
3. Web ポータルから、マルチメディアコンソールの構成を生成して公開することができます。  (さまざまなプロパティの詳細については、以下を参照してください)。
4. メディアの一覧にメディアを入力し、全般設定を構成したら、アプリの右上にある [発行] ボタンを選択します。
5. 発行が完了すると、ダイアログが表示され、配置したマルチメディアコンソールに入力する2つの単語のコードが表示されます。
  
### <a name="placing-the-multimedia-console-in-your-environment"></a>環境にマルチメディアコンソールを配置する

1. [ **ワールドエディター] > エディターパネル > [SDK アプリ > マルチメディアコンソール**] を選択します。 (登録されていないアプリの場合は、[ **> の基本] > [SDK アプリ**] を参照してください)。  
2. スペースと対象ユーザーに最適なマルチメディアコンソールを配置します。
3. 編集モードを終了するには、オレンジ色の編集モードボタンをクリックします。
4. **Media player の所有者であるかどうか** を確認するメッセージが表示されます。 このマルチメディアコンソールセッションの正式な所有者になるユーザーの方は、確認してから続行してください。 (他の与えロールも利用できます。 詳細な一覧については、以下を参照してください。)
5. [はい] を選択して、プライマリホストであることを確認します。  
6. ダイアログがポップアップ表示され、web ポータルまたは有効な JSON からコードを入力するように求められます。  ダッシュを含む2つの単語コードを web ポータルから入力し、[OK] をクリックします。 (JSON は、以下で説明する高度な構成です)
7. マルチメディアコンソールは、web ポータルで作成した構成で数秒後にロードされます。

### <a name="controlling-the-multimedia-console"></a>マルチメディアコンソールの制御

1. コードを入力して構成プロセスを完了すると、メディアディスプレイの下にコントロールボタンが表示されます。 
    * **Play** はメディアビューアーを開始します (以前に停止した場合は、現在のエントリで再起動します) 
    * [**停止**] を行うと、メディアビューアーが停止し、現在のメディアは非表示になります。  
    * **次** または前のメディアにスキップ 
    * **x/x**  メディア一覧の現在のインデックスを表示し、一覧内の任意のポイントに移動できるようにします。
    * **構成** を使用すると、web ポータルから新しいコードを再利用して、コンソールで新しい構成を設定できます。 

これで、マルチメディアコンソールを使用して共有を開始するように設定されました。  
 
## <a name="working-with-the-web-portal"></a>Web ポータルでの作業

Web ポータルは、マルチメディアコンソールのさまざまな機能を構成できる web アプリです。  これらの機能は2つのカテゴリに分類されます。一般的なメディアコンソール設定とメディア再生リスト。

### <a name="multimedia-console-general-settings"></a>マルチメディアコンソールの全般設定

**再生設定**

メディア一覧の全般的な再生設定

* [**メディア一覧のループ]**-一覧の末尾に達すると、メディアリストをループするかどうかを決定します。
* **Start メソッド** -マルチメディアコンソールを起動する方法を選択します。
    * Manual-メディアを開始する前に [再生] ボタンが押されるのを待ちます。
    * [開始から自動開始]-一覧の先頭からメディアリストを自動的に開始します
    * 自動開始ランダム-リスト内のランダムな開始位置からメディアを自動で開始します。

**ロール**

マルチメディアコンソールを制御および構成するためのロールの割り当て。    これらのロールは、次のセットに分類されます。

* **所有者のみ** -マルチメディアコンソールセッションの所有者であるユーザー
* **管理者特権** を持つユーザー-最初にマルチメディアコンソールが構成されている領域に、モデレーター、ホスト、またはプレゼンターの役割を持つユーザー
* **すべてのユーザー** -すべてのユーザー

これらのロールは、この一覧で選択されたロールの上にあるすべてのロールにも、その機能を使用するためのアクセス許可が付与されるという意味でスタックします。  例: **管理者特権** を持つユーザーには、メンバーがモデレーター、ホスト、または講師 * * でない場合でも、この **所有者** が含まれます。 ロールの割り当てによって制御される機能を次に示します。

* **メディアプレーヤーを制御できる** -マルチメディアコンソールのメディア再生ボタンを制御できるロールを決定します。
* **メディアプレーヤーを構成できる** **-[構成] ボタン** へのアクセスが許可されている場合に、マルチメディアコンソールを構成できるロールを決定します。

### <a name="adding-photos-and-videos-to-the-media-list"></a>メディアリストへの写真とビデオの追加

メディアは、マルチメディアコンソールの中核です。  イメージとビデオリンクは、マルチメディアコンソール内でメディアの種類としてサポートされています。  新しいメディアを追加するには、[ **イメージの追加** ] または [ビデオアイコンの **追加** ] を選択して、メディア情報と設定を入力するためのダイアログをポップアップ表示します。  メディアの種類と関連する設定の内訳を次に示します。

**イメージ**

画像は、jpeg、png、son などの標準のイメージの種類である必要があります。 パブリックリンクを使用して、どこかにホストする必要があります。

* **Name** -(必須) イメージを識別する名前。
* **イメージの url** -(必須) イメージのパブリック URL
* [**後にスキップ** する-イメージがスキップされるまでの秒数

**ビデオ**

ビデオは、Twitch と DLive を使用してビデオやライブストリームにすることができます。  (他のサポートが適切なストリーム url を取得するために余分な作業で機能する場合がありますが、マルチメディアコンソール内で完全にはサポートされていません)

* **名前** -(必須) ビデオを識別する名前。
* **ビデオ url** -(必須) ビデオがホストされている、またはライブストリームが提供されるパブリック URL。
* **スキップ後** -ビデオがスキップされるまでの秒数
* **Volume** -0 (最小)-1 (max) の値からのビデオのボリューム。
* **開始時刻** -ビデオの開始から開始するまでの秒数。
* [**開始距離のロールオフ**-マルチメディアコンソールから移動したときにボリュームがオフになる世界のメーターの距離。
* **ビデオの終了操作** -ビデオの終わりに達したときに実行するアクション。
    * [停止]-ビデオが終了した後、メディアの一覧が停止します。
    * Loop-ビデオは手動でスキップされるまでループします。
    * [次に再生]-現在のビデオが終了した後に、メディアリスト内の次のメディアが開始されます。

## <a name="working-with-json-directly-advancedoptional"></a>JSON を直接操作する (詳細設定/省略可能)

マルチメディアコンソールでは、Altthe Console のプロンプトに直接、JSON を入力できます。  JSON は、media player の構成を有効にするための内部メカニズムです。 JSON を直接設定する機能を公開することは、より高度なユーザーが独自のワークフローを構築して、そのニーズを満たすと共に JSON を理解できるようにするものです。  Json の構造と JSON の検証に使用されるスキーマについての簡単な説明を次に示します。 以下のプロパティの詳細については、マルチメディアコンソールの構成について説明している上記のセクションを参照してください。  このセクションでは、主に、JSON データのスキーマの例と構造に焦点を絞って説明します。

### <a name="global-media-settings"></a>グローバルメディアの設定

```json
{
  "loopMediaList": true | false
  "startMethod": "manual" | "autostart-beginning" | "autostart-random"
  "controlMediaPlayer": "everyone" | "elevated" | "owner"
  "configureMediaPlayer": "elevated" | "owner"
  ...
}
```

### <a name="media-list"></a>メディア一覧

メディアの一覧は、ロールや再生の設定など、JSON 構造のルートで設定されたプロパティです。  これは、次のいずれかのメディア構成構造を含むことができる単純な配列です。 (それぞれの機能の詳細については、上記のプロパティの説明を参照してください)。

**画像の例**

*必須フィールド: "name" および "imageUrl"*

```json
{
    "name": "Altspace Screenshot",
    "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
    "skipAfter": 10
}
```

**ビデオの例**

*必須フィールド: "name" および "videoUrl"*

```json
{
    "name": "Ninja Twitch Live Stream",
    "videoUrl":"https://www.twitch.tv/ninja",
    "volume":0.2,
    "startTime":0,
    "endOfVideoAction":"play-next"
}
```

### <a name="example-json"></a>JSON の例

```json
{
  "loopMediaList": false,
  "startMethod": "autostart-beginning",
  "controlMediaPlayer": "everyone",
  "configureMediaPlayer": "elevated",
  "mediaList": [
    {
      "videoUrl": "https://www.twitch.tv/ninja",
      "volume": 0.2,
      "startTime": 0,
      "endOfVideoAction": "play-next"
    },
    {
      "imageUrl": "http://www.hypergridbusiness.com/wp-content/uploads/2016/09/AltspaceVR-highrise.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://d1qb2nb5cznatu.cloudfront.net/startups/i/333629-6ffd7199b9bcf34d8957e8e09d974a38-medium_jpg.jpg?buster=1423092095",
      "skipAfter": 5
    },
    {
      "imageUrl": "https://pbs.twimg.com/media/CxJ-fJqUsAAFtd9.jpg",
      "skipAfter": 10
    },
    {
      "imageUrl": "https://altvr-wpengine.netdna-ssl.com/wp-content/uploads/2019/05/Educators-in-VR-Social-VR-AltspaceVR.png",
      "skipAfter": 10
    },
    {
      "videoUrl": "https://www.twitch.tv/shroud",
      "volume": 1,
      "startTime": 0,
      "endOfVideoAction": "stop"
    }
  ]
}
```

### <a name="schema"></a>スキーマ

```json
{
  "$schema": "https://json-schema.org/draft-04/schema#",
  "type": "object",
  "required": [
    "mediaList"
  ],
  "properties": {
    "loopMediaList": {
      "type": "boolean",
      "description": "Whether to loop through the media list when reaching the beginning or end of the list."
    },
    "controlMediaPlayer": {
      "type": "string",
      "enum": [
        "everyone",
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are able to control the media player. (Owner can always control player)"
    },
    "configureMediaPlayer": {
      "type": "string",
      "enum": [
        "elevated",
        "owner"
      ],
      "default": "owner",
      "description": "What roles are allowed to configure the media play list.  Note: This role needs to be able to control the media player in order to configure it. (Owner can always configure media)"
    },
    "startMethod": {
      "type": "string",
      "enum": [
        "manual",
        "autostart-beginning",
        "autostart-random"
      ],
      "default": "manual",
      "description": "The method by which the media player should start"
    },
    "mediaList": {
      "description": "A list of images or videos to configure the media player to operate on.",
      "type": "array",
      "items": {
        "oneOf": [
          {
            "title": "Image",
            "type": "object",
            "description": "Configuration for an image media.",
            "properties": {
              "imageUrl": {
                "type": "string",
                "description": "The url for the image to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              }
            },
            "required": [
              "imageUrl"
            ]
          },
          {
            "title": "Video",
            "type": "object",
            "description": "Configuration for a video media.",
            "properties": {
              "videoUrl": {
                "type": "string",
                "description": "The url of the video to load."
              },
              "skipAfter": {
                "type": "number",
                "minimum": 5,
                "default": null,
                "description": "The number of seconds that should pass before skipping to the next media. (Minimum 5)."
              },
              "volume": {
                "type": "number",
                "minimum": 0,
                "maximum": 1,
                "default": null,
                "description": "The volume to play the video at. (Minimum 0, maximum 1)"
              },
              "startTime": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The time in seconds from the start of the video to begin playing the video at. (Minimum of 0)"
              },
              "rolloffStartDistance": {
                "type": "number",
                "minimum": 0,
                "default": null,
                "description": "The distance in meters away from the media player that the volume will begin to fall off. (Minimum 0)"
              },
              "endOfVideoAction": {
                "type": "string",
                "enum": [
                  "stop",
                  "loop",
                  "play-next"
                ],
                "default": null,
                "description": "The type of action to take at the end of the video."
              }
            },
            "required": [
              "videoUrl"
            ]
          }
        ]
      }
    }
  }
}
```

> [!NOTE]
> マルチメディアコンソール v 0.5.0 を使用した最新の状態