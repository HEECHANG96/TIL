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

## fetch()
* API를 호출해주는 함수
