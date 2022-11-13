# Redux-MiddleWare

Redux의 기능을 향상 및 추가시켜준다.

## Redux의 단점

```
코드가 순차적으로 실행된다.
비동기 작업은 Redux로 할 수 없다. ex) API 요청
```

## Redux로 비동기 처리를 할 순 없을까?

```
이 문제를 해결하기 위해서 Redux-MiddleWare 등장
Redux-MiddleWare는 함수를 리턴한다. 
매개변수로는 2개를 받는다. => dispatch, getState
```

## 종류

1. redux-saga
2. redux-thunk


- [redux-thunk](https://github.com/reduxjs/redux-thunk)
