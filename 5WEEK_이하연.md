CLI 강의 노트

1. I/O 리다이렉션: 표준 출력
- `>` : 출력 파일로 저장 (예: `ls > output.txt`)
- `>>` : 출력 추가 또는 새 파일 생성 (예: `echo "Hello" >> output.txt`)

2. I/O 리다이렉션: 표준 입력
- `<` : 파일에서 입력 (예: `cat < input.txt`)
- `<`와 `>` 같이 사용 (예: `cat < input.txt > output.txt`)

3. 파이프라인 (`|`)
- `|` : 앞 출력 -> 다음 명령어 입력 (예: `cat file.txt | grep "search_term"`)

4. 확장 (Expansion)
- 특수 문자 확장 (예: `echo *` → 모든 파일 출력)

5. 백슬래시 (`\`)
- 긴 명령어 나눔 (예: `echo this is a long command \` 다음 줄에 `that spans multiple lines`)

6. 권한 (Permissions)
- `chmod` : 파일 권한 변경 (예: `chmod 600 file.txt`)
  - **6**: 읽기/쓰기, **0**: 권한 없음

7. 수퍼유저 (Superuser)
- `sudo` : 수퍼유저 권한 (예: `sudo apt-get update`)
- `exit` : 수퍼유저 종료

8. 텍스트 에디터
- CLI: `nano`, `vim` / GUI: `gedit`

9. 셸 스크립트
- 스크립트 생성: `nano script.sh`
- 권한 부여: `chmod +x script.sh`
- 실행: `./script.sh`

10. 명령어 기록
- `history` : 명령어 기록 확인 (예: `history`)

11. `wget`
- 파일 다운로드 (예: `wget https://example.com/file.txt`)

12. `curl`
- 데이터 가져오기/업로드 (예: `curl -O https://example.com/file.txt`)

13. `grep`
- 파일 내 텍스트 검색 (예: `grep "search_term" file.txt`)

옵션:
- `-i` : 대소문자 구분 안 함
- `-v` : 검색어 제외한 줄
- `-n` : 줄 번호 표시
- `-r` : 디렉토리 내 모든 파일 검색
- `-l` : 검색어 포함된 파일 이름만

정규 표현식:
- `.*` : 모든 문자 0회 이상
- `\d` : 숫자
- `[abc]` : 괄호 안 문자
- `^` : 줄 시작
- `$` : 줄 끝
