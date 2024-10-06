# CLI 강의 노트

---

## 1. I/O 리다이렉션: 표준 출력
- `>` : 출력을 파일로 저장.
  - 예: `ls > output.txt`  
- `>>` : 출력 추가. 파일 없으면 생성.
  - 예: `echo "Hello" >> output.txt`



## 2. I/O 리다이렉션: 표준 입력
- `<` : 파일에서 입력 받음.
  - 예: `cat < input.txt`
- `<`와 `>` 같이 사용.
  - 예: `cat < input.txt > output.txt`



## 3. 파이프라인 (`|`)
- `|` : 앞 명령어 출력 -> 다음 명령어 입력.
  - 예: `cat file.txt | grep "search_term"`



## 4. 확장 (Expansion)
- 특수 문자 확장됨.
  - 예: `echo *` → 디렉토리 모든 파일 이름 출력.



## 5. 백슬래시 (`\`)
- 명령어 여러 줄로 나눌 때 사용.
  - 예: `echo this is a long command \`  
    `that spans multiple lines`.



## 6. 권한 (Permissions)
- `chmod` : 파일 권한 변경.
  - 예: `chmod 600 file.txt`
  
- 권한 값:
  - **6**: 읽기(`r`), 쓰기(`w`).
  - **0**: 권한 없음.



## 7. 수퍼유저 (Superuser)
- `sudo` : 수퍼유저 권한 필요.
  - 예: `sudo apt-get update`
  
- `exit` : 수퍼유저 모드 종료.



## 8. 텍스트 에디터 (Text Editors)
- CLI: `nano`, `vim`  
- GUI: `gedit`



## 9. 셸 스크립트 (Shell Script)
- 스크립트 작성 및 실행.
  - 파일 생성: `nano script.sh`
  - 실행 권한 부여: `chmod +x script.sh`
  - 실행: `./script.sh`



## 10. 명령어 기록 (History)
- `history` : 사용한 명령어 목록 출력.
  - 예: `history`



## 11. `wget`
- 파일 다운로드.
  - 예: `wget https://example.com/file.txt`



## 12. `curl`
- 데이터 가져오기/업로드.
  - 예: `curl -O https://example.com/file.txt`



## 13. `grep`
- 파일 내 텍스트 검색.
  - 예: `grep "search_term" file.txt`

### 옵션:
- `-i` : 대소문자 구분 안 함.
- `-v` : 검색어 포함되지 않은 줄 출력.
- `-n` : 줄 번호 같이 출력.
- `-r` : 디렉토리 내 모든 파일 검색.
- `-l` : 검색어 포함된 파일 이름만 출력.

### 정규 표현식:
- `.*` : 모든 문자 0회 이상 반복.
- `\d` : 숫자.
- `[abc]` : 괄호 안 문자 중 하나.
- `^` : 줄 시작.
- `$` : 줄 끝.
