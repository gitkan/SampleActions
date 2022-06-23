# SampleActions

## GitHub Actions
### check file content 🆖
[![check file content](https://github.com/gitkan/SampleActions/actions/workflows/public_repository_scan.yml/badge.svg)](https://github.com/gitkan/SampleActions/actions/workflows/public_repository_scan.yml)

### Gitleaks scanning 🆗
[![gitleaks scanning](https://github.com/gitkan/SampleActions/actions/workflows/gitleaks_action.yml/badge.svg)](https://github.com/gitkan/SampleActions/actions/workflows/gitleaks_action.yml)
<img alt="gitleaks badge" src="https://img.shields.io/badge/protected%20by-gitleaks-blue">
- https://github.com/gitleaks/gitleaks-action
- https://github.com/zricethezav/gitleaks

#### サンプル実装および結果
- :page_facing_up: サンプル実装　：[gitleaks_action.yml](/.github/workflows/gitleaks_action.yml)
- 💻 出力結果（例）
```
{
	"Description": "GitHub Personal Access Token",
	"StartLine": 2,
	"EndLine": 2,
	"StartColumn": 2,
	"EndColumn": 41,
	"Match": "REDACTED",
	"Secret": "REDACT",
	"File": "/path/dummy_code.md",
	"Commit": "",
	"Entropy": 4.234184,
	"Author": "",
	"Email": "",
	"Date": "",
	"Message": "",
	"Tags": [],
	"RuleID": "github-pat"
}
11:46AMINF scan completed in 1.599148424s
11:46AMWRN leaks found: 2
Error: Process completed with exit code 2.
```
- 📫 メール通知（例）
<img width="393" alt="image" src="https://user-images.githubusercontent.com/2616832/175293586-763f17a1-402e-4fc9-8b77-f5fec04da12e.png">


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
~~やはり方向性として効果が薄い（誤検知が多い）と思われるで、上記タスクは一旦放置。
secret scanningや、サードパーティ製品の利用検討をしてください。~~
gitleaksでのスキャン結果はActionsで確認してみてください。
ある程度のパターンは拾える形になっているかと。
