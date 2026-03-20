# CFn Template

> **Note:** このリポジトリはアーカイブ済みです。メンテナンスは行われていません。

AWS Backup の汎用 CloudFormation テンプレートです。

## 概要

タグベースで日次・週次・月次のバックアッププランを構成する CloudFormation テンプレート（`awsbackup.yaml`）を提供します。

### 主な機能

- **日次バックアップ** — `DailyBackup: true` タグが付いたリソースを毎日バックアップ
- **週次バックアップ** — `WeeklyBackup: true` タグが付いたリソースを毎週金曜にバックアップ
- **月次バックアップ** — `MonthlyBackup: true` タグが付いたリソースを毎月1日にバックアップ
- **S3 対応** — S3 バックアップ/リストア用の IAM ポリシーを含む
- **クロスリージョンコピー** — コメントアウト済みだが、設定を有効化可能

## 関連記事

- [AWS Backup for S3でCross-Region backup](https://zenn.dev/isseeeeey55/articles/7ab17344ad0a46)
