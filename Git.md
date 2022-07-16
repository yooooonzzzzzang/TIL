# Today I Learned 

## 1. what's git and github?

깃은 분산 버전 관리 프로그램으로 백업, 복구, 협업을 위해 사용  
마지막 원본과 변경사항들만 저장함으로써 용량을 줄이는 snapshot 방식  

Git (분산버전관리프로그램) != Github(git기반의 저장소서비스)  

깃의 로컬저장소에는 3가지 공간이 나뉘어 있음  
working Directory - Staging area - .git directory
- `Working Directory (= Working Tree)` : 사용자의 일반적인 작업이 일어나는 곳
- `Staging Area (= Index)` : 커밋을 위한 파일 및 폴더가 추가되는 곳, 내가 원하는 파일들만 commit 할 수 있음
- `Repository` : staging area에 있던 파일 및 폴더의 변경사항(커밋)을 저장하는 곳
- Git은 **Working Directory → Staging Area → Repository** 의 과정으로 버전 관리를 수행함

## git 명령어 & 처음실행할때 
<span style='background-color: #f1f8ff'>작성자 이름, 메일 등록 (최초1번만 실행)</span>  
git config --global user.name "github username"
git config --global user.email "github email"  

<span style='background-color: #f1f8ff'>config 정보출력</span>  
git config --global --list

<span style='background-color: #f1f8ff'>일반 폴더 -> 로컬저장소</span>  
git init  

<span style='background-color: #f1f8ff'>버전 상태 출력</span>  
git status

<span style='background-color: #f1f8ff'> Working Directory -> Staging Area</span>   
git add File
git add .   (모든 파일 add)  

<span style='background-color: #f1f8ff'>Staging Area -> Commits</span>  
git commit -m "commit message"  

<span style='background-color: #f1f8ff'>commits 목록 출력</span>  
git log
git log --oneline  ( 한줄로 보기 옵션)


