# KNML Tag Reference

## ルート要素root
### `<knml></knml>`
`<html>`のようなKNML文書の最上位要素です。\
このタグの開始から終了までにすべての内容を記述してください。\
This is the top-level element of the KNML document like `<html>`.\
Write all contents between the start and end tags.

## 上位要素higher level
`<knml>`タグの直下にそれぞれひとつずつ配置します。\
Place each one directly under the `<knml>`tag.
### `<metadata></metadata>`
タイトルや作者名等の作品情報のためのタグです。\
These are tags for work information such as the title and author name.
### `<cover></cover>`
表紙(タイトル画面)のデザインを決めるタグです。\
Determines the design of the cover (title screen).
### `<body></body>`
小説本体を記述するタグです。\
Describes the novel itself.

## メタデータ要素metadata
`<metadata>`タグの直下にそれぞれひとつずつ配置します。\
Place each one directly under the `<metadata>`tag.
### `<title></title>`
作品の題名を記述します。\
Enter the title of the work.
### `<icon img="res://image/icon.png"/>`
書影の代わりとなるアイコンを指定します。\
Specify an icon to replace the book image.
### `<author></author>`
作者名もしくは共作の場合代表者名を記述します。\
Write the author's name or the representative name if it is a collaborative work.
### `<staff></staff>`
スタッフ全員の名前を記述します。\
List the names of all staff members.
+ `<writer></writer>`小説本文の著者
+ `<artist></artist>`イラストレーター
+ `<composer></composer>`作曲者
### `<description></description>`
作品の簡単な説明を記述します。\
Describes product discription.
### `<published></published>`
作品の公開日をYYYY-MM-DD形式で記載します。\
Enter the release date of the work in YYYY-MM-DD format.

## 表紙要素cover
`<cover>`タグの直下にそれぞれひとつずつ配置します。\
Place each one directly under the `<cover>`tag.
### `<background img="res://image/cover.png"/>`
表紙画像ファイルを指定します。\
Specify the cover image file.
### `<sound track="res://sound/BGM00.ogg"/>`
ループ再生される音楽ファイルを指定します。\
Specifies the music file to be played in a loop.

## 本体要素body
`<body>`タグの直下に任意の数配置できます。\
シーンもしくは動画から始めて、トランジションと交互に配置してください。\
Any number of them can be placed directly under the `<body>`tag.\
Start with your scenes or videos and alternate them with transitions.
### `<scene number="1" bgm="res://sound/BGM01.ogg"></scene>`
シーンのためのタグです。通し番号とループ再生される音楽を指定します。
This is a tag for a scene. Specify the serial number and the music that will play on a loop.
### `<video src="res://video/OP.mp4"/>`
再生する動画を指定します。\
Specify the video to play.
### `<transition rule="res://image/wipe.png"/ time="1">`
トランジションのルール用画像と遷移時間を指定します。\
Specify the image and transition time for the transition rule.

## シーン要素scene
`<scene>`タグの直下に任意の数配置できます。\
カットとトランジションを交互に配置してください。\
Any number of them can be placed directly under the `<scene>`tag.\
Alternate cuts and transitions.
### `<cut></cut>`
ひとつのカットを配置します。\
Place one cut.
### `<transition rule="res://image/wipe.png"/ time="1">`
トランジションのルール用画像と遷移時間を指定します。\
Specify the image and transition time for the transition rule.

## カット要素cut
`<cut>`タグの直下に任意の数配置できます。\
Any number of them can be placed directly under the `<cut>`tag.
### `<background img="res://image/background01.png"/>`
背景を画像もしくは色で指定します。例外として`<cut>`タグ内の最初にひとつだけ記述してください。\
Specify the background as an image or color. As an exception, write only one at the beginning of the `<cut>` tag.
### `<sound track="res://sound/SE01.wav"/>`
効果音を指定します。\
Specifies the sound effect.
### `<enter cast="Watson" img="res://image/Watson.png" position="center"/>`
キャラクターの入場タイミングに画像と立ち位置を指定します。\
Specify an image and position when a character enters.
### `<act cast="Watson" img="res://image/Watson.png" position="right"/>`
入場したキャラクターの画像や立ち位置を変更します。\
Change the image and position of the entering character.
### `<exit cast="Watson"/>`
キャラクターを退場させます。\
Exit the character.
### `<paragraph></paragraph>`
地の文の段落を記述します。\
Write the narrative paragraph.
### `<dialogue cast="Watson" voice="res://sound/WatsonVoice001.wav"></dialogue>`
キャラクターのセリフを記述し、必要があればボイスファイルを指定します。\
Write the character's lines and specify a voice file if necessary.
### `<wait time="10"/>`
待機時間を指定します。\
Specify the wait time.
### `<break/>`
改ページを指定します。\
Specify the page break.
