---
# ルール
# hugo new Categories/TITLE.md ※ Categoriesは半角英数字（日本語ではパンくずリストが機能しない
# 基本下書きせずに出力
# 一人称「ぼく」
# 敬語なし、自分の頭での口頭文、自己言及で言い聞かせ風
# 中学生にも分かる語彙を選ぶ

title: "{{ replace .Name "-" " " | title }}"
description : "あらすじ"
descriptText : "XXXXXX"
date: {{ .Date }}
draft: false # 反映させる時はfalseに変えるかコメントアウト
comments: true
adsense: false
archives: ["/{{ dateFormat "2006" .Date }}/", "/{{ dateFormat "2006-01" .Date }}/"]

# Twitter card gen用設定
author: ["なぴた"]
categories: ["映画備忘録"]
tags: ["邦画洋画", "Netflix", "AmazonPrime", "無料", "星1"] # tag
# ogimage: "images/og/{{ .Name }}.png" # tcardgenで生成した画像をOGP画像に設定する
ogimage: "images/favicon.jpg" # tcardgenで生成した画像をOGP画像に設定する
url: "/{{ .Type }}/{{ .Name }}/" # tcardgenでの自動生成スクリプト用のパスを設定

# Blog用---------------------------------------------------
type: blog
image: "images/blog/{{ .Name }}.png" # ブログバナーの画像

# Portfolio用----------------------------------------------
caption: "Movie profile"
image: "images/og/{{ .Name }}.png"
liveLink: link # ??

# 右側の情報説明
client: numbP
submitDate: {{ .Date }}
category: ["movie", "netflix", "amazon prime"] # tag
location: Tokyo, Japan

---

## 選んだ理由



-------------------------
-------------------------
-------------------------
-------------------------
-------------------------
-------------------------
## 以後ネタバレやでぇ
-------------------------
-------------------------
-------------------------
-------------------------
-------------------------
-------------------------

## 感想



## 感想の背景



## その背景で心動いた理由



## 心動いて至った考え



## 見た前と見た後の印象や自分の変化



## 総括し、実行へ至る考え


## 端書（鑑賞中のメモ）
- プロット→
- 