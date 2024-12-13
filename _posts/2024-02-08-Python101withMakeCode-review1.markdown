---
layout: post
title: 【ワールドレビュー】Python 101 - MakeCode 1 & 2
description: 教育版マインクラフトのPython 101 - Makecodeの概要とプレイ感想、第1回目です。

date:   2024-02-07 15:00:00 +0300
image:  '/images/b-09-00.jpg'
video_embed:
tags:   [minecraftedu, programming, python]
---

教育版マインクラフトでPython 101 - MakeCodeを始めてみました。

このコースでは、プログラミング環境MakeCodeを使ってPythonを使ったコーディングを学べます。

レッスン (ワールド) は全部で10個。

この記事ではレッスン1と2の概要とプレイ感想をまとめました。


<div style="padding: 10px; margin-bottom: 10px; border: 1px solid #181818; background-color: var(--background-alt-color); border-radius: 5px;" markdown="1">
<h4>目次</h4>
* table
{:toc}
</div>

***

## Python 101 - MakeCode レッスン1 / レッスン2の概要

Python 101 - MakeCodeではMakeCodeを使い、Pythonの書き方を学んでいきます。

<div style="padding: 10px; margin-bottom: 10px; border: 5px double #333333; border-radius: 10px;">
<p><b>要点まとめ</b></p>
<p><strong>○ 世界観：CodingMineというソフトウェア会社が舞台。社員と話しながらプログラミングの課題をこなします。</strong></p>
<p><strong>○ 提供元：Minecraft Education</strong></p>
<p><strong>○ 学習目的：レッスン1と2ではMakeCodeの使い方、Pythonの基本の構文、ブロック設置を学びます。</strong></p>
</div>

<br>

ワールドに入るとCodingMineというソフトウェア会社のCEOが登場。

プログラミングの問題を解き、社員の抱える問題を解決するよう頼まれます。

1レッスンあたりで出題される問題は3-4個。

レッスン1では、Pythonの構文 (シンタックス) への理解を深めます。

レッスン2では、ブロックを置くコマンドと相対座標を練習します。

***

## Python 101 - MakeCode レッスン1 / レッスン2の詳しい学習内容

レッスン1 / レッスン2について、それぞれの学習目的と問題内容を詳しくみてみます。

<br>

### Python 101 - MakeCode レッスン1

レッスン1の学習目的は以下のとおり。

<div style="padding: 10px; margin-bottom: 10px; border: 5px double #333333; border-radius: 10px;">
<p><b> Python 101 - MakeCode レッスン1の学習目的</b></p>
<p><strong>○ MakeCodeを使ってみる</strong></p>
<p><strong>○ Minecraft Pythonの構文 (シンタックス) を意識する</strong></p>
<p><strong>○ 文字列と数値の違いを知る</strong></p>
</div>


ワールドに入り、早速CEOに話しかけてみます。

英語テキストが表示されて早々に壁を感じますが、イマーシブリーダー機能を使うと音読や翻訳をしてくれます。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-09-01.jpg" loading="lazy">
    <img src="/images/b-09-02.jpg" loading="lazy">
    <img src="/images/b-09-03.jpg" loading="lazy">
 </div>
 <em>イマーシブリーダーを使えば、文章を音読させたり、日本語訳にすることができます。</em>
</div>
<br>


Python 101 - MakeCodeレッスン1のプログラミング課題は全3問。

コメント表示ができる**player.say()**コマンドを使いながら、エラー箇所を見つけたり、計算結果を表示させていきます。

<br>

**問題1**

**player.say()**が正しく書かれたコンピュータを探します。

コンピュータに書かれているコマンドをMakeCodeに写して実行しながら、正解を見つけましょう。


<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-09-10.jpg" loading="lazy">
    <img src="/images/b-09-04.jpg" loading="lazy">
 </div>
 <em>部屋の壁には問題の要点が書いてあります。机の上のディスプレイにはそれぞれ文字列が表示されていました。</em>
</div>
<br>



**問題2**

画面に表示された**player.say()**のエラー箇所を見つけて、該当するブロックを置いてあげます。

プログラミングをしていく上で欠かせないエラー箇所探しです。

数値の場合は「””」で囲わないということが、最後にさらっと登場します。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-09-11.jpg" loading="lazy">
    <img src="/images/b-09-05.jpg" loading="lazy">
 </div>
 <em>足りない文字のブロックを置いていきます。</em>
</div>
<br>



**問題3**

**player.say()**の中で計算式を書き、答えを出力させます。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-09-12.jpg" loading="lazy">
    <img src="/images/b-09-06.jpg" loading="lazy">
  </div>
 <em>player.say()コマンドを使って計算結果を出力します。</em>
</div>
<br>



### Python 101 - Makecode レッスン2

レッスン2の学習目的は以下のとおり。

