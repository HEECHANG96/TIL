# Lifecycle Function

상태에 따라서 실행이 가능한 함수

```
state가 업데이트 된 후에 해야하는 작업들은 모두 componentDidUpdate()에 넣는다. 
=> API 호출 작업들 
=> 그 이유는? 
=> render 끝나고 바로 호출되는 함수니까
```

## Function Component에서 사용 가능한 Lifecycle Function

* useEffect(함수) : 상황에 따라 다양한 역할을 한다.
```
매개변수 2개 받는다 => 콜백함수, 배열
기본적으로 앱 실행 후 첫번째 렌더 후에 한번 실행이 된다. => 주로 화면에 처음 보여줘야하는 데이터들에 대한 API 호출
배열에 state가 들어있으면 state 값이 바뀔때마다 호출되는 componentDidUpdate 역할을 한다.
배열에 여러개의 state가 들어있으면 state 중 하나라도 업데이트가 되면 해당 useEffect가 호출이 된다. => 여러개의 state가 동시에 업데이트 되면 한번만 호출된다.
```
