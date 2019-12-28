# Git

> Git은 분산버전관리시스템(DYCS)이다.
>
> 소스코드의 버전 및 이력을 관리할 수 있다.

## 준비하기

윈도우에서 git을 활용하기 위해서 [git_bash](https;//gitforwindows.org)를 설치한다.

git을 활용하기 위해서 GUI 툴인 `source tree`,`github`,`desktop` 등을 활용할 수도 있다.

초기 설치를 완료한 이후에 컴퓨터에 `author` 정보를 입력한다.

이메일 정보를 github에 가입된 이메일로 일치시켜야 커밋 이력들이 관리된다.

> $ git config --global user.name KYJ96
>
> $ git config --global user.email rnjsdydwns1110@gmail.com

## 로컬 저장소(repository) 활용하기

 ### 1. 저장소 초기화

```bash
$ git init
Initialized empty Git repository in C:/Users/kik54/Desktop/TIL/.git/
```

* `.git` 폴더가 생성되며, 여기에 git과 관련된 모든 정보가 저장된다.
* git bash에 `(master)` 라고 표현되는데, 이는 `master` 브랜치에 있다는 뜻이다.

### 2. add

`working directory`, 즉 작업 공간에서 변경된 사항을 이력으로 저장하기 위해서는 반드시 `staging area` 를 거쳐야한다.

```bash
$ git add markdown .md #특정 파일
$ git add images/ #특정 폴더
$ git add .# 현재 디렉토리
```



* `add` 전 상태

  ```bash
  $ git status
  On branch master
  
  No commits yet
  
  #트래킹 되고 있지 않는 파일들
  # -> commit 이력에 한번도 담기지 않은 파일들
  Untracked files:
  # 커밋될 것들에 포함시키려면 add 명령어를 사용해
    (use "git add <file>..." to include in what will be committed)
          git.md
          images/
          markdown.md
  # 아직 커밋될 것들은 없지만,
  # untracked files은 존재한다
  nothing to commit (create/copy files and use "git add" to track)
  
  ```

* add 후 상태

  ```bash
  $ git status
  On branch master
  
  No commits yet
  # 커밋될 변화들
  # => staging area에 있는 파일들
  Changes to be committed:
    (use "git rm --cached <file>..." to unstage)
          new file:   "images/\354\240\234\353\252\251 \354\227\206\354\235\214.png"
  
  Untracked files:
    (use "git add <file>..." to include in what will be committed)
          git.md
          markdown.md
  ```

  

### 3. commit

commit은 이력을 확정짓는 명령어로, 해당 시점의 스냅샷을 기록한다.

커밋시에는 반드시 메시지를 작성해야하며, 메시지는 변경사항을 알 수 있도록 명확하게 작성한다.

```bash

```





