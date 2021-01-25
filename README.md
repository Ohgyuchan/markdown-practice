# markdown-practice

## 1.1. git과 github에 대하여
#### 1.1.1. git에 대하여
+ 로컬에서 관리되는 버전 관리 시스템 (VCS : Version Control System)
+ 소스코드 수정에 따른 버전을 관리해주는 시스템
        
#### 1.1.2. github에 대하여
+ git으로 관리되는 프로젝트를 공유할 수 있는 웹서비스
+ 자체 구축이 아닌 빌려쓰는 클라우드 개념
+ 오픈소스는 일정 부분 무료로 저장 가능, 아닐 경우 유료 사용
[https://github.com]
    
    
#### 1.1.3 git, github 차이점
+ git: 로컬에서 버전 관리 시스템을 운영하는 방식
+ github: Github는 깃허브에서 제공해주는 클라우드 서버를 이용하는 방식
            
## 1.2. git, github 사용법
#### 1.2.1. commit
##### 1.2.1.1 영역
+ Working Directory: 프로젝트를 진행하는 실제 작업 공간으로 개발한 소스 및 자원이 존재하며 이곳에서 파일을 수정 및 추가
+ Staging Area: 워킹 디렉터리에서 작업한 내역을 Git 디렉터리로 커밋 하기 위해 커밋 대상 목록으로 담아두는 장바구니 목록 같은 영역
+ Git Directory: 실제로는 .git 이라는 이름의 디렉터리이며, 여러가지 버전의 커밋 데이터들과 Git 프로젝트에 대한 모든 정보를 담고 있는 핵심 데이터베이스 디렉토리

##### 1.2.1.2 Untracked와 Tracked 상태
+ 워킹 디렉터리에 있는 여러가지 파일들은 Git의 추적 관리 여부에 따라 각각 크게 두 가지 상태로 나눌 수 있다.
+ Tracked: Git이 해당 파일을 추적 및 관리하는 상태
+ Untracked: 반대로 아직 Git이 해당 파일을 추적 및 관리하지 않는 상태

##### 1.2.1.3 Unmodified와 Modified 상태
+ Untracked와 Tracked가 추적 관리 여부 관점에서 바라본 상태 였다면, 파일의 변경 여부에 따라 **Modified(변경 발생)**과 **Unmodifed(변경 없음)** 상태로 나눌 수 있습니다.

##### 1.2.1.4 Staged 상태
+ Staged: Untracked 파일이나 Modified 상태인 파일을 Staging Area에 내역을 등록하지 않은 상태

##### 1.2.1.5
+ git add: __untracked__파일을 __tracked__로 상태로 바꿈

        git add [파일명]
+ git commit: Staging Area에 있는 Staged 파일에 대한 commit을 남김

        git commit // 자세한 커밋 vim 화면으로 넘어감
        git commit -m "message" //한 줄 메세지 커밋

#### 1.2.2. repository
+ Repository: 저장소
   - Local Repository: 로컬저장소
   - Git Repository: Git을 사용할 수 있는, Git으로 관리하는 저장소
   - 원격 Repository: 내 로컬PC에 있는 저장소가 아닌 네트워크상에 있는 저장소    
                
                git init //로컬저장소를 Git저장소로 변경 .git 폴더가 생성
                git remote add [링크] //원격저장소 연결
                
#### push pull fetch
+ git push: 현재 프로젝트의 커밋된(HEAD) 내용을 원격 저장소로 내보내는 명령어
+ git pull: 원격 저장소에서 로컬 저장소로 소스를 가져오는 명령어(merge)
+ git fetch: 원격 저장소에서 로컬 저장소로 소스를 가져오는 명령어(not merge)-conflict 방지

        git push [원격저장소명] [brach명]
        git pull [원격저장소명] [brach명] //자동 merge 시도
        git fetch [원격저장소명] [brach명] //merge하지 않음
![이미지](https://i.ytimg.com/vi/0nqJKEh3YCc/maxresdefault.jpg "pull push fetch")
#### 1.2.4. branch
#### 1.2.5. merge

## 1.3. Markdown

[참고사이트]
* [코끼리를 냉장고에 넣는방법::Git](https://dololak.tistory.com/304)
