## Javascript 불편한점
1. document.getElementById("");
2. Javascript와 HTML 파일이 따로놈 => 관리가 힘들다.
3. 새 페이지 들어갈때마다 새로고침이 된다.


## React의 특징
1. document.getElementById(""); 쓰지 않기
2. JSX를 사용해 관련있는 HTML과 JS 합쳐준다.
3. 새로운 페이지, 메뉴 들어갈때 새로고침이 안 된다.
4. 코드의 재활용성이 높아짐
 * JSX는 반드시 하나의 덩어리를 리턴해야 한다!! => 하나의 태그로 감싸줘야 함.


## React : 자바스크립트의 UI 라이브러리
* React의 파생 기술 React Native를 이용하여 Desktop, Android, iOS에서 동작하는 어플리케이션을 개발할 수 있다.
1. React는 Component 기반의 UI 라이브러리.
2. 선언형 프로그래밍 : 그냥 목적을 바로 말한다.
3. Virtual DOM : 5번 업데이트 해야될 것을 한 번에 5개를 업데이트 한다.


## Component
1. 반복이 되는 부분 : 리스트의 아이템 또는 반복되는 UI요소는 Component로 만드는게 좋다.
2. 기능별로 나누어야 개발할때나 테스트, 유지보수할때 훨씬 더 용이하다.
3. 나중에 재활용될 경우를 대비해 한 Component에 한가지의 기능만 들어있는 것이 좋다.


## State
* UI를 바꾸고 싶다면 State를 만들자.
* 계속해서 변화하는 특정 상태.
* 상태에 따라 각각 다른 동작을 한다.
* set함수를 이용해 값을 업데이트 시킬 수 있다.
* state는 같은이름의 변수로 재할당 되는 것을 막기 위해 const 사용.
* 변수는 값을 바꾸면 바로 적용이 되지만 state 바꾸는 함수가 바로 실행되는게 아니라 함수가 끝날때까지 기다렸다가 state 바꾸는 함수들을 모아서 한번에 실행한다. => 비동기적으로 작동


## 조건부 렌더링
* 내가 원하는 UI를 조건과 일치하면 보여주는 것
* if-else : 조건을 주어 상황마다 다른 내용이 보이게 한다.
* 논리연산자 &&
* 삼항연산자


## 클래스 컴포넌트
1. 많은 개발 문서들이 클래스 컴포넌트로 작성이 됨.
2. 리액트에서 제공하는 유용한 함수 중에서 lifecycle function이 있는데, 클래스 컴포넌트에서만 동작했다.
3. 2019년부터는 function 컴포넌트에서도 lifecycle 함수가 제공됨. => function 컴포넌트를 사용할 것을 더 추천!!
* constructor (Lifecycle Function 중의 하나) => 생성자 : 컴포넌트가 실행되자마자 호출이 되는 함수


