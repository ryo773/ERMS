# 大学会館予約システム

<img src="https://github.com/ryo773/ERMS/blob/master/public/images/logo.png" width="320px">

ゲーム好きな人が一緒に遊ぶ仲間を探すことができるマッチングアプリ
自身がゲーム好きであり、一緒にゲームを遊ぶ仲間を探すことが難しいと感じたことからこのアプリケーションの開発に取り組む.
仲間を探したいゲームを選択し、プロフィールを設定した後マッチング画面に出てくる人をGood or Badで選択できる.
お互いにGoodを選択した人同士でマッチングした後にはチャットで連絡を取ることも可能.


# 管理者画面
## イベントカレンダー
<img width="1308" alt="スクリーンショット 2023-09-09 13 08 52" src="https://github.com/ryo773/ERMS/assets/135567732/d99554ba-bcd6-4da3-9d42-4f712d81d1eb">

## 本日以降のイベント一覧画面
<img width="1260" alt="スクリーンショット 2023-09-09 13 09 06" src="https://github.com/ryo773/ERMS/assets/135567732/129cc066-8418-46a0-b172-ba725ca28640">

## イベント新規登録画面
<img width="1272" alt="スクリーンショット 2023-09-09 13 09 17" src="https://github.com/ryo773/ERMS/assets/135567732/0d37981f-96da-4900-a5b9-708cf9511e16">

# 予約者画面
## イベント予約画面
<img width="1259" alt="スクリーンショット 2023-09-09 13 10 04" src="https://github.com/ryo773/ERMS/assets/135567732/a7b50f09-c457-4326-83df-8f9bebf04a3b">

## 予約済みのイベント一覧表示
<img width="1262" alt="スクリーンショット 2023-09-09 13 10 17" src="https://github.com/ryo773/ERMS/assets/135567732/b7610572-2055-4248-a708-2387a243b17e">

## イベントキャンセル画面
<img width="1230" alt="スクリーンショット 2023-09-09 13 10 28" src="https://github.com/ryo773/ERMS/assets/135567732/4b4dea15-3b8f-4959-b513-6d588d22c082">

## ER図
<img width="779" alt="スクリーンショット 2023-09-09 14 26 58" src="https://github.com/ryo773/ERMS/assets/135567732/81d94cdf-f78b-4d6c-884f-79aa5285897a">

・　usersテーブル：ユーザーのログイン情報を保存するテーブル
・　eventsテーブル:イベント情報を保存するテーブル
・　reservationsテーブル：ユーザーへの通知メッセージを保存するテーブル

## Futures
マッチング機能
ログイン機能＆LINEログイン
リアルタイムチャット機能
マイページ＆プロフィール変更機能
通知機能
## Future features
 管理者ページの追加(新ゲームの追加などを行う)
 ゲーム別プロフィールの設定
 マッチング通知をLINEに通知
 チャット機能の強化(画像やファイルなどを送れるようにする)
 チャットのメッセージを全件取得から最新の何件かを取得するように変更する

## Requirement
php ^7.2.5|~8.0
doctrine/dbal ^3.4
fruitcake/laravel-cors ^2.0
guzzlehttp/guzzle ^7.0.1
laravel/framework ^8.75
laravel/sanctum ^2.11
laravel/tinker ^2.5
pusher/pusher-php-server ^7.0
league/flysystem-aws-s3-v3 ~1.0
laravel/ui 3.*


## Installation
Githubからファイルをクローン
vendorファイルとcomposer.lockを作成
.envファイルを作成
.envファイル内の項目を変更してデータベースを有効化
.envファイル内の項目を変更してpusherを有効化(pusherのAppKeysを設定)
アプリケーションキーを作成
マイグレーションを実行
ストレージをリンク

## Usage
機動する

## Note
現在作成中のアプリケーションのため、不具合を見つけた際には下記の連絡先までご連絡ください.

## Author
・ 作成者: 小野　凌平
・　 所属: 岡山大学　経済学部　経済学科
・ E-mail: ryohei2323dat@gmail.com
## Licence



## 予約確定後画面
<img width="805" alt="スクリーンショット 2023-09-09 14 06 06" src="https://github.com/ryo773/ERMS/assets/135567732/02cf0573-cad6-4a02-bb0e-30d03b057d4b">
