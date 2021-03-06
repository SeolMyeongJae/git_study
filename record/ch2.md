# ch2. 깃으로 버전 관리하기

깃에서는 문서를 수정할 때마다 간단한 메모와 함께 수정 내용을 스냅샷으로 찍어서 저장하는데 이를 `버전`이라고 한다.

깃에서 가장 기본이자 중요한 기능이 이렇게 만든 버전들을 관리하는 것이다. 

## 1. 깃 저장소 만들기

깃을 사용하기 위해 먼저 사용자 컴퓨터에 저장소를 만들어야한다. 

저장소를 만들고 싶은 디렉터리로 이동해서 깃을 초기화하면 그때부터 해당 디렉터리에 있는 파일들을 버전 관리할 수 있다.

해당 디렉터리에 저장소를 만들기 위해 `git init` 명령을 입력한다.

git init 명령을 실행하고 나면 `.git`이라는 디렉터리가 생성된다.

이 디렉터리가 깃을 사용하면서 버전이 저장될 저장소이다.

## 2. 버전 만들기

프로그램이나 앱을 설치하다 보면 버전이라는 말을 자주 접하게 된다.

프로그램을 개발하면서 수정 내용이 쌓이면 새로 번호를 붙여 이전 상태와 구별하는데 이런 번호 등을 통해 구별된 것을 버전이라고 부른다.

깃에서 버전이란 문서를 수정하고 저장할 때마다 생기는 것이라고 생각하면 쉽다.

깃에서 버전을 관리하면 원래 파일 이름은 그대로 유지하면서 파일에서 무엇을 변경했는지를 변경 시점마다 저장할 수 있고 각 버전마다 작업한 내용을 확인할 수 있고, 그 버전으로 되돌아갈 수도 있다.

### 스테이지와 커밋 이해하기

***작업트리***
git init 을 통해 깃을 초기화한 디렉터리를 작업 트리(작업 디렉터리)라고 한다. 작업 트리는 파일 수정, 저장 등의 작업을 하는 눈에 보이는 디렉터리이다.

***스테이지***
스테이지는 버전으로 만들 파일이 대기하는 곳이다. 
