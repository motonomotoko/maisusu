---
layout: post
title: Raspberry Piにマインクラフトをいれる簡単な方法
description: Raspberry Piにマインクラフトをインストールする方法です。 
date:   2023-05-03 15:00:00 +0300
image:  '/images/b-02-00.jpg'
video_embed:
tags:   [Raspberry Pi, プログラミング]
---

世界でも大人気のマイクラ、Raspberry Piでも遊ぶことができます。

公式のMinecraftランチャーは利用できませんが、Pi Editionや非公式のランチャーを利用することができ、インストールもとても簡単。ものの数分で遊び始めることができます。

この記事では、Raspberry Piにマイクラをインストールする簡単な方法を紹介します。

<div style="padding: 10px; margin-bottom: 10px; border: 1px solid #181818; background-color: var(--background-alt-color); border-radius: 5px;" markdown="1">
<h4>目次</h4>
* table
{:toc}
</div>

***

## Raspberry PiでMinecraft Pi Editionをプレイする

Minecraft Pi Editionとは、Raspberry Pi用に開発されたマイクラです。

公式サポートは終了しており、ブロックやMobなど種類は少ないですが、なんといっても無料で遊べることと、プログラミングと連携しやすいことが大きな魅力です。

<br>

### 手順１：Pi-Appsをインストールする

Pi-Appsはアプリケーションのインストールを簡単にしてくれる無料ツールです。Pi-Appsでサポートされているアプリケーションであれば、ワンクリックで目的のアプリケーションをインストールしてくれます。

