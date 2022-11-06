# destructuring

객체를 분해해서 값을 가져옴(배열에서도 가능) => 값을 가져올 때 많이 사용한다.


```
// let name = person.name;
// let age = person['age'];

let {name, age} =person;

let array = [1,2,3,4];
let [a, b] = array;

console.log(a, b); // 1 2
```
