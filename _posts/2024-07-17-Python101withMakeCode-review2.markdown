---
layout: post
title: 【ワールドレビュー】Python 101 - MakeCode 3 & 4
description: 教育版マインクラフトのPython 101 - Makecodeの概要とプレイ感想、第2回目です。

date:   2024-07-17 15:00:00 +0300
image:  '/images/b-10-00.jpg'
video_embed:
tags:   [教育版マインクラフト, プログラミング, Python]
---

教育版マインクラフトでのPython学習、Python 101 - Makecodeの続きです。

このコースでは、プログラミング環境MakeCodeを使ってPythonによるコーディングを学べます。

レッスン (ワールド) は全部で10回に分かれています。

今回はレッスン3と4の概要とプレイ感想をまとめました。


<div style="padding: 10px; margin-bottom: 10px; border: 1px solid #181818; background-color: var(--background-alt-color); border-radius: 5px;" markdown="1">
<h4>目次</h4>
* table
{:toc}
</div>

***

## Python 101 - MakeCode レッスン3 / レッスン4の詳しい学習内容

レッスン3 / レッスン4について、それぞれの学習目的と問題内容を詳しくみてみます。

<br>

### Python 101 - MakeCode レッスン3

レッスン3の学習目的は以下のとおり。

<div style="padding: 10px; margin-bottom: 10px; border: 5px double #333333; border-radius: 10px;">
<p><b> Python 101 - MakeCode レッスン3の学習目的</b></p>
<p><strong>○ 変数について学び、活用する</strong></p>
<p><strong>○ 位置情報を変数に入れて使ってみる</strong></p>
<p><strong>○ コードの作成 / テスト / デバッグを行う</strong></p>
</div>

<br>

ワールドに入り、立っている人に話しかけながら進めます。

**英語テキストは、イマーシブリーダー機能を使うと音読や翻訳をしてくれます。**

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-09-01.jpg" loading="lazy">
    <img src="/images/b-09-02.jpg" loading="lazy">
 <img src="/images/b-09-03.jpg" loading="lazy">
 </div>
 <em>イマーシブリーダーを使えば、文章を音読させたり、日本語訳にすることができます。</em>
</div>
<br>


**Python 101 - MakeCodeレッスン3のプログラミング課題は全3問。**

**変数に数値や文字列を代入して、チャット表示や計算をしていきます。**

<br>

**問題1**

変数に果物の名前を代入し、**player.say()**コマンドでチャット表示します。

壁に書かれたアルファベット順にチャット表示させ、表示された順に壁の果物のボタンを押しましょう。


<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-10-02.jpg" loading="lazy">
    <img src="/images/b-10-03.jpg" loading="lazy">
    <img src="/images/b-10-04.jpg" loading="lazy">
 </div>
 <em>部屋の壁には問題の要点が書いてあります。コードビルダーの上部とコード内には詳しい指示とヒントが書いてあります。</em>
</div>
<br>



**問題2**

変数に位置情報を入れ、コードを完成させます。

画面左隅に表示される座標情報を見て、自分の立ち位置に対応する変数名を確認します。

**blocks.place()**の位置情報部分に正しい変数を入れ、天井にあるブロックと同じブロックを地面にも置ければ成功です。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-10-05.jpg" loading="lazy">
    <img src="/images/b-10-06.jpg" loading="lazy">
 </div>
 <em>コードビルダーのツールボックスからコードのヒントを得られます。この課題ではblocks.place()のposに変数を入れてコードを完成させます。</em>
</div>
<br>



**問題3**

変数に数値を代入して計算し、**player.say()**で答えを出力させます。

出力された答えを見て、正しい値のボタンを押します。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-10-07.jpg" loading="lazy">
    <img src="/images/b-10-08.jpg" loading="lazy">
<img src="/images/b-10-09.jpg" loading="lazy">
 </div>
 <em>変数を使って計算し、計算結果を出力します。細かい指示はコードビルダーの説明を読む必要があります。設定ボタンから日本語訳もできます。</em>
</div>
<br>

<br>

### Python 101 - Makecode レッスン4

