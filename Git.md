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
