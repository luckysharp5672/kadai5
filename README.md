# kadai5
Authenticationを使ってアカウント登録必要なチャットアプリ

## DEMO

  - Firebase Hostingでのデプロイをしようとしたが、下記のエラーが出てきたので諦めました。
　　Authenticationを入れると課金が必要になるのでしょうか？
  
Error: Your project kizuna-chat-caccf must be on the Blaze (pay-as-you-go) plan to complete this command. Required API compute.googleapis.com can't be enabled until the upgrade is complete. To upgrade, visit the following URL:

https://console.firebase.google.com/project/kizuna-chat-caccf/usage/details

## 紹介と使い方

  - アカウント登録時にEメール, パスワード, ユーザー名を登録して、ユーザー名はRealtime Databaseに記録しました。ログインをするとアカウント登録で登録したユーザー名が自動で表示されるようにしています。

  - ログインすると名前のところにユーザー名が表示され、送信ボタンを押すとメッセージを送れます。

  - チャット内容は画面下部に表示されます。

## 工夫した点

  - アカウント登録時に登録したユーザー名が自動で名前として表示される

  - ログイン情報を見て、自分のチャットの場合は画面右側に、その他の人のチャットは画面左側に表示されるようにしました。

  - それぞれのチャットは”X”ボタンを押すと削除できるようにしました。

## 苦戦した点

  - アカウント登録時に登録したユーザー名を取得して表示させるのに苦労しました。ユーザー名をRealtime DatabaseにUIDと紐づけて保存できることを知って、何とかかいけつできました。

## 参考にした web サイトなど

  - ChatGPTに伴走してもらいました。
