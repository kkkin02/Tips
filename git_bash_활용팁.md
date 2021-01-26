### 명령어

`cd ..`

: 상위 폴더로 이동



`clear`

: 다 지우기



`touch`

: 파일 만들기



`ls`

: 폴더에 들어있는거 표시



`ls -a`

:숨겨진 파일까지 다 표시



`mkdir`

: 폴더 만들기



`.`

: 현재 폴더(하위 폴더 모두 포함)



`..`

: 상위 폴더



`~`

: 홈 - 기본으로 가고 싶은 경로



`/`

: 루트 - 최상위 경로





### git과 연결



`git init`

: 비어있는 git 생성

(git이 있는 폴더에 **master** 표시)

* README.md 생성
* .gitignore 생성



`git comit -m "   "`

: commit에 담는 메세지 (변경사항 등)



`git status`

: 현재 상황 표현



`git log`

: 커밋된 git들의 로그



`git add  .`

: 현재 폴더에 있는 모든 파일을 스테이징

(새로 생긴거, 수정된거)



`git diff`

: 이전에 있던 최근 커밋들의 기록과 현재 상황을 비교, 차이를 알려줌



<u>처음 gitlab에 폴더를 연결하려면</u>

사이트에서 일단 프로젝트(repository) 생성하고

: `git remote ~~~ 복사에서 터미널에 붙여넣기`



`git push origin master`

: master 폴더에 있는 자료들을 github에 업로드



git에 있는 것을 pc 다운로드 받기

:저장하고 싶은 위치에서 git bash here

`git clone (git에서 clone 누르고 복사한 주소 붙여넣기) `



gitlab에 있는 프로젝트를 최신화하기

:` git pull origin master`



이미 git과 연결되어 관리되고 있는 파일을 지우고 싶을 때

: 그 파일을 지우고 add commit 한 다음 다시 파일 생성



### 처음 폴더 연결할 때

```
강인영@DESKTOP-F0IT69T MINGW64 ~/TIL
$ mkdir git

강인영@DESKTOP-F0IT69T MINGW64 ~/TIL
$ git init
Initialized empty Git repository in C:/Users/ksy21/TIL/.git/

강인영@DESKTOP-F0IT69T MINGW64 ~/TIL (master)
$ git add .

강인영@DESKTOP-F0IT69T MINGW64 ~/TIL (master)
$ git commit -m "start TIL!"
[master (root-commit) 9b86cac] start TIL!
 2 files changed, 390 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 README.md

강인영@DESKTOP-F0IT69T MINGW64 ~/TIL (master)
$ git remote add origin https://github.com/kkkin02/TIL.git

강인영@DESKTOP-F0IT69T MINGW64 ~/TIL (master)
$ git push origin master
```





