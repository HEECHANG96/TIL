# POST

## POST 요청으로 서버에 데이터를 전송할 때

```
1. body-parser 필요
2. form 데이터의 경우 input에 name=""을 쓰기
3. 요청.body : 요청했던 form에 적힌 데이터 수신 가능하다.
```

## form 데이터의 경우 input에 name을 쓰는 이유?

서버에서 input을 구분하기 위해서 name을 사용한다.
