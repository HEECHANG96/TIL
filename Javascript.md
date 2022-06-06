## 일반함수에는 있지만 화살표함수에는 없는게 하나 있다.
## 그것은 바로 this

## this 란? : 나 자신을 불러주는 객체
* 화살표함수는 스스로 this를 생성할 수 없다.
* this를 사용해야 되면 일반함수를 쓰자!!
* 화살표 함수는 정의 전에 호출할 수 없다! 순서가 매우 중요하다.

## 리펙토링이 필요한 코드는?
* 중복 코드
* 긴 함수

## 함수
* 호이스팅 : 함수 선언문 / 변수 선언을 실행되기 전에 해당 유효범위 또는 실행 컨텍스트 최상단으로 끌어올린다.
![image](https://user-images.githubusercontent.com/70733630/170868035-d54a0b81-ebb9-4977-971f-310fcba8f86e.png)
![image](https://user-images.githubusercontent.com/70733630/170868104-bb6492c2-419b-414e-8a8e-42ee7fdf33ff.png)

## 콜백함수
![image](https://user-images.githubusercontent.com/70733630/170868516-31edc9b4-3dcf-4859-a798-028495d91070.png)

## API  Application Programmingg Interface
* Header : 요청관련 정보
* Body : 요청내용
* API 부르는 방식은 대표적으로 ajax, axios, fetch가 있다.
1. fetch() : API를 호출해주는 함수
* API 문서 읽을 때 주의깊게 봐야하는 것들
1. API endpoint별 주는 데이터
2. API 인증방법 (API KEY, 토큰)
3. Query로 쓸 수 있는 인자들
4. API 응답 내용들 => 어떤 결과를 받아볼 수 있는지

## ...
* 클래스타입은 new라는 키워드를 이용해 객체 생성
* let url = new URL(``); => URL()의 기능 : 주소를 분석해준다.
* ![image](https://user-images.githubusercontent.com/70733630/172049962-ccb335c1-1756-4e83-a06c-7d8e3da73f5d.png)
