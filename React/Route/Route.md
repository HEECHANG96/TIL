# Route

여러 웹페이지를 만들때 사용

https://reactrouter.com

## ROUTE끼리 쉽게 왔다갔다 하는 법

```
Link : 함수호출할 것없이 버튼 누르면 바로 가면 될때
useNavigate : 어떤 함수안에서 써야할때
```

## RESTful Routes

url 디자인 패턴

## HTTP 명령어

```
GET : 데이터 가져올때
POST : 새로운 데이터 만들때
PUT : 기존 데이터 수정할때
DELETE : 데이터 삭제
```

## useParams

URL의 파라미터 값을 읽을 수 있다.

## useSearchParams

쿼리값을 읽을 수 있다.

## 쿼리와 파라미터의 차이 

쿼리는 URL의 경로에 영향을 미치지 않는다. => 파라미터가 달라지면 경로자체가 달라진다.

## 보호해줘야 하는 페이지 => Redirect

Navigate 컴포넌트가 Redirect하게 도와준다. => useNavigate(react hook)와는 다르다.
