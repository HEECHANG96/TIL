## Javascript 불편한점
1. document.getElementById("");
2. Javascript와 HTML 파일이 따로놈 => 관리가 힘들다.
3. 새 페이지 들어갈때마다 새로고침이 된다.

## React의 특징
1. document.getElementById(""); 쓰지 않기
2. JSX를 사용해 관련있는 HTML과 JS 합쳐준다.
3. 새로운 페이지, 메뉴 들어갈때 새로고침이 안 된다.
4. 코드의 재활용성이 높아짐

## React : 자바스크립트의 UI 라이브러리
* React의 파생 기술 React Native를 이용하여 Desktop, Android, iOS에서 동작하는 어플리케이션을 개발할 수 있다.
1. React는 Component 기반의 UI 라이브러리.
2. 선언형 프로그래밍 : 그냥 목적을 바로 말한다.
3. Virtual DOM : 5번 업데이트 해야될 것을 한 번에 5개를 업데이트 한다.

## State
* 계속해서 변화하는 특정 상태.
* 상태에 따라 각각 다른 동작을 한다.

## <React.StrictMode>
* React App을 개발하는 도중 발생할 수 있는 잠재적인 문제를 확인하기 위한 설정

## ...
* input창에 onChange이벤트를 등록하면 input 값이 바뀔때마다 콜백함수를 작동시킬 수 있다.
* 렌더링 : 화면에 표시해준다.
* React는 단방향으로만 데이터가 흐른다.
* SPA : Single Page Application : 웹사이트에 페이지가 딱 하나다!
* index.js의 역할 : index.html 파일과 App.js를 연결해준다.
