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

> 폴더 내 변화 캡슐에 담기(stage)

``` terminal
D:\Code\github>git add Github.md

또는 


```