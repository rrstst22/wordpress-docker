## 概要
ローカルでwordpress用の開発環境を構築する。

## データ移行手順
### 1. Dataエクスポート
1. wp-contentをftpでバックアップ
2. データベースをphpmyadminでエクスポート
3. 2のsqlをzip化

### 2. Dataインポート
1. docker起動 (docker-compose up -d)
2. wp-content削除＆移動 (rm -rf wp-content) (mv ....)
3. データベースをphpmyadminでインポート
4. wp-optionsテーブルのsiteurlとhomeを変更
