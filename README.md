# Handbook for github

## Contents

1. [Github에 잘못 올라간 파일 삭제 과정](#Github에-잘못-올라간-파일-삭제-과정)
1. [git add 취소하기](#git-add-취소하기)
1. [git commit 취소하기](#git-commit-취소하기)
1. [fond style](#fond-style)

## ICON link
[github-emoji][github-emoji]참고


## Github에 잘못 올라간 파일 삭제 과정

1. remove file from remote repository
이미 github remote에 push를 했기 때문에 로컬의 저장소에서 파일을 삭제해도 원격 저장소에서는 삭제되지 않음

```bash
# remote repository와 local에 있는 파일을 삭제
$ git rm [File Name]
$ git rm --cached [File Name]
```

2. commit 명령어와 push 를 수행
```bash
$ git commit -m "Fixed untracked files"
# remote repository에 push
$ git push origin master
```

## git add 취소하기
`git reset HEAD [file]`

```bash
git reset HEAD [file]
```
* 뒤에 파일명이 없으면 add한 파일 전체를 취소

## git commit 취소하기

```bash
$git reset HEAD^
```

## font style
span tag를 이용하여 style 지정  
\<span style="color:red">"text"</span>





[github-emoji]: https://gist.github.com/rxaviers/7360908