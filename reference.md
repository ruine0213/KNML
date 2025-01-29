# KNML Tag Reference

`<knml></knml>`\
`<html>`のようにすべてを包括するタグです。\
このタグの開始から終了までに内容を記述してください。\
All-encompassing tag, like `<html>`.\
Write the content between the start and end tags.

`<metadata></metadata>`\
メタデータ用のタグです。\
タイトルや作者名等の情報を記述してください。\
Metadata tag.\
Describes information such as title, author, and staff.

`<title>Adventures of Huckleberry Finn</title>`\
タイトル用のタグです。\
Title tag.

`<icon img="res://image/icon.png"/>`\
作品を示すアイコン画像用のタグです。これは空タグです。\
img属性には画像ファイルを指定してください。\
Icon tag. This tag is empty.\
img attribute specifies the image file.

`<author>Mark Twain</author>`\
作者名用のタグです。\
共作の場合、代表者の名前を記載してください。\
Author name tag.\
If collaborative, name of representative.

`<staff></staff>`\
参加者の名前用タグです。役割に応じて記載してください。\
Staffs name tag. Listed by role\
`<writer>Mark Twain</writer>`\
`<artist>Edward Windsor</artist>`\
`<composer></composer>`

`<description>The adventures of the boy Huck and the runaway slave Jim</description>`\
作品説明用のタグです。\
読者が読みたくなるような紹介を書いてください。\
Product discription tag.\
Write an introduction that will make your readers want to read it.

`<published>1884-12-10</published>`\
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

`<background img="res://image/background01.png"/>`\
背景画像用タグです。これは空タグです。\
img属性は画像ファイルを指定してください。\
Background image tag. This tag is empty.\
img attribute specifies the image file.

`<sound track="res://sound/BGM01.ogg" loop="true"/>`\
音声用タグです。これは空タグです。\
track属性は音声ファイルを指定してください。\
loop属性はループさせるかどうかを指定します。デフォルトはfalseです。\
Sound tag. This tag is empty.\
track attribute specifies the sound file.\
loop attribute determines whether to loop. Default is false.

`<character name="Watson" img="res://image/Watson.png" position="center"/>`\
キャラクターの立ち絵用タグです。これは空タグです。\
name属性はキャラクターの名前を記載します。\
img属性は画像ファイルを指定してください。\
position属性は左、右、中央からキャラクターの立ち位置を選んでください。\
Character sprite tag. This tag is empty.\
name attribute is note of the character's name.\
img attribute specifies the image file.\
position attribute allows you to choose the character's position from left, right, or center.

`<paragraph>You don’t know about me without you have read a book by the name of The Adventures of Tom Sawyer; but that ain’t no matter. That book was made by Mr. Mark Twain, and he told the truth, mainly. There was things which he stretched, but mainly he told the truth. That is nothing. I never seen anybody but lied one time or another, without it was Aunt Polly, or the widow, or maybe Mary. Aunt Polly—Tom’s Aunt Polly, she is—and Mary, and the Widow Douglas is all told about in that book, which is mostly a true book, with some stretchers, as I said before.</paragraph>`\
地の文の段落用タグです。\
実際の文章を書いてください。\
Narrative paragraph tag.\
Write the actual text.

`<dialogue cast="Watson" voice="res://sound/WatsonVoice001.ogg">Don’t put your feet up there, Huckleberry;</dialogue>`\
セリフ用タグです。\
cast属性は喋るキャラクターの名前を記載します。\
voice属性はボイスファイルを指定してください。\
Words spoken by characters tag.\
cast attribute is note of the character's name.\
voice attribute specifies the voice file.

`<wait time="10"/>`\
待機用タグです。これは空タグです。\
time属性には待機時間を秒で指定してください。\
Wait tag. This tag is empty.\
time attribute specifies the wait time in seconds

`<break/>`\
改ページタグです。これは空タグです。\
Page break tag. This tag is empty.

`<transition rule="res://image/wipe.png"/>`\
トランジションタグです。これは空タグです。\
rule属性にはトランジションルール用画像を指定してください。\
transition tag. This tag is empty.\
rule attribute specifies the transition rule image file.
