# 大学会館予約システム

<img src="https://github.com/ryo773/ERMS/blob/master/public/images/logo.png" width="320px">

大学会館の予約・利用の利便性、効率性を向上させるべく、本システムを構築しました。

## イベントカレンダー
イベント情報を表示（本日から30日先までのイベント情報を閲覧可能）
<img width="1308" alt="スクリーンショット 2023-09-09 13 08 52" src="https://github.com/ryo773/ERMS/assets/135567732/d99554ba-bcd6-4da3-9d42-4f712d81d1eb">

## イベント詳細・予約画面
予約人数を選択して予約
<img width="1259" alt="スクリーンショット 2023-09-09 13 10 04" src="https://github.com/ryo773/ERMS/assets/135567732/a7b50f09-c457-4326-83df-8f9bebf04a3b">

## イベント新規登録画面
イベントの新規登録
<img width="1272" alt="スクリーンショット 2023-09-09 13 09 17" src="https://github.com/ryo773/ERMS/assets/135567732/0d37981f-96da-4900-a5b9-708cf9511e16">

## イベントキャンセル画面
イベントをキャンセルできる
<img width="1230" alt="スクリーンショット 2023-09-09 13 10 28" src="https://github.com/ryo773/ERMS/assets/135567732/4b4dea15-3b8f-4959-b513-6d588d22c082">

## 予約済みのイベント一覧表示
予約後、マイページに予約済みのイベント一覧として表示される。
<img width="1262" alt="スクリーンショット 2023-09-09 13 10 17" src="https://github.com/ryo773/ERMS/assets/135567732/b7610572-2055-4248-a708-2387a243b17e">

## 予約確定後画面
予約確定後、再度同じイベント詳細に遷移すると、「このイベントは既に予約済み」と表示
<img width="805" alt="スクリーンショット 2023-09-09 14 06 06" src="https://github.com/ryo773/ERMS/assets/135567732/02cf0573-cad6-4a02-bb0e-30d03b057d4b">

## ER図
<img width="779" alt="スクリーンショット 2023-09-09 14 26 58" src="https://github.com/ryo773/ERMS/assets/135567732/81d94cdf-f78b-4d6c-884f-79aa5285897a">

<p>・usersテーブル：ユーザーのログイン情報を保存するテーブル</p>
<p>・eventsテーブル:イベント情報を保存するテーブル</p>
<p>・reservationsテーブル：ユーザーの予約情報を保存するテーブル</p>

## Futures
<p>メールアドレス認証機能</p>
<p>通知機能</p>

## Requirement
<p>"php": "^8.0.2"</p>
<p>"guzzlehttp/guzzle": "^7.2"</p>
<p>"laravel/framework": "^9.19"<p>
<p>"laravel/jetstream": "^3.0"</p>
<p>"laravel/sanctum": "^3.0"</p>
<p>"laravel/tinker": "^2.7"</p>
<p>"livewire/livewire": "^2.11"</p>

## Installation
GitHubからファイルをクローン
```bash
https://github.com/ryo773/erms.git
```
vendorファイルとcomposer.lockを作成
```bash
cd erms/
composer install
```
.envファイルを作成
```bash
cp .env.example .env
```
.envファイル内の項目を変更してデータベースを有効化
```bash
DB_DATABASE=<使用するデータベース名>
DB_USERNAME=<ユーザーの名前>
DB_PASSWORD=<データベースのパスワード>
```
.envファイル内の項目を変更してpusherを有効化(pusherのAppKeysを設定)
```bash
BROADCAST_DRIVER=pusher

PUSHER_APP_ID=<App Keysのapp_id>
PUSHER_APP_KEY=<App Keysのkey>
PUSHER_APP_SECRET=<App Keysのsecret>
PUSHER_APP_CLUSTER=<App Keysのcluster>
```
アプリケーションキーを作成
```bash
php artisan key:generate
```
マイグレーションとシーディングを実行
```bash
php artisan migrate --seed
```
ストレージをリンク
```bash
php artisan storage:link
```

## Usage
機動する
```bash
php artisan serve --port=8080
```

## Note
現在作成中のアプリケーションのため、不具合を見つけた際には下記の連絡先までご連絡ください.

## Author
<p>・作成者: 小野凌平</p>
<p>・所属: 岡山大学　経済学部　経済学科</p>
<p>・E-mail: ryohei2323dat@gmail.com</p>