<div style="padding: 10px; margin-bottom: 10px; border: 5px double #333333; border-radius: 10px;">
<p><b> Python 101 - Makecode レッスン2の学習目的</b></p>
<p><strong>○ 相対座標について学ぶ</strong></p>
<p><strong>○ コマンドでブロックを置いてみる</strong></p>
<p><strong>○ コード補完ツールを使ってみる</strong></p>
</div>


レッスン2のプログラミング課題は全4問。

ブロックを置く**blocks.place(ブロック名, 位置)**コマンドを使い、相対座標を変えながらブロックを置いていきます。

<br>

**問題1**

まずは自分の立っている場所にブロックを一つ置いてみます。

このレッスンでは全て相対座標を使いますので、自分の場所**(0, 0, 0)**からスタートです。

MakeCode上のツールボックスや、予測入力がコマンドや変数の入力をサポートしてくれます。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-09-13.jpg" loading="lazy">
    <img src="/images/b-09-07.jpg" loading="lazy">
  </div>
 <em>ブロックを置くコマンドを使います。MakeCode上のツールボックスから必要なコマンドのベースをドラッグ＆ドロップで入力することもできます。</em>
</div>
<br>



**問題2**

次の問題では座標のうち、高さが変わるy座標（2番目の数値）を変更していきます。

壁に表示された数字を見ながら、正しい数値を入力して、天井の照明部分３箇所にレッドストーンランプを設置します。

うまく設置できたら、壁にあるレバーで点灯させます。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-09-14.jpg" loading="lazy">
    <img src="/images/b-09-15.jpg" loading="lazy">
  </div>
 <em>blocks.place()コマンドの座標のy座標の数値を変えながらブロックを正しい位置に配置します。</em>
</div>
<br>


**問題3**

次は高い壁を乗り越えるための階段を作ります。座標のうち、y座標とz座標（2番目と3番目の数値）を変えながらブロックが段差になるように置いていきます。

足元に金のブロックがある場所が目印。ここから動くと相対座標の指定の仕方も変わってくるので、移動しないように注意しながら位置座標を変えていきます。


<br>

**問題4**

最後は穴を渡る橋を作ります。座標のうち、x座標とy座標（1番目と2番目の数値）を変えながらブロックを置いていきます。

慣れてきたら、複数個まとめて置いてみても良いかもしれません。

ちなみに落ちてしまっても、抜け穴で上に戻れるので安心です。



<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-09-16.jpg" loading="lazy">
    <img src="/images/b-09-17.jpg" loading="lazy">    
  </div>
 <em>問題3と問題4。blocks.place()コマンドの座標を変えながらブロックを正しい位置に配置します。</em>
</div>
<br>

***

## プレイ感想 ー プログラミングをやってみるキッカケに！

6歳の息子と「少しプログラミングをやってみようか」ということで始めてみました。

マイクラ好き、ゲーム好きなので、誘えばるんるんで付き合ってくれます。

**やってみて、いいなと思ったのは以下のポイントです。**

* __1時間以内で終わり、ダラダラしない__
* __プログラミング課題もちょうど良い難易度__
* __英語の勉強にもなる__
* __イマーシブリーダーを使えば読む負担軽減__


こどもの集中力 / 私の都合の両面で、1時間以内で終わるというのはちょうど良い長さでした。

学校やアフタースクールの1コマでやるのにも使いやすそうです。

プログラミング課題については、求められている内容は一緒に確認。

確認後は、6歳児でもあれこれ自分で考えて取り組めていました。

すごく良かったのはイマーシブリーダーです。

息子はまだ読むより聞く方が得意なので、イマーシブリーダーで読み上げてくれるのは助かりました。

リスニングの勉強にもなりそうです。

まだ始めたばかりですが、プログラミングに慣れ親しむ上では良いスタートを切れた感じです。

今後のレッスンでどういったことが取り上げられるのか、次回が楽しみです。

***

## 注意点など

**日本語対応：デフォルトは英語。イマーシブリーダーを使えば翻訳してくれます。**


***
## まとめ

Python 101 - Makecodeのレッスン1とレッスン2についてまとめました。

ここまでで、MakeCodeやコーディングサポート機能の操作方法、Pythonの構造やブロックの設置について学びます。

息子にとっては、ほぼ初めてのPythonですが、使って慣れてみるという上では良い題材でした。

まだまだレッスン10までありますので、引き続き遊んでレビューしていきたいと思います。

***

## サポート資料

以下のサイトで指導者用のガイド資料、授業スライド、追加アクティビティへのリンクなどが見つかります。

**[<span style="color:#1589FF">Python 101 with MakeCode - Lesson 1
</span>](https://education.minecraft.net/ja-jp/lessons/python-101-lesson-1)**

**[<span style="color:#1589FF">Python 101 with MakeCode - Lesson  2
</span>](https://education.minecraft.net/ja-jp/lessons/python-101-lesson-2)**
