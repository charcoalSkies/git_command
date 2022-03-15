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

D:\Code\github>git add Github.md   

폴더 내 모든 파일 stage 

D:\Code\github>git add -A
```

&nbsp;

> 현상태 저장

``` terminal
D:\Code\github>git commit -m "적어둘 내용"
[master (root-commit) cd1a539] Make Github.md
 1 file changed, 44 insertions(+)
 create mode 100644 Github.md

```