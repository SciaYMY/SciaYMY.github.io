---
layout: post
title: JavaScript .Day1
subtitle: 
categories: Javascript
tags: javascript
---
## 자바스크립트

> 스크립트 script : 자바스크립트로 작성한 프로그램

### 자바스크립트 이름의 역사

> LiveScript → JavaScript → ECMAScript

- 당시 시대의 자바의 인기로 인한 명칭 변경

### 자바스크립트 엔진

브라우저에는 **자바스크립트 가상머신**이라 불리는 엔진이 내장되어 있다.

#### 브라우저에 따른 JavaScript 엔진 코드네임

- Chrome, Opera - V8
- Firefow - 스파이더 몽키 Spider Monkey
- 익스플로러 - 트라이던트 Trident, 샤크라 Charkra
- Microsoft Edge - 샤크라코어 ChakraCore
- Safari - 시쿼럴피쉬 SquirrelFish

### 엔진 동작

1. 파싱 : 엔진이 스크립트를 읽는다.
2. 컴파일 : 읽어 들인 스크립트를 기계어로 전환한다.
3. 기계어로 전환된 코드가 빠르게 실행한다.

> 가비지 컬렉션 Garbage Collection : 엔진에서 메모리 관리

### 브라우저 환경에서의 자바스크립트

#### 할 수 있는 영역

- 웹조작, 클라우드/서버 상호작용
- 이벤트 조작, Ajax
- 쿠키 값을 가져오거나 설정, 사용자에게 메시지 보여주기
 (인터넷 사용기록 설정 : Ctrl + Shift + Del)

    ┌ 쿠키 Cookie : 웹브라우저 정보를 가지고 있는 값, 브라우저에 저장   
    ├ 세션 Session : 사용자 식별자로 저장, 노출되는 쿠키 보안 문제 방지     
    └ 캐시 : 서버에서 미리 받아둔 내 로컬에 남아있는 정보

### 자바스크립트의 발전

- 트랜스파일 : 브라우저에서 실행 되기 전에 자바스크립트로 변환

#### 트랜스파일 가능한 새로운 언어
> TypeScript / CoffeScript / Flow / Dart

### Web Framework
> **Express** - Node.js 웹 애플리케이션 프레임워크

- Python : Django, Flask, FastAPI ...

#### Node.js로 Express 사용하기

{% highlight Node.js %}
    npm install -g express-generator
    express jsproject --view=pug
    npm install
    npm start
{% endhighlight %}
