# KNML(Kinetic Novel Markup Language)

## 概要
KNMLはキネティックノベル[^1]をHTMLのように記述して作成することができるようにするためのマークアップ言語仕様です。\
小説本文・画像・音楽などを用意し、それらを一連の作品として組み合わせるためのものです。\
エンジンの実装はまだありませんが、将来的にひとつのビューアですべての作品が読めることを目指しています。\
KNML is a markup language specification that allows kinetic novels[^1] to be written and created in a way similar to HTML.\
It is designed to allow you to prepare the novel text, images, music, etc. and combine them into a series of works.\
The engine has not yet been implemented, but in the future we aim to make it possible to read all works with a single viewer.\

[^1]: キネティックノベルとは、絵と音を組み合わせた小説で選択肢のないものを言います\
Kinetic Novel is a digital novel that combines pictures and sound and has no choices

## データ形式について
KNMLの実体はEPUBのようなZIPアーカイブ形式です。\
アーカイブの中にはメタデータとコンテンツそれぞれを記述したKNML文書(XML形式)とサムネイル用画像(PNG形式)を最低限含みます。\
詳細はsampleディレクトリを確認してください。\
KNML is a ZIP archive format similar to EPUB.\
The archive contains at least a KNML document (XML format) describing the metadata and content, and a thumbnail image (PNG format).\
See sample directory for more infomation.

## 協力のお願い
言語仕様の開発および実際に動かすためのエンジンの開発に協力していただける方を募集しています。\
We are looking for people who can cooperate in developing the language specification and the engine that will actually run it.

[Sample file](sample/content.xml)\
[Tag Reference](reference.md)
