# hanko-login-sample

Hankoライブラリを使ったログインのサンプルプロジェクトです。ユーザーはHankoを使って簡単にログインできます。

## デモ
[サンプルページ](https://code4fukui.github.io/hanko-login-sample/)でデモを確認できます。

## 機能
- Hankoを使ったログイン
- ログイン状態の保持（ブラウザのローカルストレージ）
- ログイン後にユーザーの公開鍵を表示
- ログアウト機能（セッション削除）

## 必要環境
特に必要ありません。ブラウザから利用可能です。

## 使い方
1. 「Hankoでログイン」ボタンをクリックします。
2. Hankoアプリでログイン処理を完了します。
3. ログイン後、ユーザー情報が表示されます。
4. 「ログアウト（セッション削除）」ボタンをクリックするとログアウトできます。

## データ・API
このプロジェクトでは以下の外部ライブラリを使用しています:
- [Hanko](https://github.com/code4fukui/hanko/) - 分散型認証
- [QRCode.js](https://js.sabae.cc/QRCode.js) - QRコード生成
- [DateTime.js](https://js.sabae.cc/DateTime.js) - 日時処理
- [Base32.js](https://code4fukui.github.io/Base32/Base32.js) - セッションIDのエンコーディング

## ライセンス
このプロジェクトは MIT ライセンスの下で提供されています。