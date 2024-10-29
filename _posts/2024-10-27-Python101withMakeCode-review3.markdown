---
layout: post
title: 【ワールドレビュー】Python 101 - MakeCode 5 & 6
description: 教育版マインクラフトのPython 101 - Makecodeの概要とプレイ感想、第3回目です。

date:   2024-10-27 15:00:00 +0300
image:  '/images/b-12-00.jpg'
video_embed:
tags:   [教育版マインクラフト, プログラミング, Python]
---

教育版マインクラフトでのPython学習、Python 101 - Makecodeの続きです。

このコースでは、プログラミング環境MakeCodeを使ってPythonによるコーディングを学べます。

レッスン (ワールド) は全部で10回に分かれています。

今回はレッスン5と6の概要とプレイ感想をまとめました。


<div style="padding: 10px; margin-bottom: 10px; border: 1px solid #181818; background-color: var(--background-alt-color); border-radius: 5px;" markdown="1">
<h4>目次</h4>
* table
{:toc}
</div>

***

## Python 101 - MakeCode レッスン5 / レッスン6の概要

Python 101 - MakeCodeではいよいよエージェントが登場します。

エージェントは、コーディングで作業をしてくれるマインクラフト内ロボットのようなキャラクターです。


<div style="padding: 10px; margin-bottom: 10px; border: 5px double #333333; border-radius: 10px;">
<p><b>要点まとめ</b></p>
<p><strong>○ 世界観：CodingMineというソフトウェア会社から、ロボット開発への協力を頼まれます。</strong></p>
<p><strong>○ 提供元：Minecraft Education</strong></p>
<p><strong>○ 学習目的：レッスン5と6ではループと条件分岐を使っていきます。</strong></p>
</div>

<br>

ワールドに入るとCodingMineというソフトウェア会社のCEOが登場。

ロボット (エージェント) の開発を手助けしてくれるよう頼まれます。

1レッスンあたりで出題される問題は大問3題。

レッスン5では、for文を使ったループへの理解を深めます。

レッスン6では、if / if else / elsif文を使った条件分岐を練習します。

***

## Python 101 - MakeCode レッスン5 / レッスン6の詳しい学習内容

レッスン5 / レッスン6について、それぞれの学習目的と問題内容を詳しくみてみます。

<br>

### Python 101 - MakeCode レッスン5

レッスン5の学習目的は以下のとおり。

<div style="padding: 10px; margin-bottom: 10px; border: 5px double #333333; border-radius: 10px;">
<p><b> Python 101 - MakeCode レッスン5の学習目的</b></p>
<p><strong>○ コーディングにおけるループの概念を学び、活用する</strong></p>
<p><strong>○ エージェント用のコードを書いてみる</strong></p>
</div>


ワールドに入り、早速CEOに話しかけてみます。

英語テキストは、イマーシブリーダー機能を使うと音読や翻訳をしてくれます。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-12-01.jpg" loading="lazy">
    <img src="/images/b-12-02.jpg" loading="lazy">
    <img src="/images/b-12-21.jpg" loading="lazy">
 </div>
 <em>イマーシブリーダーを使えば、文章を音読させたり、日本語訳にすることができます。今回はエージェントが登場！</em>
</div>
<br>


Python 101 - MakeCodeレッスン５のプログラミング課題は大問3問。

エージェントを動かすための**agent.xxx**という形式のコマンドを利用して書いていきます。

<br>

**問題1**

エージェントに重い荷物を持って運んでもらいます。

**agent.collect_all()**、**agent.move()**、**agent.place()**を使ってプログラムを書いていきます。

パート1では1回のみの動作、パート2では同じ動作を4回するようにfor文を使ってループ構造にします。


<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-12-03.jpg" loading="lazy">
    <img src="/images/b-12-04.jpg" loading="lazy">
 <img src="/images/b-12-09.jpg" loading="lazy">
 </div>
 <em>ブロックを拾う / 移動する / ブロックを置くをコーディングします。左側のツールボックスからコマンドのヒントを得られます。</em>
</div>
<br>



**問題2**

エージェントに洗濯をしてもらいます。

**agent.turn()**を使い、洗濯機の中でエージェントが自ら (!?) 回転して洗濯します笑

パート2ではfor文の多重ループ（for文の中にfor文）をやってみます。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-12-05.jpg" loading="lazy">
    <img src="/images/b-12-07.jpg" loading="lazy">
<img src="/images/b-12-06.jpg" loading="lazy">
 </div>
 <em>向きを変えるコマンドでエージェントを回転させます。エディタ部分のヒントが参考になります。</em>
</div>
<br>



**問題3**

エージェントにカーペットを掃除してもらいます。

**agent.move()**でエージェントをうまく動かしながら**agent.collect_all()**でゴミを回収していきます。

