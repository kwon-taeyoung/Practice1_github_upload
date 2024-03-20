--Korean
Github 연결을 위한 Project 예문
-OS : Window
-Terminal : PowerShell
-IDE : VS Code(Visual Studio Code)

Github는 버전관리를 위해 사용되며, 이는 대부분의 프로젝트에서 사용되고 있다.
Github에서는 개인 컴퓨터에서 원격 저장소를 통해 프로젝트를 유통시키고, 협업을 위한 버전관리를 제공해준다.
Github 연결을 위해 Git을 다운로드 할 필요가 있다.

1. Git다운로드 및 설치
http://gitforwindows.org
위 사이트에서 git을 다운로드 받을 수 있다.
맥OS를 사용하는 경우에는 같은 사이트에서 Mac OS용을 다운로드 받을 수 있다.
2. Git설치 확인
설치를 확인하는 방법은 cmd창(Window + R)을 열고 아래의 커맨드를 입력해준다.
git version
예상 되는 결과값 : git version 2.25.1.windows.1 
3. VS Code
왼쪽 메뉴바의 소스제어에서 리푀토리를 초기화시켜준다.
이를 통해 폴더 내부에 .git폴더가 생성되고, 이곳이 로컬 저장소가 된다.(숨긴항목이 때문에 체크해서 보이게 처리해야한다.)
4. Git설정
처음 시작하는 경우에는 git을 config하는 과정이 필요하다.
아래의 커맨드를 입력하여 계정에 대한 정보를 설정한다.
git config --global user.name "유저명"
git config --global user.email "유저이메일"
5. 새로운 파일 생성
VS Code의 문서관리에서 여러가지 파일들을 생성한다.
이때, 파일명 옆에 U가 붙어있는데, 이는 github에 업로드 되어있지 않은 상태를 의미한다.
6. 파일 스테이지에 올리기
파일명 옆 U가 있는 쪽에 마우스 커서를 이동하면, +버튼이 보이는데, 이것을 클릭하면, 파일이 스테이징 되면서 옆 글자가 U에서 A로 변경된다.
이것이 인덱스에 추가된 것으로 위의 커밋 버튼을 누르면 커밋이 된다.
※반드시 Commit을 할 때는 Commit메세지를 작성해야하고, 이를 작성하지 않으면 Commit이 되지 않을 수 있다.
7. 원격 저장소 연결하기
아래의 커맨드를 입력하여 Git리모트를 설정한다.
git remote add origin https://github.com/유저명/프로젝트명.git
8. Github로 Push하기
VS Code의 소스제어에서 ...아이콘을 눌러 Push를 누르면, github로 Push되는 것을 확인할 수 있다.
9. Github에서 확인하기
Github에서 Push된 것을 확인한다.
