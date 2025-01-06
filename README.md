
## Reference
- MarkDown Cheat Sheet - markdownguide.offshoot.io/cheat-sheet
- GIT Cheat Sheet - education.github.com/git-cheat-sheet-education.pdf


---------------------------------------------------
### HELP 사용법 (예시)
git help status  
git help add  
git help commit  

### git 저장소 초기화
git init
### git 워킹트리 상태 출력
git status

--------------------------------------------------

### 전역 옵션 내용 출력
git config --global <옵션명>

### 전역 옵션 내용 지정
git config --global <옵션명> <옵션값>

### 전역 옵션 내용 삭제
git config --global --unset

### 전체 프로젝트의 모든 옵션 리스트 출력
git config --list

---------------------------------------------------

### 파일 스테이지 출력
git add <파일명>

### 스테이지에 있는 파일들 커밋
git commit 

### 마지막 커밋 수정하기
git commit -m "<수정 할 메시지>"

### 현재 브랜치에서 새로 생성한 커밋들 원격저장소에 업로드
git push

---------------------------------------------------

### 원격 저장소의 브랜치와 커밋들을 로컬 저장소로 동기화
git fetch [원격 저장소 별명] [브랜치 이름]

### 현재(checkout) 브랜치에서 대상 브랜치를 끌어와서 병합
git merge <대상 브랜치>

### 원격 저장소의 변경 사항을 워킹트리에 반영 (pull = fetch + merge)
git pull

### 현재(checkout) 브랜치에서 대상 브랜치로 붙어라
git rebase <대상 브랜치>	

---------------------------------------------------

### 원격 저장소 등록
git remote add <원격 저장소 이름> <원격 저장소 주소>

### 원격 저장소 목록 출력
gir remote -v

---------------------------------------------------

### 간단한 커밋 해시와 제목만 출력
git log --oneline

### 모든 브랜치의 이력 출력
git log --oneline --graph --all --decorate	

### 내 브랜치의 최신 커밋을 5개만 보고 싶을 때
git log --oneline -n5

---------------------------------------------------

### 로컬저장소 브랜치 출력
git branch 	

### 원격저장소 포함 브랜치 출력
git branch -a

### 로컬저장소 브랜치 출력 및 마지막 커밋 확인
git branch -v

### 브랜치를 특정 커밋으로 옮길 때
git branch -f <브랜치 이름> <커밋 체크섬>	

### 브랜치 삭제
git branch -d <브랜치>

### 지정 브랜치로 변경
git swich <브랜치 이름>

---------------------------------------------------

### 2 커밋 이전 커밋으로 옮기기
git reset --hard HEAD~2 	

### 원격 저장소 커밋 로컬 저장소로 복사
git clone <저장소 주소> .
