---
title: Style-Bert-VITS2の使い方
description: DigitalCloneVの導入
slug: DigitalCloneV/howto/howto_sbv2
---

## はじめに

[Style-Bert-VITS2](https://github.com/litagin02/Style-Bert-VITS2)<br>
ここではStyle-Bert-VITS2の簡単な使い方を説明します。<br>
導入方法は[Style-Bert-VITS2の導入](../install/install_sbv2/)の記事を参考にしてください。<br>
Style-Bert-VITS2公式が用意してくださった解説動画もありますのでこちらも参考にしてください。<br>
[Style-Bert-VITS2解説動画](https://www.youtube.com/watch?v=aTUSzgDl1iY)<br>

## 音声学習

まず音声学習させる為にあなたの声の音声データが必要です。<br>
録音時間が長い程学習の精度が上がるので10分～20分程度の音声を用意するとよいです。<br>

こちらに朗読用のサンプル文を用意したのでご利用ください。<br>
[朗読文(ひらがな)](/kiokuya/files/sbv2/speech_text.txt)
[朗読文(漢字)](/kiokuya/files/sbv2/speech_text_kanji.txt)

![sbv2](/kiokuya/images/sbv2/sbv2_inputs.png)

音声ファイルが用意できたらStyle-Bert-VITS2のinputsフォルダの中にそのファイルを置いてください。<br>

![sbv2](/kiokuya/images/sbv2/sbv2_app_bat.png)

Style-Bert-VITS2のフォルダの中にあるApp.batをダブルクリックしてStyle-Bert-VITS2を起動してください。<br>
起動が成功したらブラウザにWebUIが表示されます。<br>

![sbv2](/kiokuya/images/sbv2/sbv2_ui.png)

上部のタブから「データセット作成」を選択してください。<br>

![sbv2](/kiokuya/images/sbv2/sbv2_ui_slice.png)

任意のモデル名を入力して「スライスを実行」ボタンを押してください。<br>
それほど時間がかからずに右側の結果に「音声のスライスが完了しました。」と表示されると思います。<br>

![sbv2](/kiokuya/images/sbv2/sbv2_ui_word.png)

続いて下の「音声の文字起こし」ボタンを押してください。<br>
2分～5分程度に右側の結果に「音声の文字起こしが完了しました。」と表示されると思います。<br>

![sbv2](/kiokuya/images/sbv2/sbv2_ui_auto_pre.png)

上部タブから「学習」を選択してください。<br>
モデル名に先ほどと同じ名前を入力して「自動前処理を実行」ボタンを押してください。<br>
2分～5分程度で右側の状況に「Success:~」と表示されると思います。<br>

![sbv2](/kiokuya/images/sbv2/sbv2_ui_auto_pre_cmd.png)

App.batを実行した時に同時に立ち上がったターミナル(黒い画面)を見ると一番下に「Success」とあるので成功していると思われます。<br>
その上でワーニングが出ていますが結果はSuccessなので多分大丈夫だと思います。<br>

![sbv2](/kiokuya/images/sbv2/sbv2_ui_learn.png)

続いて下部の「学習を開始する」ボタンを押してください。<br>
学習はかなり時間がかかり、PCのスペックをかなり使うのでその後PCでしばらく作業できなくなります。<br>
学習時間は音声ファイルのデータ量次第ですが30分以上はかかると思ってください。<br>
下の状況が「Success:~」になったら完了です。<br>

## 動作確認

![sbv2](/kiokuya/images/sbv2/sbv2_ui_use.png)

Style-Bert-VITS2 WebUIの上部タブで「音声合成」を選択してください。<br>

![sbv2](/kiokuya/images/sbv2/sbv2_ui_use_done.png)

ページ下部までスクロールすると音声合成UIがあります。<br>
「モデル一覧」からあなたの音声AIモデルを選択してください。<br>
一覧にあるはずなのに出てこない場合は右の「更新」ボタンを押してください。<br>

モデルを選択したらその右の「ロード」ボタンを押してください。<br>
任意のテキストを入力し、右の「音声合成」ボタンを押してください。<br>
少し待つと結果に再生ボタンなどが表示されると思います。<br>

再生ボタンを押してきちんとあなたの声で話してくれたら音声AIモデル作成は成功です。<br>