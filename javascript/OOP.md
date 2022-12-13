> # TL;DR

객체의 집합으로 프로그램을 표현하려는 프로그래밍 패러다임으로 `작은 문제를 해결해 큰 문제를 쉽게 만드는 방법`이라고 할 수 있고 `캡슐화`, `상속`, `추상화`, `다향성`의 핵심요소를 가지고 있다.

> # OOP의 4가지 핵심요소

### 캡슐화

데이터(fields)와 기능(methods)을 하나의 단위로 묶고 필요한 인터페이스만 밖으로 보낸다.

### 상속

만드려고 하는 클래스에 기존의 클래스에 있는 데이터(fields)와 기능(methods)를 사용할 수 있게 한다.

### 추상화

복잡한 내부는 숨기고 필요한 기능만 제시한다.

### 다형성

하나의 데이터 또는 기능이 여러 타입에 대입되어 다양한 결과를 얻는다.

> # Javascript Example

ES6 이후에 추가된 문법인 `class`를 사용해서 틀(template)를 만들 수 있으며 `new 연산자`로 인스턴스를 생성할 수 있다.

```js
class Person {
  // constructor
  constructor(name, age) {
    // fields
    this.name = name;
    this.age = age;
  }

  // methods
  sayHello() {
    console.log(`${this.name}: Hello !`);
  }
}

const sung = new Person('성석민', 28);

console.log(sung.name); // 성석민
console.log(sung.age); // 28
console.log(sung.sayHello()); // 성석민: Hello !
```
