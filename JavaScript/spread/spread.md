# spread

```
let person = {name:"hee", age:27}

let person2 = {...person};
let person3 = person;

console.log(person2); // { name: 'hee', age: 27 }
console.log(person3); // { name: 'hee', age: 27 }

console.log(person == person2); // false
console.log(person == person3); // true

```

## person2와 person3의 차이

spread를 사용한 person2는 실제로 객체를 하나 더 생성하는 것.
person3는 객체의 주소값만 복사 => 즉 객체는 하나이고 그 객체를 참조하는 변수가 두개
