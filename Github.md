# Git 명령어 정리

> 사용자 정보 입력

``` terminal
git config -g user.name "사용자 계정"
git config -g user.email "메일 주소"
```

&nbsp;

> Git 저장소 생성

``` terminal
D:\Code\github>git init 
Initialized empty Git repository in D:/Code/github/.git/
```

&nbsp;

> 폴더 내 변화들과 캡슐 상태 확인

``` terminal
D:\Code\github>git status 
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Github.md

nothing added to commit but untracked files present (use "git add" to track)
```

&nbsp;

> 폴더 내 변화 캡슐에 담기(stage)

``` terminal
특정 파일만 stage

D:\Code\github>git add testfile.txt  

폴더 내 모든 파일 stage 

D:\Code\github>git add -A
```

&nbsp;

> 현상태 저장

``` terminal
D:\Code\github>git commit -m "적어둘 내용" 
[master d46daa3] make testfile.txt
 1 file changed, 1 insertion(+)
 create mode 100644 testfile.txt

D:\Code\github>git status
On branch master
nothing to commit, working tree clean

```

&nbsp;

> git 상태들 확인(일련번호 등)

``` terminal
D:\Code\github>git log
commit 1f9955750814a848e27f77de4879a7376a39eb08 (HEAD -> master)
Author: Backtrack404 <jun48470@gmail.com>
Date:   Tue Mar 15 22:12:35 2022 +0900

    add line2

commit d46daa32bba2d39a575f927c65a2cef61e0b80f3
Author: Backtrack404 <jun48470@gmail.com>
Date:   Tue Mar 15 22:10:16 2022 +0900

    make testfile.txt
```

&nbsp;

> 특정 시점으로 돌아가기 (복구 불가능)

``` terminal
D:\Code\github>git reset d46daa32bba2d39 --hard
HEAD is now at d46daa3 make testfile.txt

D:\Code\github>git log
commit d46daa32bba2d39a575f927c65a2cef61e0b80f3 (HEAD -> master)
Author: Backtrack404 <jun48470@gmail.com>
Date:   Tue Mar 15 22:10:16 2022 +0900

    make testfile.txt

```

&nbsp;

> 브랜치 만들기

``` terminal
D:\Code\github>git branch main

```

&nbsp;

> 생성된 브랜치 확인

``` terminal
D:\Code\github>git branch
  main
* master
```

&nbsp;

> 특정 브랜치로 이동

``` terminal
D:\Code\github>git checkout main
Switched to branch 'main'

D:\Code\github>git branch
* main
  master
```

&nbsp;

> 다른 브랜치의 변경사항 가져오기

``` terminal
D:\Code\github>git merge master
Already up to date.
```

&nbsp;

> 다른 브랜치의 변경사항 가져오기 (이력 깔끔히)

``` terminal

```