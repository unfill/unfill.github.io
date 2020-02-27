---

layout: post

title: "Pro Git 공부 정리"
expert: "Pro Git 간단히 정리하기"

categories:
   -Git

tags:
   -Git
   -Github

date: 2020-02-27 11:18

---

#Git 최초설정

###설정파일

/etc/gitconfig   
모든사용자와 모든 저장소에 적용되는설정.  
git config --system 옵션으로 설정가능.  

~/.gitconfig, ~/.config/git/config   
특정사용자에 적용되는 설정.  
git config --global 옵션   

.git/config  
특정저장소(현재 작업 프로젝트)에만 적용.  

우선순위는 거꾸로  

###사용자정보   

$ git config --global user.name "John Doe"   
$ git config --global user.email johndoe@example.com   
--global옵션은 한번만.  
프로젝트마다 다른이름 필요시 --global빼고   

###편집기  

$ git config --global core.editor vim  

###설정확인

$ git config --list  

