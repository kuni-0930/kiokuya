---
title: DigitalCloneV
description: きおく屋の提供するサービス
slug: DigitalCloneV/main
---

![DigitalCloneV](/kiokuya/images/DigitalCloneV/DigitalCloneV.png)

## はじめに

DigitalCloneVは配信でAIがあなたの代わりにあなたの声で受け答えするソフトです。<br>
もう少し詳しく言うと、あなたの性格データ、実際の体験談を元に、あなたのAIの分身を作り、あなたの体験談に忠実な話をあなたそっくりな声のAIがYoutubeLiveで話してくれるソフトです。<br>
このソフトを使う為にはいくつかの準備が必要です。<br>
準備はおおまかに以下のものです。<br>
- 初期設定
- FFmpegの導入
- Style-Bert-VITS2のインストール
- ファインチューニングデータ作成
- エンベッドデータ作成
- OpenAIAPIKeyの取得
- YoutubeAPIKeyの取得
- DigitalCloneVの設定

## 各項目の簡単な説明
### 初期設定
InitialSettings.exeを使ってあなたの名前や生年月日等を入力します。<br>

### FFmpegの導入
DigitalCloneVではStyle-Bert-VITS2を利用しており、Style-Bert-VITS2を使うにはFFmpegが必要です。<br>
[FFmpegの導入](../install/install_ffmpeg/)<br>

### Style-Bert-VITS2のインストール
AIの考えた返答をあなたの音声にするためにStyle-Bert-VITS2というAIを利用します。<br>
[Style-Bert-VITS2の導入](../install/install_sbv2/)

### ファインチューニングデータ作成
OpenAIであなたの性格を学習したAIモデルを作成します。<br>

### エンベッドデータ作成
あなたの体験談をAIが利用する為にデータを作成します。<br>

### OpenAIAPIKeyの取得
OpenAIの機能を使う為にAPIキーを取得します。<br>

### YoutubeAPIKeyの取得
Youtubeの機能を利用する為にAPIキーを取得します。<br>

### DigitalCloneVの設定
取得したAPIキーなどをDigitalCloneVの設定に入力します。<br>


