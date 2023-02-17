---
layout: post
title: Javascript 기본 문법 .Day2
subtitle:
categories: Javascript
tags: javascript
---

## 상호작용에 관한 함수

> 모달 창 **modal window**

- 메세지가 있는 작은 창
- 페이지의 나머지 부분과 상호 작용이 불가능

### alert

```javascript
    alert();
```

- 확인

### prompt

```javascript
    prompt(보여줄 문자열, [입력 필드의 초깃값])
```

- 입력 필드, 확인, 취소
- 입력 필드 문자열 반환 / null
- 미입력 : `' '` 빈 문자열 반환
- `ESC` : `null` 반환

### confirm

```javascript
    confirm(question);
```

- 질문 question, 확인, 취소
- true / false

## 형 변환 Type Conversion

### 문자형 변환

```javascript
    String(value);
```

- `alert()` : 매개변수를 문자형으로 받아, 다른 형의 값은 문자형으로 자동 변환

### 숫자형 변환

```javascript
    Number(value);
```

- 숫자 이외의 글자가 들어있는 문자열을 숫자형으로 변환 : `NaN` 형 변환 실패

> **NaN** : Not-a-Number

### 불린형 변환

```javascript
    Boolean(value);
```

- `false` : 0, 빈 문자열, null, undefined, NaN

## 기본 연산자

- `+` :  숫자가 아닌 경우 숫자형으로의 변환

```javascript
    console.log(+true);  // 1
    console.log(+'');   // 0
```

- [우선순위](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Operator_Precedence#table) 가 있다.

### 할당연산자

- `x=value` : `x`에 `value`가 쓰여지고 `value` 반환

### 증가·감소 연산자

> `++`    `--`

- `counter++` postfix form : 증가·감소 후 **새로운 값 반환**
- `++counter` perfix form : **기존값 반환** 후 증가·감소
-  변수에만 쓸 수 있다.

### 비트 연산자 bitwise operator

> `&`(and)    `|`(or)    `!`(not)

### 쉼표 연산자

- 여러 표현식을 코드 한 줄에서 평가할 수 있게 해준다. 표현식 각각이 모두 평가되지만, 마지막 **표현식의 평가 결과만 반환**된다.
- 쉼표의 우선순위는 매우 낮다. 할당 연산자 `=`보다 더 낮다.

## 비교 연산자

> 동등 연산자 equality operator
> 일치 연산자 strict equality operator

### 다른 형을 가진 값 간의 비교

- `true == 1`, `false == 0`

### 동등 연산자

> Equality operator

- `0 == false`, `'' == false` >> true <br> 숫자형으로 형변환

### 일치 연산자

> strict Equality operator

- **형변환 없이** 값 비교

### null과 undefined

- `null == undefined`
- 일치 연산자를 제외한 비교에서의 형변환<br>: null → 0, undefined → NaN

## 조건 처리

### 조건부 연산자

> 물음표 연산자, 삼항 연산자 **?**

```javascript
    let result = condition ? value1 : value2;
```

- 조건에 따라 `true : false` 반환
- 우선 순위 : 비교 연산자 > 물음표 연산자

## 논리 연산자

> `&&`(and)    `||`(or)    `!`(not)

- 왼쪽부터 시작해 피연산자를 평가

||AND|OR|
|---|:---:|:---:|
|연산을 멈추고 값 반환|false|true|
|마지막 값 반환|true|false|

> nullish 병합 연산자 `??`

- `0`이 할당될 수 있는 기능 개발에 적합

### ! NOT

- 불린형으로 변환 → 역 반환
- 불린형 변환 : `!!`, `Boolean()`

## 반복문

> while, for

- 반복 iteration : 반복문 본문이 한 번 실행

```javascript
    while (condition) { 반복문 본문 }
```

```javascript
    do {
        // 반복문 본문
    } while (condition)
```

```javascript
    for (begin; condition; step) { 반복문 body }
```

- begin → condition → body → step
- 무한 반복문 : `for (;;) { }`

### break, continue

- 중첩 레벨 감소
- 삼항 연산자에 사용 불가
- 레이블 : 중첩 반복문을 한 번에 빠져나와야 하는 경우

## switch 문

```javascript
    switch (x) {
        case 'value1':
            break;
        case 'value2':
            break;
        default:
            break;
    }
```
- x와 case문의 값이 일치 비교
- case문 안에 `break`가 없다면 이하 모두 실행

## 함수

- 매개변수 : 함수는 언제나 복사된 값 사용

### 함수 선언

> Function Declarartion

```javascript
    function 함수이름(파라미터){
        // 함수 본문
    }
```

### 함수 표현식

> Function Expression

```javascript
    let 함수이름 = function(파라미터){
        // 함수 본문
    }
```

### 함수 선언 vs 표현식

- 문법
- 자바스크립트 엔진이 **함수를 생성하는 시기**
- 스코프

### 화살표 함수

```javascript
    let 함수이름 = (파라미터) => expression
```
