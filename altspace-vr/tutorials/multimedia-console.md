---
title: マルチメディア コンソールの使用
description: AltspaceVR エクスペリエンスでマルチメディア コンソールの構成、発行、制御を開始する方法について説明します。
ms.date: 03/11/2021
ms.topic: article
keywords: コンソール、マルチメディア
ms.openlocfilehash: 4a51ff76e44d3870972bc17288ae77c1fa888922
ms.sourcegitcommit: 2db596ab5a1ecd4901a8c893741cc4d06f6aecea
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2021
ms.locfileid: "112923009"
---
# <a name="using-the-multimedia-console"></a>マルチメディア コンソールの使用

マルチメディア コンソールは、イベントや世界でのメディア共有を可能にするツールです。 画像、プレゼンテーション スライド、ライブストリーム、ビデオ、プレイリストなど、その他を共有するために使用できます。 マルチメディア コンソール **v0.5.0+** の使い方の詳細な手順を次に示します。 

## <a name="getting-started"></a>はじめに

マルチメディア コンソールの使用は、2 部構成のプロセスです。  まず、環境に配置するマルチメディア コンソール セッションの構成を生成して発行するために使用する Web ポータルがあります。  2 つ目は、実際のマルチメディア コンソール アプリを環境内に配置し、使用する必要がある構成コードを設定する方法です。

### <a name="configuring-the-multimedia-console-with-the-web-portal"></a>Web ポータルを使用したマルチメディア コンソールの構成

