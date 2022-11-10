# combineReducers

```
reducer를 기능에 따라 여러개의 파일을 만들 수 있다.
그러면 reducer들을 합쳐줘야 된다.
그때 사용하는 것이 combineReducers
reducer들을 객체 형태로 합쳐서 전달한다.
```

# 주의할점

```
원래는 useSelector로 id 값을 가져오고 싶으면 state.id로 가져왔음.
하지만 combineReducer를 사용하면 state.객체 안에 키 값.id로 불러와야 한다.
```
