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

1. 메모리의 빈공간을 할당하고 식별자를 obj1으로 지정
2. 값이 객체이므로 내부 프로퍼티 저장을 위한 별도의 메모리 공간을 마련하고, 프로퍼티 개수에 따라 공간을 확보합니다
2. 프로퍼티의 키를 별도의 메모리 공간에 식별자로 저장합니다.
3. 메모리의 다른 부분의 프로퍼티의 value를 저장하고 이 값의 주소를 
</pre>
</details>
