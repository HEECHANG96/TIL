## Git
* Version Control System : 프로그램의 버전관리를 위한 툴
* CLI (Command Line Interface) : 명령줄을 입력해서 사용
* GUI (Graphical User Interface) : 일반사용자가 쓰기 편하도록 그래픽 요소를 활용한 인터페이스 => Source Tree 사용


## add와 commit 한꺼번에
* git commit -am "메시지"
* 단, 새로 추가된 파일(untracked)이 없을 때 한정


## Branch
* 프로젝트를 하나 이상의 모습으로 관리할 때
* 여러 작업들이 독립되어 진행될 때


## Merge vs Rebase
* branch의 사용 내역들을 남겨둘 필요가 있다면 Merge
* 히스토리를 깔끔하게 만드는게 중요하다면 Rebase


## Github
* Git으로 관리되는 프로젝트의 원격 저장소


## GitHub에서 프로젝트 다운받는 방법
* Download ZIP : 파일들만 다운받음 => Git 관리내역 제외됨
* Gitt clone : Git 관리내역 포함 다운로드함
* 터미널이나 Git Bash에서 대상 폴더 이동 후 git clone (원격 저장소 주소) 입력한다.


## push, pull
* push : 원격으로 커밋 밀어올리기
* push를 하기 위해서는 나의 내역이 원격저장소의 최신내역대로 맞춰져 있어야 한다.
* pull : 원격의 커밋 당겨오기 (다른 동료가 작업한 것들)\
* git pull --no-rebase : 로컬과 원격의 어긋난 시간선을 한군데로 모아준 다음에 push를 진행한다.
* git pull --rebase : 원격에 맞춰서 일단은 원격 커밋을 붙인 다음에 로컬에서 한 커밋을 붙여준다.
* git push --force : 로컬의 내역 강제 push

## non-fast-forward 에러 해결하기
* git push origin master --force : 과거 커밋내역과 상관없이 지금 현재 커밋내용으로 덮어씌운다. => 이 명령어를 통해 에러 해결
