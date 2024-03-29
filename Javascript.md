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

## spread
![image](https://user-images.githubusercontent.com/70733630/175796052-1141d71d-4834-4973-99f2-3f5bfc60a411.png)
![image](https://user-images.githubusercontent.com/70733630/175796060-b998bef3-8a88-4f43-bfa3-4ce47a7b2d77.png)
* person3 : 객체의 주소값만 복사 => 객체는 하나이고 그 객체를 참조하는 변수가 두개 (person과 person3가 같은 객체를 바라보고 있는 것)
* person2 : 객체를 하나 더 생성함
* console.log(person == person2) => 결과는 false
* console.log(person == person3) => 결과는 true


## ...
* 클래스타입은 new라는 키워드를 이용해 객체 생성
* let url = new URL(``); => URL()의 기능 : 주소를 분석해준다.
* ![image](https://user-images.githubusercontent.com/70733630/172049962-ccb335c1-1756-4e83-a06c-7d8e3da73f5d.png)

## 배열 함수 : 매개변수로 함수를 받음
1. forEach() : for문 역할
2. map() : return을 해줘야 한다.
※ forEach는 반환값이 없다
※ map은 반드시 배열을 반환한다.
3. filter() : 조건을 넣고, 조건에 대해 참인 것만 반환함. 결과값 : 배열
4. some() : 조건에 만족하는 게 말 그대로 몇개가 있으면 true 반환
5. every() : 모든 값이 조건에 만족하면 true 반환
6. find() : string타입으로 첫번째로 찾은 한 개의 값만 반환
7. findIndex() : 인덱스번호를 찾아줌


## 대문자, 소문자 찾기
1. 대문자 : toUpperCase()
2. 소문자 : toLowerCase()

## 아스키코드 넘버
1. 대문자 아스키넘버 : 65 ~ 90
2. 소문자 아스키넘버 : 97 ~ 122
