# 웹접근성

## 자바스크립트에서 데이터의 종류
<details>
<summary>자세히 보기</summary>
<pre>
크게 원시형(기본형)과 참조형으로 구분할 수 있습니다.
원시형 : number, string, boolean, null, undefined, Symbol
참조형 : Object, Array, Funtion, Date, RegExp 등
</pre>
</details>

## 변수에 원시값 데이터를 할당할 때의 과정
<details>
<summary>자세히 보기</summary>
<pre>

1. 변수에 대한 메모리 공간 할당
2. 원시 값 데이터를 할당된 메모리 공간에 저장
3. 식별자를 값이 저장된 메모리 주소에 연결
</pre>
</details>

## 변수에 객체(참조값 데이터)를 할당할 때의 과정
<details>
<summary>자세히 보기</summary>
<pre>

1. 메모리의 두 공간을 확보
2. 한 공간에는 실제 객체를 저장하고 다른 공간에는 객체가 저장된 공간을 가리키는 참조 값을 저장
3. 변수의 식별자에 참조값이 저장된 메모리 주소를 연결
</pre>
</details>

## undefined와 null의 차이점
<details>
<summary>자세히 보기</summary>
<pre>

undefined는 다음 상황에서 자바스크립트가 반환해주는 값
1. 변수 선언만 하고 할당하지 않았을 때 (var, let)
2. 객체 내부에 존재하지 않는 프로퍼티에 접근하려고 할 때
3. return문이 없거나 호출되지 않은 함수 실행 결과

개발자가 “없다" 라는 것을 명시할 때 null을 사용.
👀 querySelector나 getElementById 등의 DOM 선택 메서드에서 요소를 찾지 못했을 땐 null이 반환된다. 
</pre>
</details>

## 얕은 복사와 깊은 복사
<details>
<summary>자세히 보기</summary>
<pre>

- 얕은 복사 : 객체의 첫 번째 레벨(1단계)의 속성만 복사
ex) 스프레드 문법, slice(), concat()

- 깊은 복사 객체의 모든 레벨의 속성을 완전히 복사
ex) 라이브러리(immutable, immer), JSON.parse(), JSON.stringify() 메서드

👀 JSON.parse(), JSON.stringify()은 속도가 느리고 JSON으로 변경할 수 없는 프로퍼티는 무시된다는 단점
</pre>
</details>

## call by value, call by reference
<details>
<summary>자세히 보기</summary>
<pre>

- 원시타입의 인수는 값 자체가 복사되어 매개변수에 전달되므로 함수 내부에서 그 값을 변경해도 원본이 영향이 없다.
- 참조 타입의 인수는 값 자체가 아니라 참조(값의 주소)값이 복사되어 매개변수에 전달되므로 함수 내부에서 그 값을 변경하면 원본도 변경된다.
- 따라서 함수 내부에서 객체의 상태 변경이 필요한 경우, 깊은 복사를 통해 새로운 객체를 재할당하는 것이 바람직하다.
</pre>
</details>

## 호이스팅
<details>
<summary>자세히 보기</summary>
<pre>

- JavaScript 엔진은 코드를 실제로 실행(런타임)하기 이전에 평가 단계에 변수 및 함수의 선언을 식별하고 처리한다. 이처럼 선언문이 코드의 선두로 끌어 올려진 것처럼 동작하는 자바스크립트의 특징을 호이스팅이라고도 한다.
</pre>
</details>

##  let, var, const의 차이점
<details>
<summary>자세히 보기</summary>
<pre>
재선언, 재할당, scope 세가지에 따라 구분할 수 있다.

- var는 재선언, 재할당이 가능하고 함수 스코프를 가진다
- let은 재선언 불가, 재할당 가능, 블럭(중괄호) 스코프를 가진다.
- const는 재선언, 재할당 불가, 블럭(중괄호) 스코프를 가진다.
</pre>
</details>

##  원시 타입과 참조 타입의 차이
<details>
<summary>자세히 보기</summary>
<pre>
- 원시 타입
불변성, 새로운 메모리에 재할당값이 저장될 뿐 기존 값은 절대 변하지 않는다 
number, string, boolean, null, undefined, symbol

- 참조 타입
변수가 실제 데이터가 저장된 공간이 아니라 참조값()이 저장된 공간을 참조한다.
</pre>
</details>
