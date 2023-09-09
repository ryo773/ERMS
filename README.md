<img src="https://github.com/ryo773/ERMS/blob/master/public/images/logo.png" width="320px">

## 
<img width="1308" alt="スクリーンショット 2023-09-09 13 08 52" src="https://github.com/ryo773/ERMS/assets/135567732/d99554ba-bcd6-4da3-9d42-4f712d81d1eb">
<img src="" width="320px">
<img src="" width="320px">
<img src="" width="320px">

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


