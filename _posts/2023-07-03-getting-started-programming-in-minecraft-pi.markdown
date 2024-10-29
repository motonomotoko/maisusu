---
layout: post
title: ラズパイ用マインクラフトで子どもとプログラミング
description: ラズパイで使えるマインクラフト Pi Rebornを使い、プログラミングをしてみました。
date:   2023-07-03 15:00:00 +0300
image:  '/images/b-04-00.jpg'
video_embed:
tags:   [初心者向け, プログラミング, RaspberryPi]
---

プログラミングや電子工作の学習用にも人気の小型コンピュータ、ラズベリーパイ。

ラズベリーパイを使えば、マインクラフトPi Editionを無料で遊ぶことができます。

しかもPi Editionは、プログラミング開発環境と連携させることができるので、簡単にプログラミングを始めることができます。

我が家でもプログラミングを通してマイクラの世界を遊んでみたので、その内容をまとめました。

<div style="padding: 10px; margin-bottom: 10px; border: 1px solid #181818; background-color: var(--background-alt-color); border-radius: 5px;" markdown="1">
<h4>目次</h4>
* table
{:toc}
</div>

***

## ラズベリーパイとは

ラズベリーパイとは、手のひらサイズほどの小型コンピュータです。

もともとはコンピューターサイエンスの教育用教材としてイギリスで開発され、日本でもオンラインショップや電子部品屋さんで購入することができます。

ラズベリーパイという名前はフルーツのラズベリー、プログラミング言語のPython（パイソン）とお菓子のパイをかけていて、日本ではラズパイという愛称で親しまれています。

小さいものの、モニターやキーボードをつければネット検索やゲームをして楽しむこともできますし、ロボットの制御や、家庭内のIoT環境の構築などにも利用できます。

価格も定価が10,000円以下と、コンピュータとしては低予算で購入できるため、子供のプログラミング学習や電子工作用としても人気があります。（ただし現在は半導体不足の影響で、定価で入手しづらい状況が続いているようです。）

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-04-01.jpg" loading="lazy">
  </div> 
 <em>手の平サイズのラズベリーパイ。マウスと比べても同じくらいの大きさです。</em>
</div>

***

## マインクラフトPi Editionとは

マインクラフトPi Editionは、ラズパイ上で動作する特別なバージョンのマインクラフトです。

公式サポートはすでに終了しているため、ブロックやMobなどの種類は少ないですが、通常のマイクラと同じように採掘や建築を楽しむことができます。

さらに、Pi Editionではプログラミング言語のPythonを使ってゲームの操作をすることができます。

このおかげで、子ども達に大人気のマイクラで、気軽にプログラミング学習を始められるのです。

なお、マインクラフトPi Editionはラズベリーパイを持っていれば無料でインストール可能です！

***

## ラズベリーパイのプログラミング環境

もともと教材として開発されたラズパイには、プログラミングを手軽に始められるアプリが標準で搭載されています。

ラズパイを立ち上げて、モニターに画像を写し、メニューからプログラミングを開くと、そこにはずらっとプログラミング用のアプリが並びます。

中には子ども達に大人気のScrachもあります。

今回の記事では、この中からThonnyを使ってプログラミングしていきたいと思います。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-04-02.jpg" loading="lazy">
  </div>
 <em>メニューからプログラミングを開くと、ずらっとアプリが並びます。</em>
</div>

***

## マインクラフトの世界をプログラミングで遊ぶ

今回のプログラミングではラズパイに標準搭載されているThonnyを使っていきます。

Thonnyは初心者向けのPythonの開発環境で、ソースコードごとにファイルを作成・保存してくれるのが特徴です。

このため、別々のコードがつながって分かりづらくなることを防いでくれ、コード完成後も保存ファイルとして整理しやすくなります。

<br>

### 事前準備

**1.マインクラフトPi Editionのインストール**

マインクラフトPi Editionはインストールが必要です。

