# Redux

오픈 소스 자바스크립트 라이브러리

state 저장소

## React 불편한점

```
자식 컴포넌트끼리 state 공유를 못한다.
그러므로 props를 많이 사용하게 된다.
이 단점을 해결하기 위해서 Redux 등장!

※ React의 단점인 단방향 통신을 보완해준다. => 언제든지 어디서든 store에 저장된 state를 가져다 쓸 수 있다.
```

## useDispatch, useSelector

```
useDispatch : action을 던지는 리액트 훅
useSelector : store에 있는 값을 가져다 쓸 때 사용하는 리액트 훅
```

## Provider가 App을 감싸는 이유?

store을 제공하기 위해서


- [redux](https://ko.redux.js.org/introduction/getting-started/)
- [react-redux](https://react-redux.js.org/)
