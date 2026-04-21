---
title: FFmpegの導入
description: DigitalCloneVの導入
slug: DigitalCloneV/install/install_ffmpeg
---

## はじめに

DigitalCloneVではStyle-Bert-VITS2を利用しており、Style-Bert-VITS2を使うにはFFmpegが必要です。<br>
FFmpegを使うにはダウンロード・解凍・PATHを通す必要があります。<br>
以下にその手順を説明します。<br>

## ダウンロード・解凍

<a href="https://ffmpeg.org/" target="_blank" rel="noopener noreferrer">FFmpeg公式サイト</a> に移動します。<br>

![FFmpeg Home](/kiokuya/images/ffmpeg/ffmpeg_home.png)

上の画像の赤丸のDownloadボタンを押してください。<br>
すると以下のような画面になります。<br>

![FFmpeg Windows](/kiokuya/images/ffmpeg/ffmpeg_windows.png)

上の画像の赤丸の所にマウスカーソルを移動するとWindows用のダウンロードリンクが表示されると思います。<br>
Windows用のダウンロードリンクが表示されたら上の画像の下の赤丸のリンクをクリックしてください。<br>
(多分[Windows builds from gyan.dev]と記載されているものです)<br>

![CODEX FFMPEG](/kiokuya/images/ffmpeg/ffmpeg_codex.png)

上の画像のページに飛べたと思います。<br>
これはFFmpegを配布しているページです。<br>
そのページを下の方にスクロールすると「release builds」の項目があります。<br>

![release builds](/kiokuya/images/ffmpeg/ffmpeg_release_build.png)

赤丸で囲った「latest release」の中からお好きなものをクリックしてダウンロードしてください。<br>
DigitalCloneV及びStyle-Bert-VITS2ではffmpeg-release-essentialsの方で動作することを確認していますので「essentials」の方で問題ないと思います。<br>
.7zipと.zipについては使用しているPCに7zipが対応しているのであれば.7zipで良いと思います。<br>
7zipって何？という状況であれば.zipを選ぶと良いです。<br>
ダウンロードの保存先はどこでもよいです。<br>
ダウンロードしたらzip解凍してください。<br>

![zip解凍画面](/kiokuya/images/ffmpeg/ffmpeg_download_folder.png)

解凍したフォルダを任意の場所に移動してください(C:\FFmpegがおすすめです。日本語表記のフォルダの下に置くとエラーが出る可能性もあります)。<br>

![ffmpeg保存先](/kiokuya/images/ffmpeg/ffmpeg_folder_c.png)

## PATHを通す

ダウンロード・解凍が完了したらPATHを通す作業を行います。<br>
ダウンロードしただけではPCのシステム(OS)から見てまだ使えない状況で、「FFmpegがここにあるよ」ってPCに教えてあげることによってPCはFFmpegを使用できるようになります。<br>
これを環境変数のPATHを通すと言います<br>

まずキーボードのwindowsキー+Rキーを押してください。<br>

![win R](/kiokuya/images/ffmpeg/ffmpeg_winr.png)

上の画像のタブが出てきたら「sysdm.cpl」と入力してシステムのプロパティを開いてください。<br>

![システムプロパティ](/kiokuya/images/ffmpeg/ffmpeg_system_property.png)

上のタブの「詳細設定」を押してください。<br>

![詳細設定](/kiokuya/images/ffmpeg/ffmpeg_system_env.png)

赤丸の「環境変数(N)」ボタンを押してください。<br>

![環境変数](/kiokuya/images/ffmpeg/ffmpeg_system_env_user.png)

赤丸のユーザー環境変数の「Path」を選択して「編集(E)」ボタンを押してください。<br>

![環境変数名の編集](/kiokuya/images/ffmpeg/ffmpeg_system_env_path_edit.png)

赤丸の「新規(N)」ボタンを押してください。<br>
入力欄が追加されると思うのでそこにFFmpegの中のbinフォルダのPATHを入力します。<br>
下の画像のような感じで入力してください。<br>
(例: C:\FFmpeg\ffmpeg-8.1-essentials_build\bin)

![環境変数 FFmpeg](/kiokuya/images/ffmpeg/ffmpeg_system_env_path_edit_ffmpeg.png)

入力が終わったら各ウィンドウの「OK」ボタンを押して閉じてください。<br>

これでFFmpegの導入は完了です。