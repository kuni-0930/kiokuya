---
title: YoutubeAPIKeyの取得
description: DigitalCloneVの導入
slug: DigitalCloneV/install/install_youtube_apikey
---

## はじめに

YoutubeLiveのコメントを取得するのにYoutube API Keyが必要になります。<br>
ここではYoutube API Keyの取得方法を解説します。<br>

## APIKeyの取得


まず<a href="https://console.cloud.google.com/welcome?project=solid-space-459107-m0" target="_blank" rel="noopener noreferrer">Google Cloud Console</a>のページにいきます。<br>

![youtube](/kiokuya/images/youtube/youtube_new.png)

Consoleの画面で左上のところに「プロジェクトを選択」のようなボタンがあるのでそれをクリックしてください。<br>
出てきたウィンドウの「新しいプロジェクト」ボタンを押してください。<br>

![youtube](/kiokuya/images/youtube/youtube_create.png)

プロジェクト名は適当でよいです。<br>
親リソースは空欄でよいです。<br>
作成したらConsoleの画面で作成したプロジェクトの画面になっていることを確認してください。<br>
違う場合は左上のプロジェクト名の所をクリックすれば選択できます。<br>

![youtube](/kiokuya/images/youtube/youtube_search.png)

上部の検索欄で「youtube」と入力して出てくる「Youtube Data API v3」を選択してください。<br>

![youtube](/kiokuya/images/youtube/youtube_dataapi.png)

「有効にする」ボタンをクリックしてください。<br>

![youtube](/kiokuya/images/youtube/youtube_api.png)

「APIとサービス」画面にて「認証情報」を選択してください。<br>

![youtube](/kiokuya/images/youtube/youtube_api_key.png)

中上の「認証情報を作成」から「APIキー」を選択してください。<br>

![youtube](/kiokuya/images/youtube/youtube_key_info.png)

ブラウザの右側に出てくるウィンドウにて、キーの名前は適当な名前を入力してください。<br>
「APIの制限の選択」欄にて右の▼ボタンを押してドロップダウンリストの中から「Youtube Data API v3」にチェックを入れて「OK」ボタンをおしてください。<br>
「選択中のAPI:」に「Youtube Data API v3」があれば正しいです。<br>
上記ができたら下へスクロールして「作成」ボタンを押してください。<br>

![youtube](/kiokuya/images/youtube/youtube_key_num.png)

キーが作成できたら表示されます。<br>
このAPIキー番号はConsole画面からAPIキーを選択して詳細情報のところから再度表示させることが可能です。<br>
DigitalCloneVではこのキーを使用します。<br>


