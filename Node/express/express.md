# express

node.js기반의 웹 프레임워크이다.

## express의 역할

웹 프레임워크를 만들고 사용하는 것이다.

## 웹 프레임워크의 역할

요청에 따라 응답해주는 역할을 한다.

## express 서버를 띄우기 위한 기본셋팅

```
const express = require('express');
const app = express();

// 서버 띄울 포트번호, 띄운 후 실행할 코드
app.listen(3000, function() {
    console.log("listening on 3000");
});
```