for文を複数使い、多重ループやカウンタ変数、タブを正しく使えるように練習していきます。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-12-08.jpg" loading="lazy">
  </div>
 <em>エージェントにカーペット上を移動させ、浮かぶゴミを回収します。</em>
</div>
<br>



### Python 101 - Makecode レッスン6

レッスン6の学習目的は以下のとおり。

<div style="padding: 10px; margin-bottom: 10px; border: 5px double #333333; border-radius: 10px;">
<p><b> Python 101 - Makecode レッスン2の学習目的</b></p>
<p><strong>○ コーディングにおける条件分岐の概念を学び、活用する</strong></p>
<p><strong>○  if、if else、elsifを活用する</strong></p>
</div>


レッスン6のプログラミング課題は大問3問。

条件分岐を使いながらエージェントに車の運転を教えます。

<br>

**問題1**

信号に従った停車と発進を教えます。

**agent.detect()**を使い、エージェントの左側にブロックがある場合に発進、停車、一時停車をするようにコーディングしていきます。

**agent.detect()**は、指定方向に隣接したブロックがあるかを調べて、TrueかFalseを返します。

パート1ではブロックがある場合に前進。パート2ではブロックがある場合に停止。パート3ではブロックがある場合に2秒停止するようにします。


<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-12-10.jpg" loading="lazy">
    <img src="/images/b-12-14.jpg" loading="lazy">
  <img src="/images/b-12-13.jpg" loading="lazy">
  </div>
 <em>agent.detect()で、左側のブロックを認識させて発進、停車、一時停車をコーディングします。</em>
</div>
<br>



**問題2**

道路標識に従ってエージェントが左折 / 右折をできるようにします。

**agent.inspect()**を使い、正面にあるブロックの種類によってエージェントを左か右に方向転換させます。

**agent.inspect()**は、指定方向に隣接したブロックを調べて、ブロックIDやデータを返します。

パート1では左折、パート2では左折と右折を使い分けて前に進めるようにします。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-12-15.jpg" loading="lazy">
    <img src="/images/b-12-16.jpg" loading="lazy">
    <img src="/images/b-12-17.jpg" loading="lazy">
  </div>
 <em>エージェントが突き当たった先のテラコッタの色によって左折か右折をするようにコーディングします。</em>
</div>
<br>


**問題3**

最後は、if分の条件の部分に論理演算子 (and / and not / or) を使って複数条件式を作ります。

エージェントの前方と左右にブロックがあるかを判断し、状況に応じて前 / 左 / 右に動くようにコーディングします。

エージェントが目の前の障害物ブロックを避けながらゴールまで辿り着くことができれば成功です！


<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-12-18.jpg" loading="lazy">
    <img src="/images/b-12-19.jpg" loading="lazy">
    <img src="/images/b-12-20.jpg" loading="lazy">
  </div>
 <em>条件分岐のifのところでand notやandを利用して複数条件式を作ります。</em>
</div>
<br>

***

## プレイ感想 ー エージェントが意図した通りに動くと嬉しい！

Python 101 - Makecodeのレッスン5 / レッスン6では、ついにエージェントが登場しました。

ループや条件分岐を使いこなしてエージェントを動かすのですが、

各コマンドの実行結果が目に見えて確認できるので楽しいです。

パズルを解く楽しさと、正解した時の快感があります。

[<span style="color:#1589FF">前回の変数や配列のレッスン</span>](https://www.maisusu.com/blog/python101withmakecode-review2)では飽きがちだった息子も、ここまでいけば逆に楽しくやっていました。

これまで同様、コードビルダー内には使用するコマンドやヒントが記載されているので、前提知識があればそれらヒントを頼りに書いていけます。

座学で軽く学んだ上で、実践編として挑戦すると楽いでしょう。

***

## 注意点など

日本語対応：デフォルトは英語。イマーシブリーダーを使えば翻訳してくれます。


***
## まとめ

Python 101 - Makecodeのレッスン5とレッスン6についてまとめました。

この回ではエージェントを動かしながらfor文やif分を使ったコードを書いていきます。

ループと条件分岐を使いこなせば、エージェントを使ってできることもグッと広がります。

単純作業をエージェントに任せ、整地や建築を楽々高速でこなせるようになるのも目前！

全10回のレッスンも後半に入りました、引き続き遊んでレビューしていきます。

***


## サポート資料

**[<span style="color:#1589FF">Python 101 with MakeCode - Lesson 5
</span>](https://education.minecraft.net/ja-jp/lessons/python-101-lesson-5)**
指導者用のガイド資料、授業スライド、追加アクティビティへのリンクなどが見つかります。

**[<span style="color:#1589FF">Python 101 with MakeCode - Lesson  6
</span>](https://education.minecraft.net/ja-jp/lessons/python-101-lesson-6)**
指導者用のガイド資料、授業スライド、追加アクティビティへのリンクなどが見つかります。