もしまだインストールしていない場合は、[<span style="color:#1589FF">こちらのページ</span>](https://www.maisusu.com/blog/install-minecraft-on-raspberry-pi)をご覧ください。

Pi-Appsを使った簡単なインストール方法を紹介しています。

<br>

**2.マイクラ用のPythonライブラリのインストール**

マイクラをPythonから操作するため、マイクラ用のPythonライブラリであるmcpiをインストールしておく必要があります。

インストールするためには、ターミナルを開いて以下のコマンドを実行します。

この手順は初回一回のみで大丈夫です。

{% highlight css %}
pip install mcpi
{% endhighlight %}

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-04-pip.jpg" loading="lazy">
  </div>
 <em>マイクラ用のPythonライブラリ、mcpiをインストールします。</em>
</div>

<br>

### マイクラとThonnyを連携させる

マイクラとThonnyは、それぞれのアプリを**マイクラのワールド -> Thonnyの順に立ち上げるだけ**で簡単に連携できます。

まず、マイクラのワールドを開きます。**ワールドはクリエイティブモード**を選んでください。

ワールドが開いたらキーボードで**Tab**を押して、マウスをマイクラの画面内から出し、**プログラミングメニューからThonny Python IDE**を開きます。

これでマイクラとThonnyが連携しました。

※マイクラ側で別ワールドを立ち上げてしまうなど、何らかの操作の拍子にマイクラとThonnyの連携が切れてしまうことがあります。
その場合は一度マイクラのワールドを閉じ、再度マイクラのワールド->Thonnyの順に立ち上げると復活します。

<br>

### マイクラの画面にHello World!を出してみる。

新しい言語を学ぶときの定番で、まずはチャット欄に "Hello World!"を出すプログラムを書いてみます。

Thonnyの画面を見ると、上下に二つのスペースがあります。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-04-04.jpg" loading="lazy">
  </div>
 <em>Thonnyの画面、上下に二つのスペースがあります。</em>
</div>

上のスペースはコードを書くスペース。下のスペースはコードを実行した時の結果やデバッグ情報が表示されます。

上側のスペースに**以下のコードを入力またはコピペ**します。

{% highlight js %}
from mcpi.minecraft import Minecraft 
mc = Minecraft.create() 

mc.postToChat("Hello world!")
{% endhighlight %}

入力が完了したら、ファイルを保存します。

Thonnyの画面上にある**Save**をクリックして保存します。ファイル名は拡張子を入れず、名前だけを入力すればOKです。

保存できたらThonnyのSaveの隣りにある**Run**をクリックします。

マイクラのチャットにHello World!の文字が出ました。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-04-05.jpg" loading="lazy">
    <img src="/images/b-04-06.jpg" loading="lazy"> 
  </div>
 <em>Thonnyでプログラミング。マイクラのチャット欄にHello World!と表示されました。</em>
</div>

<br>

### 自分のいる位置の座標を取得してからテレポート

次に自分のいる位置の座標を取得し、取得した値をもとに離れた場所へテレポートするコードを書いてみます。

新しいコードを書くときはThonnyの画面上で、**New**をクリックし、開いた新しいタブにコードを書いていきます。

自分のいる位置の座標は以下のコードで取得することができます。

{% highlight js %}
x, y, z = mc.player.getPos()
{% endhighlight %}

それでは、これを使って**x方向に10歩進んだところまでテレポート**してみます。コードは以下のようになりました。

{% highlight js %}
from mcpi.minecraft import Minecraft 
mc = Minecraft.create() 

x, y, z = mc.player.getPos() #プレイヤーの現在位置を取得
mc.postToChat('x=' + str(x) + 'y=' + str(y) + 'z=' + str(z)) #座標をチャットに表示

mc.player.setPos(x+10, y, z) #プレイヤーの位置をx方向に10ブロック移動

x, y, z = mc.player.getPos() #プレイヤーの移動後の位置を取得
mc.postToChat('x=' + str(x) + 'y=' + str(y) + 'z=' + str(z)) #座標をチャットに表示
{% endhighlight %}

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-04-07.jpg" loading="lazy">
    <img src="/images/b-04-08.jpg" loading="lazy">
  </div>
 <em>建物の左側にいましたが、コードを実行して右側に移動しました。</em>
</div>

上記コードではチャットに現在地を表示するために**mc.postToChat**を追加しました。入れなくても構いません。

行きたい場所の座標がすでに決まっている場合は、上記のコードの**mc.player.setPos(x, y+10, z)**の座標を行きたい座標に置き換えて実行すると、その場所へテレポートできます。

<br>

### プログラミングでブロックを設置

今度はプログラミングでブロックを配置していきたいと思います。

ブロックの指定には、ブロックIDを使います。

ブロックIDは、[<span style="color:#1589FF">こちらのサイト</span>](https://www.davesmotleyprojects.com/raspi/minecraft/blocks.html)で確認しました。ブロックの画像と一緒にIDを一覧にしてくれているので便利です。

今回は金のブロックID、41を使ってコードを書いていきます。

<br>

**1.まずは金のブロック一個置き**

まずはブロックを一個だけ置いていきます。

以下のコードでブロックを設置できます。

{% highlight js %}
from mcpi.minecraft import Minecraft 
mc = Minecraft.create() 

x, y, z = mc.player.getPos() #プレイヤーの現在位置を取得
mc.setBlock(x+1, y, z, 41) #プレイヤーの位置の隣にブロックを設置
{% endhighlight %}

上記コードでは、**自分の座標を取得後、mc.setBlockの座標指定を(x+1, y, z)とする**ことで、自分の立っている位置からx方向に一個動いた場所に金ブロックを置いています。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-04-09.jpg" loading="lazy">
  </div>
 <em>自分の立っている位置からx方向に+1した場所に金ブロックを一個置きました。</em>
</div>

<br>

**2.複数のブロックを一気に設置**

次に複数のブロックを一度に置いてみます。

以下のコードで金のブロックを3x3x3のサイズで置きました。

{% highlight js %}
from mcpi.minecraft import Minecraft 
mc = Minecraft.create() 

x, y, z = mc.player.getPos() #プレイヤーの現在位置を取得
mc.setBlocks(x+1, y, z, x+3, y+2, z+2, 41) #プレイヤーの位置の隣に3x3x3のサイズでブロックを設置
{% endhighlight %}

一つ前で書いたコード内のmc.setBlockが、複数形の**mc.setBlocks**になっている点に注意です。

座標指定部分は、**一番小さい座標 -> 一番大きい座標の順**に並べて書きます。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-04-10.jpg" loading="lazy">
  </div>
 <em>金のブロックを3x3x3のサイズで置きました。</em>
</div>

<br>

**3.中が空洞の直方体を設置**

最後に中が空洞の直方体を作成してみます。

外枠用のブロックで直方体を作った後に、中心部を空気ブロックで置き換えることで中を空洞にします。

空気ブロックのブロックID、0を使って、以下のコードを書きました。

{% highlight js %}
from mcpi.minecraft import Minecraft 
mc = Minecraft.create() 
x, y, z = mc.player.getPos()

mc.setBlocks(x+1, y, z, x+5, y+3, z+6, 41) #金ブロックを5x7x4で設置
mc.setBlocks(x+2, y+1, z+1, x+4, y+3, z+5, 0) #金の直方体の内側を空気ブロックで上書き設置
{% endhighlight %}

これで中が空洞の直方体ができました。屋根をつけたり装飾をして家にすることができます。

プログラムは上から順に実行されていきますので、金ブロックの後に空気ブロックを設置することで、空気ブロックで内側を上書きできます。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-04-11.jpg" loading="lazy">
  </div>
 <em>中が空洞の直方体ができました。大幅な時間短縮になりプログラミングの有り難みを感じてきます。</em>
</div>

<br>

### 歩いた場所にブロックを自動設置

**1.歩いた場所にお花を植える**

次に歩いた場所に自動でお花を植えていくコードを書いてみます。

while文を使うことで、コードが停止されるまでwhile内のプログラム（お花を植える）が実行されます。

コードは以下のようになります。

{% highlight js %}
from mcpi.minecraft import Minecraft
from time import sleep
mc = Minecraft.create()

while True:
    x, y, z = mc.player.getPos() #現在位置を取得
    mc.setBlock(x, y, z, 38) #現在位置に花のブロックを設置
    sleep(0.1)  #0.1秒待機
{% endhighlight %}

while内で**自分の位置を取得 -> お花を置く -> 待機**という動作がずっと続くようになっています。

プログラムを止める際にはキーボードでCtrl + Cを押して停止します。


<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-04-12-0.jpg" loading="lazy">
    <img src="/images/b-04-12-1.jpg" loading="lazy">   
    <img src="/images/b-04-13.jpg" loading="lazy">
  </div>
 <em>（中）プログラム実行前。（右）プログラム実行後に歩きまわって青いお花を植えました。</em>
</div>

<br>

**2.足元のブロックが草ブロックの時だけお花を植える**

先ほどのコードに、**足元のブロックの種類をチェックするコード**を加え、足元が草ブロックの時だけお花を植えるようにしてみます。

if文を使うことで、条件に合致した時のみ、その後ろにある命令が実行されるようになります。

コードは以下のようになりました。

{% highlight js %}
from mcpi.minecraft import Minecraft
from time import sleep
mc = Minecraft.create()

while True:
    x, y, z = mc.player.getPos() #現在位置を取得
    block_beneath = mc.getBlock(x, y-1, z) #足下のブロックの種類を取得してblock_beneathに代入
    if block_beneath == 2: #もし下にあるブロックが草であれば
        mc.setBlock(x, y, z, 38) #現在位置に花のブロックを設置
    sleep(0.1) #0.1秒待機
{% endhighlight %}

石レンガブロックを並べた上で、上記を実行して歩き回り、花壇を作りました。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-04-14.jpg" loading="lazy">
  </div>
 <em>石レンガブロックで囲まれた花壇の内側だけにお花を植えられました。</em>
</div>

<br>

### TNTを爆発！

Pi EditionのクリエイティブモードではTNTの爆発ができません。

しかし**コード内でデータ値を指定して設置する**と、着火して爆発するTNTを置くことができます。

以下のコードのように、TNTのブロックID46の後ろにデータ値1を追加しました。

{% highlight js %}
from mcpi.minecraft import Minecraft 
mc = Minecraft.create() 

x, y, z = mc.player.getPos()
mc.setBlocks(x+1, y, z, x+3 y+2, z+2, 46,1) #TNTのブロックID46の後ろにデータ値1を追加
{% endhighlight %}

TNTブロックが置けたら、あとは叩くだけでTNTが爆発します！

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-04-15.jpg" loading="lazy">
  </div>
 <em>データ値1を指定して置いたTNTはクリエイティブモード内でも爆発させることができます。</em>
</div>


<br>

### 叩いたブロックがダイヤモンドに変わる！？

最後に、叩いたブロックがダイヤモンドに変わるプログラムを試してみます。

コードは[<span style="color:#1589FF">こちらのブログ</span>](https://raspberrytips.com/program-minecraft-raspberry-pi/)を参考にしました。

ちょっと長いですが、コードは以下のようになります。

{% highlight js %}
from mcpi.minecraft import Minecraft
from time import sleep
mc = Minecraft.create()

try:
    while True:
        blockEvents = mc.events.pollBlockHits() #ブロックのヒットイベントを取得
        if blockEvents: #もしヒットイベントがあれば
            for blockEvent in blockEvents: #各ヒットイベントに対して処理を実行
                mc.postToChat('Hit detected') #チャットにヒットが検出されたことを表示
                x,y,z = blockEvent.pos #ヒットしたブロックの位置を取得
                mc.setBlock(x,y,z,56) #ヒットしたブロックの位置にブロックID56（ダイヤモンドブロック）を設置
        sleep(1) #1秒待機
except KeyboardInterrupt:
    print('Stopped') #Ctrl+C時にThonny画面上でStoppedのメッセージを表示
{% endhighlight %}


叩くときは、ブロックを持っていない状態にするか、剣などに持ち替えて右クリックで叩きます。

チャット欄に"Hit detected"の表示がされると共に叩いたブロックが変わります。

ダイヤモンドを指定しているIDを変えればTNTなど別のブロックにもできますよ。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-04-17.jpg" loading="lazy">
    <img src="/images/b-04-18.jpg" loading="lazy">
  </div>
 <em>Hit detectedの表示と共に金ブロックがダイヤモンドブロックに置き換わりました。</em>
</div>


***

## まとめ

ラズパイで遊べるマイクラを使い、子どもとプログラミングをしてみました。

まだ一人で書くことは難しいですが、ブロックIDを変えて好きなブロックを置いたり、大きな建築物を作るときにはプログラミングで置こうと提案してきたり、プログラミングを介した遊び方を子どもなりに楽しんでいました。

爆発するTNTやブロックの自動設置、ヒットでのブロックの置き換えなどはプログラミングならではの遊びなので、うまく動くと面白いと思います。

特段難しい手順もなく簡単に始められるので、子どもと試しにやってみるには良いチャレンジでした。

***

参考サイト
* [Getting Started with Minecraft Pi](https://projects.raspberrypi.org/en/projects/getting-started-with-minecraft-pi/0)
* [How to program Minecraft with Python on a Raspberry Pi?](https://raspberrytips.com/program-minecraft-raspberry-pi/)


