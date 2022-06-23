# SampleActions

## GitHub Actions
### check file content
[![check file content](https://github.com/gitkan/SampleActions/actions/workflows/public_repository_scan.yml/badge.svg)](https://github.com/gitkan/SampleActions/actions/workflows/public_repository_scan.yml)

### Gitleaks scanning
[![gitleaks scanning](https://github.com/gitkan/SampleActions/actions/workflows/gitleaks_action.yml/badge.svg)](https://github.com/gitkan/SampleActions/actions/workflows/gitleaks_action.yml)
<img alt="gitleaks badge" src="https://img.shields.io/badge/protected%20by-gitleaks-blue">

## Task List
### ＜input＞
- [x] キーワードを変数化
- [ ] 固定ユーザーのPublicリポジトリの配列から取得
- [ ] ユーザー配列からのPublicリポジトリの配列を取得

### ＜process＞
- [ ] ループ処理
- [x] チェックアウトを既定ジョブで
- [ ] matrix使った並列処理で

### ＜output＞
- [ ] ジョブ結果のOK/NG切替
- [ ] エラーリストを履歴で閲覧可能に（件数、ユーザー、リポジトリ、ファイルパス、検知行コンテンツ）
- [ ] 管理者通知で結果概要を伝える

## 効果
やはり方向性として効果が薄い（誤検知が多い）と思われるで、上記タスクは一旦放置。
secret scanningや、サードパーティ製品の利用検討をしてください。
