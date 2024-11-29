# GIT CLI


## 기본설정
``` 
git config --global user.name "tester"
git config --global user.email "tester@gmail.com"
```

## config 확인
```
git config --list
```
```
$ git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/etc/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.helper=manager
credential.https://dev.azure.com.usehttppath=true
init.defaultbranch=master
user.name=KIM-YONG-HA
user.email=vb901217@gmail.com
difftool.sourcetree.cmd=''
mergetool.sourcetree.cmd=''
mergetool.sourcetree.trustexitcode=true
core.autocrlf=true
core.repositoryformatversion=0
core.filemode=false
core.bare=false
core.logallrefupdates=true
core.symlinks=false
core.ignorecase=true
remote.origin.url=https://github.com/KIM-YONG-HA/OrgolScore.git
remote.origin.fetch=+refs/heads/*:refs/remotes/origin/*

```




## github cli 로그인

gh auth login



// 원격 레포지토리 생성
```
gh repo create <repository-name> --public -- description "desc"
gh repo create <repository-name> --private -- description "desc"

gh repo create GitStudy --visibility private --description "GitStudy"

```



rmdir --ignore-fail-on-non-empty GitStudy
rm -rf GitStudy 

//

git init

echo "# GitStudy" > README.md

git add README.md



$ git add README.md
warning: in the working copy of 'README.md', LF will be replaced by CRLF the next time Git touches it


git config --global core.autocrlf true


git commit -m "Initial commit"




$ git push origin main
error: src refspec main does not match any
error: failed to push some refs to 'origin'


git checkout -b main

생성과 동시에 체크아웃 


Switched to a new branch 'main'

kj@DESKTOP-2DK9R40 MINGW64 ~/Desktop/myGit/OrgolScore (main)
$ git push origin main
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.



// 원격 레포 클론
gh repo clone <username>/<repo-name>


```

…or create a new repository on the command line
echo "# OrgolScore" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/KIM-YONG-HA/OrgolScore.git
git push -u origin main


…or push an existing repository from the command line


git remote add origin https://github.com/KIM-YONG-HA/OrgolScore.git
git branch -M main
git push -u origin main

```



--------------------



## 원격 레포지토리 추가

## 원격 레포지토리명 변경

## 원격 레포지토리 삭제  











# 이클립스 깃연동


## 로컬 레포지토리가 이미 있는 경우

new - import - projects from git - existing local repository - add 

- 디렉토리 선택 후 add - 추가된 디렉토리 클릭 후 next 

- import existing eclipse projects



## 이클립스 프로젝트가 이미 있는 경우

프로젝트 우클릭 - team - share project






git config --global --unset user.name
git config --global --unset user.email


