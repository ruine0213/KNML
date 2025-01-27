# KNML(Kinetic Novel Markup Language)
KNMLはキネティックノベル用の標準スクリプトを目指して開発中のXMLベースのマークアップ言語です。\
(キネティックノベルとは、絵と音を組み合わせた小説で選択肢のないものを言います)\
KNML is an XML-based markup language currently under development that aims to be a standard for Kinetic Novel scripting.\
(Kinetic Novel is a digital novel that combines pictures and sound and has no choices)

エンジンもビューアもまだありません。ご自身で開発してください！\
There is no engine, no viewer yet. Develop it yourself!

## Template
```xml:sample.knml
<?xml version="1.0" encoding="UTF-8"?>
<knml>
	<metadata>
		<title>タイトル</title>
		<icon img="アイコン画像ファイル"/>
		<author>作者(代表者)</author>
		<staff>
			<writer>著者</writer>
			<artist>イラストレーター</artist>
			<composer>作曲家</composer>
		</staff>
		<description>作品説明</description>
		<published>2025-01-27</published>
	</metadata>
	<body>
		<scene number="1">
			<background img="背景画像ファイル"/>
			<sound track="BGMファイル" loop="true"/>
			<character name="キャラ名" img="画像ファイル" position="立ち位置"/>
			<paragraph>地の文の段落</paragraph>
			<dialogue cast="キャラ名" voice="音声ファイル">セリフ</dialogue>
			<sound track="効果音ファイル"/>
			<break/>
			<paragraph>地の文の段落</paragraph>
			<dialogue cast="キャラ名" voice="音声ファイル">セリフ</dialogue>
		</scene>
		<transition rule="ルール画像ファイル"/>
		<scene number="2">
		</scene>
	</body>
</knml>
```

## Tags
`<knml> </knml>`\
`<html>`のようにすべてを包括するタグです。\
このタグの開始から終了までに内容を記述してください。\
All-encompassing tag, like `<html>`.\
Write the content between the start and end tags.

`<metadata></metadata>`\
メタデータ用のタグです。\
タイトルや作者名等の情報を記述してください。\
Metadata tag.\
Describes information such as title, author, and staff.

`<title></title>`\
タイトル用のタグです。\
Title tag.

`<icon img="icon.png"/>`\
アイコン画像用のタグです。これは空タグです。\
img属性には画像ファイルを指定してください。\
Icon tag. This tag is empty.\
img attribute specifies the image file.

`<author></author>`\
作者名用のタグです。\
共作の場合、代表者の名前を記載してください。\
Author name tag.\
If collaborative, name of representative.

`<staff></staff>`\
参加者の名前用タグです。役割に応じて記載してください。\
Staffs name tag. Listed by role\
`<writer></writer>`\
`<artist></artist>`\
`<composer></composer>`

`<description></description>`\
作品説明用のタグです。\
読者が読みたくなるような紹介を書いてください。\
Product discription tag.\
Write an introduction that will make your readers want to read it.

`<published></published>`\
公開日用タグです。YYYY-MM-DDの形式で書いてください。\
Publication day tag. YYYY-MM-DD format.

`<body></body>`\
小説本編用のタグです。\
シーンごとに分けて記述してください。\
Body tag. Main Story is here.\
Described by scene.

`<scene number="1"></scene>`\
シーン用タグです。実際の内容はこの中に記述してください。\
number属性は通し番号を表現します。\
Scene tag. Describe the actual content.\
number attribute is expressing serial numbers.

`<background img="background01.png"/>`\
背景画像用タグです。これは空タグです。\
img属性は画像ファイルを指定してください。\
Background image tag. This tag is empty.\
img attribute specifies the image file.

`<sound track="BGM01.ogg" loop="true"/>`\
音声用タグです。これは空タグです。\
track属性は音声ファイルを指定してください。\
loop属性はループさせるかどうかを指定します。デフォルトはfalseです。\
Sound tag. This tag is empty.\
track attribute specifies the sound file.\
loop attribute determines whether to loop. Default is false.

`<character name="Watson" img="Watson.png" position="left"/>`\
キャラクターの立ち絵用タグです。これは空タグです。\
name属性はキャラクターの名前を記載します。\
img属性は画像ファイルを指定してください。\
position属性は左、右、中央からキャラクターの立ち位置を選んでください。\
Character sprite tag. This tag is empty.\
name attribute is note of the character's name.\
img attribute specifies the image file.\
position attribute allows you to choose the character's position from left, right, or center.

`<paragraph></paragraph>`\
地の文の段落用タグです。\
実際の文章を書いてください。\
Narrative paragraph tag.\
Write the actual text.

`<dialogue cast="Watson" voice="WatsonVoice001.ogg"></dialogue>`\
セリフ用タグです。\
cast属性は喋るキャラクターの名前を記載します。\
voice属性はボイスファイルを指定してください。\
Words spoken by characters tag.\
cast attribute is note of the character's name.\
voice attribute specifies the voice file.

`<break/>`\
改ページタグです。これは空タグです。\
Page break tag. This tag is empty.

`<transition rule="wipe.png"/>`\
トランジションタグです。これは空タグです。\
rule属性にはトランジションルール用画像を指定してください。\
transition tag. This tag is empty.\
rule attribute specifies the transition rule image file.
