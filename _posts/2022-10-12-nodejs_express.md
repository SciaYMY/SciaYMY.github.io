---
layout: post
title: Node.js로 Express 사용하기
subtitle: 
categories: Nodejs
tags: nodejs express
---
> Node.js는 Chrome V8 JavaScript 엔진으로 빌드된 JavaScript 런타임이다.

## npm

> Node Package Manager 또는 Node Package Modules

> Node.js의 패키지 생태계

- npm은 세계에서 가장 큰 오픈 소스 라이브러리 생태계이기도 하다.

### package.json

> 프로젝트에 대한 명세

- Node.js 버전 관리를 할 수 있다.

## Node.js로 Express 사용하기

`Express-generator`는 Express 환경을 간단하게 구축해주는 npm이다.

```node.js
    npm install -g express-generator
    express jsproject --view=pug
    npm install
    npm start
```
1. npm 전역설치 :`npm install -g express-generator` 
2. 새 express 프로젝트 생성 : `express [설치할 폴더이름] --view=pug` 
   - `--view=pug` : **pug 템플릿 엔진** 사용
3. npm 모듈을 설치 : `npm install`
   - package.json 생성
