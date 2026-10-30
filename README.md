# 김민기 포트폴리오

<https://laekhole.github.io/>에서 볼 수 있습니다.

한 페이지짜리 정적 사이트입니다(`index.html`, `style.css`, `assets/`). 원고는 비공개 저장소에서 관리합니다.

## PDF

첫 화면의 'PDF 다운로드'는 `assets/kim-mingi-portfolio.pdf`를 내려받습니다. 이 파일은 `style.css`의 인쇄용 스타일(A4, 쪽 번호)로 만듭니다. 내용을 고치면 저장소 폴더의 PowerShell에서 다시 만들어 함께 커밋합니다.

```powershell
Start-Process -Wait "C:\Program Files\Google\Chrome\Application\chrome.exe" -ArgumentList '--headless=new', '--no-pdf-header-footer', "--print-to-pdf=`"$PWD\assets\kim-mingi-portfolio.pdf`"", "`"$PWD\index.html`""
```
