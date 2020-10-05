# Markdown

## 概要

Markdownはドキュメントを作成する際に便利な記法(マークアップ言語)のこと．エンジニア同士がやりとりするドキュメントは基本的にMarkdownで記述されることが多く，GitHub, Trelloなどエンジニア向けのWebサービスでも広くMarkdown記法が利用されている．Markdownには見出し・箇条書きなどのHTMLのタグと対応する記法があり，簡単にHTML互換のドキュメントを作成できる．しかしMarkdownはあくまでマークアップ言語であるため，どのように表示されるかはMarkdownビューアが設定してるCSSに依存する．

VS CodeやWebサービスなどを利用することで，Markdownのプレビューを見ながら記述できて便利．[Dillinger](https://dillinger.io/)などのサービスが有名．


## 参考
- [【超入門】Markdown記法の使い方 （サンプル付き） - RAKUS Developers Blog | ラクス エンジニアブログ](https://tech-blog.rakus.co.jp/entry/20200624/markdown)
- [Markdown記法 サンプル集 - Qiita](https://qiita.com/tbpgr/items/989c6badefff69377da7)


## 記法

以下よく利用する記法を紹介する．


### 見出し

#の数に応じて見出し(HTMLのh1タグなどに相当)を作成することができる．最大見出し6まで作成可能で#を7個以上続けても#がそのまま表示される．

Markdown
```
# 見出し1
## 見出し2
### 見出し3
#### 見出し4
##### 見出し5
###### 見出し6
```

表示
# 見出し1
## 見出し2
### 見出し3
#### 見出し4
##### 見出し5
###### 見出し6

### 箇条書き

HTMLのliタグに対応する箇条書きを行う．Markdownでは```-```, ```+```, ```*```のいずれかで箇条書きが利用できるが基本的には```-```しか利用しない．


Markdown
```
- リスト1
  - リスト1-1
  - リスト1-2
- リスト2
```

表示
- リスト1
  - リスト1-1
  - リスト1-2
- リスト2


### リンク

`[表示テキスト](リンクのURL)`の形式でリンクを表示することができる．

Markdown
```
[この](https://github.com/kobe-pablo/wiki)リポジトリでドキュメントを管理している
```

表示

[このリポジトリ](https://github.com/kobe-pablo/wiki)でドキュメントを管理している


### 強調

アスタリスクで指定部分を囲むことで強調することができる．アスタリスクは1つから3つまで利用でき，1つの場合は斜体に，2つの場合は太字に，3つの場合は斜体かつ太字になる．

Markdown
```
You say *goodbye* and I say hello.  
You say **goodbye** and I say hello.  
You say ***goodbye*** and I say hello.  
```

表示

You say *goodbye* and I say hello.  
You say **goodbye** and I say hello.  
You say ***goodbye*** and I say hello.  


### コードスニペット

コードのスニペットをバッククォートで囲むことで表示できる．

Markdown
```
`wget http://example.com`
```

表示

`wget http://example.com`


### テーブル

以下のように書くことで表形式の表示ができる．

Markdown
```
| 項目 | 詳細 |
|--|--|
| Hey! | Yo! |
| Hey! | Yo! |
```

表示

| 項目 | 詳細 |
|--|--|
| Hey! | Yo! |
| Hey! | Yo! |


### 取り消し線

2つのチルダで該当箇所を囲むことで取り消し線を引くことができる．

Markdown
```
You say ~~goodbye~~ and I say hello.
```

表示

You say ~~goodbye~~ and I say hello.
