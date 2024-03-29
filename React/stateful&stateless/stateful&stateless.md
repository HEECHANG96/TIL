# stateful, stateless

```
stateful 컴포넌트 : 모든 state를 들고있는 컴포넌트
stateless 컴포넌트 : state가 없고 props와 같이 받은 데이터만 보여주는 컴포넌트
```

## REACT 특징

```
단방향 통신이다 => 부모에서 자식으로만 데이터를 전달할 수 있다.
데이터 흐름을 추적하기는 쉽지만, 같은 형제끼리 데이터를 주고받는 것이 힘들다.
```

## REACT 장점

```
state를 들고있는 부모 컴포넌트는 stateful 컴포넌트, 
부모가 주는 데이터만 받는 자식 컴포넌트를 stateless 컴포넌트라고 한다.
이렇게 컴포넌트를 구성하면 stateless 컴포넌트는 재사용이 쉽고 데이터를 걱정하지 않아도 된다.
모든 중요한 데이터들은 stateful 컴포넌트에 있기 때문에 유지보수가 쉽다.
최대한 모든 컴포넌트를 stateless로 만들고 몇개의 stateful 컴포넌트에서 데이터를 관리하는 구조가 이상적이라고 리액트는 말한다.
```
