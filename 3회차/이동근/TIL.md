# 오늘 배운 것

아라보자



## pull, clone 의 차이점

* 가장 큰 차이는 pull 은 변경된 커밋을 받아오고, clone 은 저장소를 받아온다.

* 명령어

  | git clone           | git pull                                                     |
  | ------------------- | ------------------------------------------------------------ |
  | git clone {{ URL }} | git init + git remote add origin {{ URL }} + git pull origin master |

* 정리

  * ```$ git clone ```  : 리모트 설정을 자동으로 해주므로, **초기 다운로드**에 사용한다.
  * ```$ git pull``` : 리모트 설정이 이미 되어있고, **커밋을 가져와서 병합할 때** 사용한다.  



## 또 한번 간단하게 정리하는 처음부터 원격 저장소까지 흐름

```bash
# 로컬
$ git init
$ git add .  
$ git commit -m "커밋 메세지"
$ git status 
$ git log

# 원격
$ git remote add origin {{ URL }}
$ git push origin master
$ git pull origin master
$ git clone {{ URL }}
```



## branch

```bash
# 브랜치

$ git branch # 목록 조회
$ git branch <branchname> # 브랜치 만들기
$ git checkout <branchname> # 브랜치 이동하기
$ git checkout -b <branchname> # 브랜치 생성 및 이동하기
$ git branch -d <branchname> # 브랜치 삭제하기

# 브랜치 병합

$ git merge <commit> # 지정한 커밋 내용이 'HEAD'가 가리키고 있는 브랜치에 넣어짐
$ 
```



## 참조링크

1. [git pull, clone 차이1](https://balsamic-egg.tistory.com/11)
2. [git pull, clone 차이2](https://meaownworld.tistory.com/157)
3. [git pull, clone 차이3](https://mminky.tistory.com/39)
