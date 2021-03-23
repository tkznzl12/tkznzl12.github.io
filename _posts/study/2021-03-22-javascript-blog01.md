---
title: JavaScript 기초
layout: post
subtitle: JavaScript에 대해 이해하자
categories: study
tags: JavaScript
comments: true
---

# 정규표현식
 - 문자열에서 특정한 문자를 찾아내는 도구
 (하나의 언어라고도 할 수 있다).
 - 이 도구를 이용하면 수십줄이 필요한 작업을 한줄로 끝낼 수 있음.
 - 참고 사이트 : https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Regular_Expressions
<br>

**정규표현식의 단계**

정규표현식은 두가지 단계로 이루어진다.
> - **컴파일(Compile)**
>  검출하고자 하는 패턴을 만드는 일
> - **실행(execution)**
>  대상에 대해서 어떠한 작업을 구체적으로 하는것

 - 컴파일
   -
   - 정규표현식 리터럴
   **var pattern = /a/**
   **var pattern = /a./** //여기서  '.'은 문자를 나타냄
   - 정규표현식 객체 생성자
   **var pattern = new RegExp('a')**

  위의 표현을 해석해보면 a가 우리가 찾고자 하는 대상이라는 것을 알려주고 pattern이라는 것에 변수로 지정해준다는 뜻이다.
  (두개의 표현만 다를뿐 같은 의미)

 - 실행
   -
   정규표현식을 컴파일 해서 객체를 만들었다면 아제 문자열에서 원하는 문자를 찾아내야함
   <br>
>   - **RegExp.exec() : (추출)**
>    pattern.exec('abcde');를 할경우 도출되는 것은 a이다.
>    (입력한것 중에 a가 있다는 의미.)
>    만약 a가 없을경우엔 null이 뜬다.
><br>
>    - **RegExp.test() : (존재유무를 test)**
>     pattern.test('abcde');를 할경우 도출되는 것은 true이다.
>     (입력한것 중에 a가 있다는 의미.)
>     만약 a가 없을경우엔 false가 뜬다.
   <br>
   <hr>

>   - **문자열 메소드**
    ***String.match()***
    RegExp.exec()와 비슷함.
    ***String.replace()***
    문자열에서 패턴을 검색해서 이를 변경한 후에 변경된 값을 리턴함.
   <br>

  - **옵션**
   */"string"/**i***
   : i가 붙어있다는 것은 대소문자를 구분하지 않겠다는 의미<br>
   */"string"/**g***
   : //안의 문자의 갯수 만큼을 출력하겠다는 의미   
  **두개를 합쳐서 사용할 수도 있음.**
   <br>
