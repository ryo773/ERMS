<img src="https://github.com/ryo773/ERMS/blob/master/public/images/logo.png" width="320px">

## 
<img width="1308" alt="スクリーンショット 2023-09-09 13 08 52" src="https://github.com/ryo773/ERMS/assets/135567732/d99554ba-bcd6-4da3-9d42-4f712d81d1eb">
<img width="1260" alt="スクリーンショット 2023-09-09 13 09 06" src="https://github.com/ryo773/ERMS/assets/135567732/129cc066-8418-46a0-b172-ba725ca28640">
<img width="1272" alt="スクリーンショット 2023-09-09 13 09 17" src="https://github.com/ryo773/ERMS/assets/135567732/0d37981f-96da-4900-a5b9-708cf9511e16">

<img width="1259" alt="スクリーンショット 2023-09-09 13 10 04" src="https://github.com/ryo773/ERMS/assets/135567732/a7b50f09-c457-4326-83df-8f9bebf04a3b">

<img width="1262" alt="スクリーンショット 2023-09-09 13 10 17" src="https://github.com/ryo773/ERMS/assets/135567732/b7610572-2055-4248-a708-2387a243b17e">

<img width="1230" alt="スクリーンショット 2023-09-09 13 10 28" src="https://github.com/ryo773/ERMS/assets/135567732/4b4dea15-3b8f-4959-b513-6d588d22c082">

<img width="805" alt="スクリーンショット 2023-09-09 14 06 06" src="https://github.com/ryo773/ERMS/assets/135567732/02cf0573-cad6-4a02-bb0e-30d03b057d4b">


git clone

git clone https://github.com/ryo773/erms

git clone ブランチを指定してダウンロードする場合

git clone -b ブランチ名 https://github.com/ryo773/erms

もしくはzipファイルでダウンロードして下さい


## インストール方法
cd erms
composer install
npm install
npm run build
.env.example をコピーして .envファイルを作成

.envファイルの中の下記をご利用の環境に合わせて変更してください。

DB_CONNECTION=mysql DB_HOST=127.0.0.1 DB_PORT=3306 DB_DATABASE=erms DB_USERNAME=dbuser DB_PASSWORD=negiryou17

XAMPP/MAMPまたは他の開発環境でDBを起動した後に、

php artisan migrate:fresh --seed

と実行してください。(データベーステーブルとダミーデータが追加されればOK)

最後に php artisan key:generate と入力してキーを生成後、

php artisan serve --port=8080で簡易サーバーを立ち上げ、表示確認してください。


## インストール後の実施事項

画像のリンク php artisan storage:link

プロフィールページで画像アップロード機能を使う場合は、 .envのAPP_URLを下記に変更してください。


