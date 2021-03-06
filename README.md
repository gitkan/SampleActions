## GitHub Actions
### ð check file content
[![check file content](https://github.com/gitkan/SampleActions/actions/workflows/public_repository_scan.yml/badge.svg)](https://github.com/gitkan/SampleActions/actions/workflows/public_repository_scan.yml)

### ð Gitleaks scanning
[![gitleaks scanning](https://github.com/gitkan/SampleActions/actions/workflows/gitleaks_action.yml/badge.svg)](https://github.com/gitkan/SampleActions/actions/workflows/gitleaks_action.yml)
<img alt="gitleaks badge" src="https://img.shields.io/badge/protected%20by-gitleaks-blue">
- https://github.com/gitleaks/gitleaks-action
- https://github.com/zricethezav/gitleaks

## :office: ãµã³ãã«å®è£ããã³çµæ
- :page_facing_up: ãµã³ãã«å®è£ãï¼[gitleaks_action.yml](/.github/workflows/gitleaks_action.yml)
- :memo: ãµã³ãã«èå¼±æ§ãï¼[dummy_code.md](/dummy_code.md)
- ð» åºåçµæï¼ä¾ï¼
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
- ð« ã¡ã¼ã«éç¥ï¼ä¾ï¼
<img width="393" alt="image" src="https://user-images.githubusercontent.com/2616832/175293586-763f17a1-402e-4fc9-8b77-f5fec04da12e.png">


## Task List
### ï¼inputï¼
- [x] ã­ã¼ã¯ã¼ããå¤æ°å
- [ ] åºå®ã¦ã¼ã¶ã¼ã®Publicãªãã¸ããªã®éåããåå¾
- [ ] ã¦ã¼ã¶ã¼éåããã®Publicãªãã¸ããªã®éåãåå¾

### ï¼processï¼
- [ ] ã«ã¼ãå¦ç
- [x] ãã§ãã¯ã¢ã¦ããæ¢å®ã¸ã§ãã§
- [ ] matrixä½¿ã£ãä¸¦åå¦çã§

### ï¼outputï¼
- [ ] ã¸ã§ãçµæã®OK/NGåæ¿
- [ ] ã¨ã©ã¼ãªã¹ããå±¥æ­´ã§é²è¦§å¯è½ã«ï¼ä»¶æ°ãã¦ã¼ã¶ã¼ããªãã¸ããªããã¡ã¤ã«ãã¹ãæ¤ç¥è¡ã³ã³ãã³ãï¼
- [ ] ç®¡çèéç¥ã§çµææ¦è¦ãä¼ãã

## å¹æ
~~ãã¯ãæ¹åæ§ã¨ãã¦å¹æãèãï¼èª¤æ¤ç¥ãå¤ãï¼ã¨æãããã§ãä¸è¨ã¿ã¹ã¯ã¯ä¸æ¦æ¾ç½®ã
secret scanningãããµã¼ããã¼ãã£è£½åã®å©ç¨æ¤è¨ããã¦ãã ããã~~
gitleaksã§ã®ã¹ã­ã£ã³çµæã¯Actionsã§ç¢ºèªãã¦ã¿ã¦ãã ããã
ããç¨åº¦ã®ãã¿ã¼ã³ã¯æ¾ããå½¢ã«ãªã£ã¦ãããã¨ã