1.[<span style="color:#1589FF">Pi-Apps公式Webサイトのインストールページ</span>](https://pi-apps.io/install)を開きます。

2.Raspberry Piでターミナルを開き、上記で開いたページの一番上のコマンドをコピペします。
{% highlight css %}
wget -qO- https://raw.githubusercontent.com/Botspot/pi-apps/master/install | bash
{% endhighlight %}
![Sea]({{site.baseurl}}/images/b-02-01.jpg)

3.インストール完了後は、Main MenuとデスクトップにPi-Appsのアイコンが追加されます。

![Sea]({{site.baseurl}}/images/b-02-02.jpg)

これで、Pi-Appsのインストールは完了です。

<br>

### 手順２：Pi-AppsでMinecraft Pi Editionをインストールする

1.Main Menuまたはデスクトップから**Pi-Apps**を開きます。

2.アプリケーションのリストが表示されるため、**Games**を選択します。
![Sea]({{site.baseurl}}/images/b-02-03.jpg)

3.**Minecraft Pi (Modded)**を選択し、右下に表示される**Install**を選択します。
![Sea]({{site.baseurl}}/images/b-02-04.jpg)

4.あとは何もせずインストール完了するまで待ちます。インストール完了後は、Main MenuのGamesの中にMinecraft Pi (Modded)が追加されます。

<br>

### 手順３：Minecraft Pi Editionを開く

1.Main Menuから**Games -> Minecraft Pi (Modded)**を選びます。

2.ゲームを始める前にいくつか設定確認画面が現れます。設定は変更しなくても良いですし、いろいろ変えて試しても良いです。
![Sea]({{site.baseurl}}/images/b-02-06.jpg)

我が家では以下の値を変更してから遊んでいます。

* Animated Waterのチェックを外す（処理が軽くなることを期待して）
* Expand Creative Mode Inventoryのチェックをつける（クリエイティブモードで使えるブロックを増やします）
* Remove Creative Mode Restrictionsのチェックをつける（クリエイティブモードでクラフトができるようになります）

3.設定が終わるとゲーム開始画面が現れます。**Start Game**を選択し、**Create new**を選択してワールドを作成します。ワールドの名前、クリエイティブ／サバイバル、シード値（入れなくて構いません）を設定後、ゲームが始まります。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-02-07.jpg" loading="lazy">
    <img src="/images/b-02-08.jpg" loading="lazy">
  </div>
</div>

***

## Raspberry PiでMinecraft Java版をプレイする

Raspberry Pi上でJava版を遊ぶことも可能です。こちらもPi-Appsから利用可能なランチャーをインストールして遊びます。

ランチャーにもいくつか種類がありますが、私の環境ではMinecraft Java GDLauncherを使ってJava版を動かせることを確認しました。

<br>

### 手順１：Pi-Appsをインストールする

まだインストールされていない場合は、上記の[<span style="color:#1589FF">Pi-Appsをインストールする</span>](https://www.maisusu.com/blog/install-minecraft-on-raspberry-pi#%E6%89%8B%E9%A0%86%EF%BC%91pi-apps%E3%82%92%E3%82%A4%E3%83%B3%E3%82%B9%E3%83%88%E3%83%BC%E3%83%AB%E3%81%99%E3%82%8B)をご参照ください。

<br>

### 手順２：Pi-AppsからMinecraft Java GDLauncherをインストールする

1.Main Menuまたはデスクトップから**Pi-Apps**を開きます。

2.アプリケーションのリストが表示されるため、**Games**を選択します。

3.**Minecraft Java GDLauncher**を選択し、右下に表示されている**Install**を選択します。
![Sea]({{site.baseurl}}/images/b-02-09.jpg)

4.あとは何もせずインストール完了するまで待ちます。インストール完了後は、Main MenuのGamesの中にMinecraft Java GDLauncherが追加されます。

<br>

### 手順３：Minecraft Java GDLauncherを開く

1. Manin Menuから**Games -> Minecraft Java GDLauncher**を開きます。

2. Javaが不足している場合、初回起動時に以下のようなウィンドウが表示されます。この場合は**Automatic Setup**をクリックしてランチャーがJavaをインストールするのを待ちます。
![Sea]({{site.baseurl}}/images/b-02-11.jpg)

3. サインインします。Java版を購入しているアカウントを入力してサインインします。
![Sea]({{site.baseurl}}/images/b-02-12.jpg)

4. サインインすると、制作チームへのサポート方法が書かれたメッセージが画面に表示されます。画面右下の矢印を押して下にスクロールしていくと、インスタンス作成画面になります。画面左下にあるプラス（＋）ボタンを選択しインスタンスを作成しましょう。最初はVanillaの最新バージョンで試すのがお勧めです。
![Sea]({{site.baseurl}}/images/b-02-13.jpg)

5. インスタンスができたら選択してゲームを開始します。初回のみナレーション等が必要か確認画面があり、**Continue**を選択すると見慣れた画面が出てきます。ワールド作成まではしばらく時間がかかりますが、ゆったり休憩をしてまた覗いてみてください。
![Sea]({{site.baseurl}}/images/b-02-14.jpg)

<br>

**補足.** **Invalid maximum heap size**というエラーが出た場合は、GDLauncherの設定画面でJavaのタブから**Java Memory**を**1024 MB**に変更するとエラーを回避できます。しかし、どうしても処理が遅くなってしまいます。検索すると64ビットの環境を作って解決を試みている方もいたので、機会があれば検証してみたいと思います。

<div class="gallery-box">
  <div class="gallery">
    <img src="/images/b-02-15.jpg" loading="lazy">
    <img src="/images/b-02-16.jpg" loading="lazy">
  </div>
</div>

***

## まとめ

この記事ではRaspberry Piでマイクラを遊ぶための手順をまとめました。

Pi-Appsを利用することで、思いの外簡単にマイクラを導入できます。

特にPi Editionは、Raspberry Pi専用というだけありとても快適に遊べます。


正規品に比べるとブロックなどの種類は少ないですが、無料で遊べ、しかもプログラミング言語との接続も簡単にできるので、使い方次第でとても楽しめそうです。

Raspberry Piでマイクラ、もしご自宅にRaspberry Piがあればぜひお試しください。


