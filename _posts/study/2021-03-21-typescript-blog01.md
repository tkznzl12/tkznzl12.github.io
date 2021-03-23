---
title: TypeScript 기초
layout: post
subtitle: TypeScript에 대해 이해하자
categories: study
tags: TypeScript
comments: true
---

# TypeScript기초
<br>

  **TypeScript란?**
  - 자바스크립트에 타입을 부여한 언어

  **TypeScript의 장점?**
  - 에러의 사전방지 : 항상 코드 작성 후 브라우저로 가 에러를 확인했다면, 브라우저로 가기 전 코드에서 에러를 확인할 수 있게함(ex>단어...)
  - 코드 가이드 및 자동완성

  >- TypeScript에서 변수에 타입을 줄 떄 : String 이런식으로 값을 주어 타입을 입력시킨다.
  > - 변수의 타입이 다른것이 들어갈경우 빨간 밑줄을 주어 에러를 표시해준다

  **TypeScript 기본타입(새로운 방식)**
  >**튜플**
  >주로 배열에서 쓰이는 것으로 단순히 배열 안에 들어가는 타입을 한개만 선언하는 것이 아닌 각각의 변수를 선언해 주는것
  >**ex>let address: [String,number] = []**
  >
  >**객체**
  >오브젝트
  >**ex>
  >let obj: object ={
  >name:
  >age:
  >};**
  >
  >**let person: {name:string, age:number} ={
  >name:
  >age:
  >};**

  **함수 타입**
  >**옵셔널 파라미터**
  >선택적으로 값을 입력?시키는것.
  >인자 2개를 선언하고 1개만 받아온다던가 하는...
  >인자를 **b:String** 이렇게 선언했을때, **b?:String**같은 형식으로 ?를 넣어준다면 해당인자는 넣어도 되고 안넣어도 되는 선택적 파라미터가 된다.