1. まず、URL が必要なので、コンテンツがオンラインでホストされている必要があります。 (画像に写真をアップロード altvr.com、オンラインでビデオ .mp4ホストしたり、Dlive ライブ ストリーム リンクを使用することができます。 https://dlive.tv/yourlivestream) 
2. マルチメディア コンソールの Web ポータル () に移動します。 [https://multimedia-console.altvr.com/](https://multimedia-console.altvr.com/)
3. Web ポータルから、マルチメディア コンソールの構成を生成して発行できます。  (さまざまなプロパティの詳細については、以下を参照してください)。
4. メディアの一覧にメディアを入力し、全般設定を構成したら、アプリの上部にある [発行] ボタンを選択します。
5. 発行が完了すると、配置したマルチメディア コンソールに入力する 2 つの単語コードがダイアログに表示されます。
  
### <a name="placing-the-multimedia-console-in-your-environment"></a>環境にマルチメディア コンソールを配置する

1. [World **Editor]/(ワールド エディター> エディター パネル> SDK Apps > マルチメディア コンソール] を選択します**。 ([World Editor > Basics > **SDK App(** 登録されていないアプリの場合) に移動しない。  
2. 空間と対象ユーザーに最適なマルチメディア コンソールを配置します。
3. オレンジ色の [編集モード] ボタンをクリックして、編集モードから抜け出します。
4. メディア プレーヤーの所有者ですか **? というメッセージが表示されます。** このマルチメディア コンソール セッションの正式な所有者である必要があるユーザーは、確認して続行します。 (その他のアクセス許可ロールも使用できます。 詳細な一覧については、以下を参照してください)。
5. [はい] を選択して、プライマリ ホストを確認します。  
6. Web ポータルまたは有効な JSON からコードを入力するダイアログが表示されます。  Web ポータルからダッシュを含む 2 つの単語コードを入力し、[OK] をクリックします。 (JSON は、以下で説明する高度な構成です)
7. マルチメディア コンソールは、Web ポータルで構築した構成で数秒後に読み込む必要があります。

### <a name="controlling-the-multimedia-console"></a>マルチメディア コンソールの制御

1. コードを入力して構成プロセスを完了すると、メディアディスプレイの下にコントロール ボタンが表示されます。 
    * **再生** によってメディア ビューアーが開始されます (または、以前に停止した場合は現在のエントリで再起動します) 
    * **[停止** ] を選択すると、メディア ビューアーが停止し、現在のメディアが非表示にされます。  
    * **Next/Prev は** 次のメディアまたは前のメディアにスキップします 
    * **x/x**  では、現在のインデックスがメディア リストに表示され、リスト内の任意のポイントにジャンプできます。
    * **構成** を使用すると、Web ポータルから新しいコードを再入力して、コンソールで新しい構成を設定できます。 

これで、マルチメディア コンソールを使用して共有を開始します。  
 
## <a name="working-with-the-web-portal"></a>Web ポータルの操作

Web ポータルは、マルチメディア コンソールのさまざまな機能を構成できる Web アプリです。  これらの機能は 2 つのカテゴリに分類されます。一般的なメディア コンソール設定とメディア 再生リスト。

### <a name="multimedia-console-general-settings"></a>マルチメディア コンソールの全般設定

**再生設定**

メディア リストの一般的な再生設定

* **[メディアリストの** ループ] - リストの末尾に到達したら、メディア リストをループ処理するかどうかを決定します。
* **Start メソッド** - マルチメディア コンソールを開始する方法を選択します。
    * 手動 - メディアを起動する前に再生ボタンが押されるのを待ちます
    * [開始から自動開始] - 一覧の先頭からメディア リストを自動開始します
    * 自動開始ランダム - 一覧のランダムな開始点からメディアを自動開始します

**ロール**

マルチメディア コンソールを制御および構成するためのロールの割り当て。    これらのロールは、次のセットに分けらされます。

* **所有者のみ** - マルチメディア コンソール セッションの所有者であるユーザー
* **昇格されたユーザー** - マルチメディア コンソールが最初に構成されている領域にモデレーターまたはホスト ロールを持つユーザー
* **すべてのユーザー** - すべてのユーザー

これらのロールは、この一覧で選択したロールより上のすべてのロールにも、その機能を使用するためのアクセス許可が付与されるという意味でスタックします。  例:**管理者特権のユーザー** には、AltspaceVR のモデレーターまたはホストではない場合でも所有者が含まれます。  ロールの割り当てによって制御される機能は次のとおりです。

* **メディア プレーヤーを制御できる** - マルチメディア コンソールのメディア再生ボタンを制御できるロールを決定します
* **メディア プレーヤーを構成できる** - [構成] ボタンへのアクセスを許可することで、マルチメディア コンソールを構成できるロールを **決定** します

### <a name="adding-photos-and-videos-to-the-media-list"></a>メディア リストへの写真とビデオの追加

メディアはマルチメディア コンソールの中心です。  画像とビデオ リンクは、マルチメディア コンソール内でメディアの種類としてサポートされています。  新しいメディアを追加するには、[イメージの追加]アイコンまたは [ビデオの追加] アイコンを選択して、メディア情報と設定を入力するダイアログ をポップアップ表示します。  メディアの種類と関連する設定の内訳を次に示します。

**Image**

画像は、jpeg、png、および子などの標準的な画像の種類である必要があります。 パブリック リンクを使用してどこかでホストする必要があります。

* **名前** - (必須) イメージを識別する名前。
* **イメージ URL** - (必須) イメージのパブリック URL
* **Skip After** - イメージをスキップする必要がある時間 (秒)

**ビデオ**

ビデオは、Twitch と DLive を介してビデオまたはライブ ストリームをホストできます。  (その他のサポートは、適切なストリーム URL を取得するために追加の作業で機能する場合がありますが、マルチメディア コンソール内では完全にはサポートされていません)

* **名前** - (必須) ビデオを識別する名前。
* **ビデオ URL** - (必須) ビデオがホストされているパブリック URL。またはライブ ストリームが提供されます。
* **Skip After** - ビデオのスキップ後にスキップする必要がある時間 (秒)

> [!NOTE]
> 必須: ビデオの長さと一致する時間を入力して、ビデオを正しく転送します。 たとえば、ビデオの長さ 5 分が 300 秒の場合、ビデオは次のコンテンツにスキップされます。

* **ボリューム** - 0 (分) から 1 (最大) の値のビデオのボリューム。
* **[開始時刻** ] - ビデオの開始から開始する時間 (秒)。
* **Roll Off Start Distance** (開始距離のロールオフ) - マルチメディア コンソールから離れるとボリュームが落ち始める世界のメートルの距離
* **[End of Video Action]/(** ビデオの終了アクション)- ビデオの末尾に到達したら実行するアクション。
    * [停止] - ビデオが終了した後にメディアリストが停止します
    * ループ - ビデオは手動でスキップされるまでループします
    * [次へ再生] - メディアリスト内の次のメディアは、現在のビデオが終了した後に開始されます。

## <a name="working-with-json-directly-advancedoptional"></a>JSON を直接操作する (詳細/省略可能)

マルチメディア コンソールでは、AltspaceVR でコンソールのプロンプトに直接 JSON を入力できます。  JSON は、メディア プレーヤーの構成を有効にする内部メカニズムです。 JSON を直接設定する機能を公開することで、より高度なユーザーは、JSON に対するニーズと使い慣れた独自のワークフローを構築できます。  JSON 構造と JSON の検証に使用されるスキーマの簡単な説明を次に示します。 以下のプロパティの詳細については、マルチメディア コンソールの構成に関する上記のセクションを参照してください。  このセクションでは、主に JSON データのスキーマの例と構造化に重点を置いて説明します。

### <a name="global-media-settings"></a>グローバル メディア設定

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

メディア リストは、JSON 構造のルート (ロールや再生設定など) に設定されたプロパティです。  これは、次のいずれかのメディア構成構造を含む単純な配列です。 (それぞれの機能の詳細については、上記のプロパティの説明を参照してください)。

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