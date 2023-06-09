# 2023-1-OC-Web-Study

## Fork란

**Fork** <br/>
(1) 타인의 프로젝트에 기여하기 위한 첫 시작<br/>
(2) 자신의 저장소로 타인의 프로젝트를 통째로 복사한 뒤, 자신의 로컬 저장소에 클론해서 수정을 해야함. <br/>
(3) Fork하는 방법 : 원하는 레포지터리에 들어가서 우상단의 Fork 버튼을 누르면 됨 <br/>

    ∴ 깃허브를 통해 통째로 복사하는 것 = Fork <br/>

![image](https://user-images.githubusercontent.com/110219986/228207810-0ba7b6dd-d3c8-4192-9832-830327e936cb.png)

## Pull Request란 <br/>

(1) git clone을 통해서 자신의 local repository에 repository를 다운받음 <br/>
(2) 보통 자신(수정자)의 이름으로 branch를 생성한 뒤, 수정사항들을 작성하고 이를 git push origin 만든branch이름 해서 보냄 <br/>
(3) github에서 pull request를 보냄 <br/>

## Merge <br/>

(1) Pull Request를 받은 원본 저장소 관리자는 코드 변경 내역을 확인하고 Merge 여부를 결정 <br/>
(2) Merge를 했다면, 이후 동기화 및 branch 삭제 <br/>

## master로 이동

git checkout master

## upstream 동기화

git pull [원본 저장소] [브랜치명]
git pull upstream master

## origin에 반영

git push origin master

## 로컬 브랜치 삭제

git branch -d develop

## 원격 브랜치 저장소도 삭제하고 싶은 경우

git push origin --delete [브랜치명]

## commit 메세지 작성법 (커밋 메세지 컨벤션)

feat : 새로운 기능과 관련된 것을 의미한다. <br/>
fix : 오류와 같은 것을 수정했을 때 사용한다. <br/>
test : test를 추가하거나 수정했을 때를 의미한다. <br/>
docs : 문서와 관련하여 수정한 부분이 있을 때 사용한다. <br/>
style : 코드의 변화와 관련없는 포맷이나 세미콜론을 놓친 것과 같은 부분들을 의미한다. <br/>
refactor : 코드의 리팩토링을 의미한다. <br/>
build : 빌드 관련 파일 수정에 대한 커밋 <br/>
chore : 패키지 매니저 설정 등 여러가지 production code와 무관한 부분 들을 의미한다. <br/>
