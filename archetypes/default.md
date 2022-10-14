---
# ルール
# hugo new Categories/TITLE.md ※ Categoriesは半角英数字（日本語ではパンくずリストが機能しない
# 基本下書きせずに出力


title: "{{ replace .Name "-" " " | title }}"
description : "説明文"
date: {{ .Date }}
draft: false # 反映させる時はfalseに変えるかコメントアウト
comments: true
adsense: false
archives: ["{{ dateFormat "2006" .Date }}", "{{ dateFormat "2006-01" .Date }}"]

# Twitter card gen用設定"]
author: ["@_numbP"]
categories: ["映画備忘録"]
tags: ["邦画洋画", "Netflix", "AmazonPrime", "299円", "星1"] # tag
ogimage: "images/og/{{ .Name }}.png" # tcardgenで生成した画像をOGP画像に設定する
url: "/{{ .Type }}/{{ .Name }}/" # tcardgenでの自動生成スクリプト用のパスを設定

# Blog用---------------------------------------------------
type: post
image: "images/og/{{ .Name }}.png" # ブログバナーの画像

# Portfolio用----------------------------------------------
caption: Product Mockup
image: images/portfolio/item-2.jpg
liveLink: link # ??
# 右側の情報説明
client: Julia Robertson
submitDate: November 20, 2017
category: ["mockup","design"] # tag
location: 1201 park street, Avenue, Dhaka

---