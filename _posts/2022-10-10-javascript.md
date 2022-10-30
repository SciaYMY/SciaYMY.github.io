---
layout: post
title: Javascript 기본 문법 .Day1
subtitle: 
categories: Javascript
tags: javascript
---
> 코어 자바스크립트 **core JavaScript**

실행 환경에 독립적인 자바스크립트

- **서버 사이드 환경(node .js)**에서 스크립트 실행 가능

## script 태그

```javascript
    <script> </script>
```

- HTML4 - type 속성

```javascript
    <script type="text/javascript"> </script>
```

### 외부 스크립트

```javascript
    <script src="경로"> </script>
```
- scr 속성이 있으면 태그 내부의 코드 무시

## 세미콜론

- 자바스크립트에 줄 바꿈이 있으면 암시적 세미콜론으로 해석

## 주석 Comment

- 한줄 : `//`
- 여러줄 : `/* */` - 중첩 주석 미지원

## 엄격 모드

> use strict

- 이 지사자가 스크립트 최상단에 오면 스크립트 전체가 **모던한** 방식으로 동작

## 변수와 상수

- camelCase
- [예약어](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Lexical_grammar#keywords)

## 자료형

- 동적 타입 ***dynamically typed*** 언어 : 자료의 타입은 있지만 변수에 저장되는 값의 타입은 언제든지 바꿀 수 있는 언어
- 종류 : 숫자형, 문자형, 불린형, null 값, undefined 값, 객체형, 심볼형
  - **null** : 존재하지 않는 값 nothing, 비어 있는 값 empty, 알 수 없는 값 unknown
  - **undefined** : 값이 할당되지 않은 상태