## Lifecycle Function : 상태에 따라서 실행이 가능한 함수
![lifecycle_function](https://user-images.githubusercontent.com/70733630/176342062-677722fe-b12d-4bd1-bc04-1dffd691e396.png)
* state가 업데이트 된 후에 해야하는 작업들은 모두 componentDidUpdate()에 넣는다. => API 호출 작업들 => 그 이유는? render 끝나고 바로 호출되는 함수니까
* 여기 나오는 Lifecycle Function들은 class component에서만 사용할 수 있다.
### Function Component에서 사용 가능한 Lifecycle Function
1. useEffect(함수) : 상황에 따라 다양한 역할을 한다. 
* 매개변수 2개 받는다 => 콜백함수, 배열
* 기본적으로 앱 실행 후 첫번째 렌더 후에 한번 실행이 된다. => 주로 화면에 처음 보여줘야하는 데이터들에 대한 API 호출
* 배열에 state가 들어있으면 state 값이 바뀔때마다 호출되는 componentDidUpdate 역할을 한다.
* 배열에 여러개의 state가 들어있으면 state 중 하나라도 업데이트가 되면 해당 useEffect가 호출이 된다. => 여러개의 state가 동시에 업데이트 되면 한번만 호출된다.

## ROUTE
* https://reactrouter.com
* 여러 웹페이지를 만들때 사용
### ROUTE끼리 쉽게 왔다갔다 하는 법
1. Link : 함수호출할 것없이 버튼 누르면 바로 가면 될때
2. useNavigate : 어떤 함수안에서 써야할때
### RESTful Routes
* url 디자인 패턴
* [RESTful Routes](https://velog.velcdn.com/images/yumjongeun/post/446f623b-efdd-460b-bd4b-6419af3b6136/image.webp)
### HTTP 명령어
1. GET : 데이터 가져올때
2. POST : 새로운 데이터 만들때
3. PUT : 기존 데이터 수정할때
4. DELETE : 데이터 삭제
### useParams : URL의 파라미터 값을 읽을 수 있다.
### useSearchParams : 쿼리값을 읽을 수 있다.
### 쿼리와 파라미터의 차이 : 쿼리는 URL의 경로에 영향을 미치지 않는다. => 파라미터가 달라지면 경로자체가 달라진다.
### 보호해줘야 하는 페이지 => Redirect
* Navigate 컴포넌트가 Redirect하게 도와준다. => useNavigate(react hook)와는 다르다.


## stateful, stateless
* stateful 컴포넌트 : 모든 state를 들고있는 컴포넌트
* stateless 컴포넌트 : state가 없고 props와 같이 받은 데이터만 보여주는 컴포넌트
* 리액트는 단방향 통신이다 => 부모에서 자식으로만 데이터를 전달할 수 있다.
* 데이터 흐름을 추적하기는 쉽지만, 같은 형제끼리 데이터를 주고받는 것이 힘들다.
* state를 들고있는 부모 컴포넌트는 stateful 컴포넌트, 부모가 주는 데이터만 받는 자식 컴포넌트를 stateless 컴포넌트라고 한다.
* 이렇게 컴포넌트를 구성하면 stateless 컴포넌트는 재사용이 쉽고 데이터를 걱정하지 않아도 된다.
* 모든 중요한 데이터들은 stateful 컴포넌트에 있기 때문에 유지보수가 쉽다.
* 최대한 모든 컴포넌트를 stateless로 만들고 몇개의 stateful 컴포넌트에서 데이터를 관리하는 구조가 이상적이라고 리액트는 말한다.


## Json Server
* npx json-server --watch db.json --port 포트번호
* my json server란? : Json Server를 localhost가 아닌 다른 사람들도 데이터를 볼 수 있게 연결해주는 사이트
* https://my-json-server.typicode.com/
* 바로 위의 url에다가 /<your-username>/<your-repo> 추가해서 기존의 localhost 포트번호의 url를 변경해주기


## Redux : 라이브러리
* state를 저장해두는 창고 = store  
* React의 단점인 단방향 통신을 보완해준다. => 언제든지 어디서든 store에 저장된 state를 가져다 쓸 수 있다.
* https://ko.redux.js.org/introduction/getting-started
* https://react-redux.js.org/introduction/getting-started
* Provider가 App을 감싸는 이유? : store을 제공하기 위해서  
* ![image](https://user-images.githubusercontent.com/70733630/175224743-bd1fd02e-701d-4f4d-a70b-4f9580c2ba03.png)  

  
## Redux의 단점
* 동기적 : 코드가 순차적으로 실행된다.
* 비동기 작업은 리덕스로 할 수 없다. => 이 문제를 해결하기 위해 Redux Middleware를 사용한다.


## Redux Middleware  
1. redux-saga
2. redux-thunk : 작은 서비스에 적용하기 쉽다.
  

## Redux Toolkit
* Redux 최신 문법 적용
* https://redux-toolkit.js.org
  
  
## <React.StrictMode>
* React App을 개발하는 도중 발생할 수 있는 잠재적인 문제를 확인하기 위한 설정


## Random 함수
* ![image](https://user-images.githubusercontent.com/70733630/172993573-92b0898e-f751-4c07-a933-5e308f615194.png)
* 헷갈리는 부분이 많으니, 한번씩 복습하기


## ...
* input창에 onChange이벤트를 등록하면 input 값이 바뀔때마다 콜백함수를 작동시킬 수 있다.
* 렌더링 : 화면에 표시해준다.
* React는 단방향으로만 데이터가 흐른다.
* SPA : Single Page Application : 웹사이트에 페이지가 딱 하나다!
* index.js의 역할 : index.html 파일과 App.js를 연결해준다.
* React에서는 문자열이 아닌 함수를 받아서 이벤트를 처리한다. => 함수를 콜백형태로 전달해주는 것이 중요하다. (= 함수를 전달하는 형식으로 넣어줘야 함)
* ![image](https://user-images.githubusercontent.com/70733630/172860964-c649d810-3cdf-4bf8-b760-de23663d7a94.png)
