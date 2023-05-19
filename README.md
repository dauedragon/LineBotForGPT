# LineBotForGPT

このリポジトリは、LINE上で動作するPythonベースのチャットボットです。このボットはChatGPT APIを使用して、ユーザからのメッセージに対してレスポンスを生成します。

## 必要な環境変数

このアプリケーションは以下の環境変数を必要とします。

- `OPENAI_APIKEY` : OpenAI APIのアクセスキー
- `LINE_ACCESS_TOKEN` : LINE Messaging APIのアクセストークン
- `MAX_DAILY_USAGE` : ユーザごとの最大日次利用回数
- `SECRET_KEY` : メッセージの暗号化/復号化に使用する秘密鍵
- `SYSTEM_PROMPT` : システムのプロンプト

これらの環境変数が設定されていない場合、チャットボットは適切に動作しません。

## データベースのセットアップ

このチャットボットはGoogle Cloud Firestoreを使用してユーザーデータを保存します。Firestoreを使用するには、以下のステップに従ってセットアップしてください：

1. Google Cloudプロジェクトを作成します：Google Cloud Consoleに移動し、新しいプロジェクトを作成します。

2. Firestoreを有効にします：左側のナビゲーションメニューで「Firestore」を選択し、Firestoreをプロジェクトで有効にします。

3. データベースを作成します：Firestoreダッシュボードに移動し、「データベースの作成」をクリックします。プロダクション環境の場合は、「ネイティブ」モードを選択します。

## デプロイ

このアプリケーションはFlaskベースで作成されています。そのため、任意のウェブサーバー上にデプロイすることが可能です。デプロイ方法は使用するウェブサーバーによります。

## 注意


## ライセンス

このプロジェクトはMITライセンスの下でライセンスされています。