レッスン4の学習目的は以下のとおり。

<div style="padding: 10px; margin-bottom: 10px; border: 5px double #333333; border-radius: 10px;">
<p><b> Python 101 - Makecode レッスン4の学習目的</b></p>
<p><strong>○ リストについて学び、活用する</strong></p>
<p><strong>○ リストの名前はスペースの代わりに "_" を利用する</strong></p>
<p><strong>○ リストのメソッドを使ってみる</strong></p>
</div>

<br>

**レッスン4のプログラミング課題は全3問。**

**リストを使いこなしていきます。**

<br>

**問題1**

まずはリストに値を代入してみます。

**list_name=[]**の構文で書かれた箇所に、部屋に置かれている動物と同じ順番で名前を書いていきます。

コードビルダー上の予測入力が動物名の入力をサポートしてくれます。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-10-11.jpg" loading="lazy">
    <img src="/images/b-10-12.jpg" loading="lazy">
 <img src="/images/b-10-14.jpg" loading="lazy"> 
 </div>
 <em>コードビルダーを開き、list_name=[]の構文で書かれた箇所に動物の名前を順に記入します。</em>
</div>
<br>



**問題2**

**append**と**pop**を使い、リスト内の値の追加や削除をします。

コードビルダーのコード内にヒントが書かれているので参考にしましょう。

実行後は、出てきたご飯を犬の前まで持っていって**q**で離します。

この際、犬に直接あげてしまうと、正しく検知されないので気をつけてください。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-10-15.jpg" loading="lazy">
    <img src="/images/b-10-16.jpg" loading="lazy">
 <img src="/images/b-10-17.jpg" loading="lazy"> 
 </div>
 <em>appendやpopでリストの内容を変更して、各犬に必要な食材を手に入れます。</em>
</div>
<br>


**問題3**

最後はリスト内の値を書き換えたり、**sort**と**reverse**を使い、値の並び替えをします。

コマンド実行後、チャットに出力された名前と同じ名前の猫を探し、ボタンを押します。

猫の名前は近づいたら頭上に現れます。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-10-18.jpg" loading="lazy">
    <img src="/images/b-10-21.jpg" loading="lazy">    
 <img src="/images/b-10-19.jpg" loading="lazy"> 
 </div>
 <em>リスト内の値の変更や並び替えを行います。コードビルダーの電球マークにもヒントがあります。</em>
</div>
<br>


***

## プレイ感想 ー 難易度UP！座学後の実践編に良さそう

Python 101 - Makecodeのレッスン3、レッスン4では変数やリストについて学び、グッとプログラムらしくなってきました。

コードの文字数も多くなってくるので、レッスン2までと比べると難易度が上がった感じがします。

**ゲーム内の手引きやヒントのおかげで、ざっくりとした知識さえあればサクサクと書いていけます。**

ただ、構文やメソッドの詳しい説明はゲーム内ではさほどありません。

**0から勉強する場合には、座学で学んだ上で、実践編として挑戦するのが良いと感じました。**

***

## 注意点など

**日本語対応：デフォルトは英語。イマーシブリーダーを使えば翻訳してくれます。**


***
## まとめ

Python 101 - Makecodeのレッスン3とレッスン4についてまとめました。

**この回ではPythonの変数とリストについて学びます。**

**変数とリストの概念や機能に関する説明はゲーム内では薄いので、座学で学んだ上での実践編として挑戦するのがおすすめです！**

ヒントや手引きがしっかりしているので、大雑把な知識でも、教科書やWebに戻ることなく進めていける点が高評価でした。

まだ6回分ありますので、引き続き遊んでレビューしていきたいと思います。

***

## サポート資料

以下のサイトで指導者用のガイド資料、授業スライド、追加アクティビティへのリンクなどが見つかります。

**[<span style="color:#1589FF">Python 101 with MakeCode - Lesson 3
</span>](https://education.minecraft.net/ja-jp/lessons/python-101-lesson-3)**

**[<span style="color:#1589FF">Python 101 with MakeCode - Lesson  4
</span>](https://education.minecraft.net/ja-jp/lessons/python-101-lesson-4)**


