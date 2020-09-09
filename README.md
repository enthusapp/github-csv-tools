# GitHub CSV Tools for me
Customized [GitHub CSV Tools](https://github.com/gavinr/github-csv-tools)

GitHub CSV Tools 의 csv 포멧은 issue 의 body 와 comment 가 가로열로 펼쳐져 pdf 로 바로 출력하기 어렵습니다.

issue 의 body 영역과 comment 를 포함하여 pdf 파일로 출력하기 쉽게 하기위해 GitHub CSV Tools 의 코드를 수정하여 사용합니다.

## Command
```sh
$ node index.js -o {username} -r {repository} -t {token} -c
```

## 후처리
MS Office 로 csv 파일를 읽으면 한글이 깨지는 현상이 있습니다.

구글 드라이브로 업로드 한뒤에 구글 스프레드시트로 파일을 Open 합니다.

엑셀 시트에서 원하는 형태로 가공(외곽선, 행고정, 페이지 번호 추가 등)을 한 뒤에 pdf 파일로 다운로드 합니다.
