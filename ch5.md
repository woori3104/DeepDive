# 표현식과 문

## 값
- 값은 식이 평가되어 생성된 결과를 말한다. 
    - 평가란 식을 해석해서 값을 생성하거나 참조하는 것을 의미한다. 

```
10+20 = 30
// 10+20은 평가되어 숫자 값 30을 생성한다. 
```
- 변수는 하나의 값을 저장하기위해 확보한 메모리 공간 자체, 또는 그 메모리공간을 식별하기 위해 붙인 이름

## 리터럴
- 리터럴은 사람이 이해할 수 있는 문자 또는 약속된 기호를 사용해 값을 생성하는 표기법을 말한다. 
    - 리터럴은 사람이 이해할 수 있는 문자(아라비아숫자, 알파벳,한글, 미리 약속된 기호)등으로 표기한 코드이다. 

## 표현식 
- 표현식은 값으로 평가될 수 있는 문이다. 
- 즉 표현식이 평가되면 새로운 값을 생성하거나 기존값을 참조한다. 
- 값으로 평가될 수 있는 문은 모두 표현식이다. 
```
// 리터럴 표현식 
10  // 정수리터럴
'Hello' // 문자열리터럴
true // 불리언 리터럴

// 식별자 표현식 (선언이 미리 존재한다고 가정)
sum
person.name
arr[1]

// 연산자 표현식 
10+20
sum = 10
sum !== 10

// 함수 메서드 호출 표현식 (선언이 이미 존재한다고 가정)
squre()
person.getName()
```

## 문
- 문은 프로그램을 구성하는 기본단위이자 최소 실행단위이다. 
- 문은 여러 토큰으로 구성된다.
    - 토큰은 문법적인 의미를 가지며, 문법적으로 더이상 나눌 수 없는 코드의 기본요소를 의미한다. 
        - ex) 키워드, 식별자, 연산자, 리터럴, 세미클론, 마침표
    - 문은 선언문, 할당문, 조건문, 반복문으로 구분할 수 있다. 

## 세미클론과 세미클론 자동 삽입 기능
- 세미클론은 문의 종료를 나타낸다. 
    - 자바스크립트엔진은 세미클론으로 문이 종료한 위치를 파악하고 순차적으로 하나씩 문을 실행한다. 
    - 자바스크립트엔진은 문의 끝이라고 예측되는 지점에 세미클론을 자동으로 붙여주는 자동삽인 기능이 암묵적으로 수행되기때문에 사용자가 생략할 수 있다. 
    - 자동삽입기능과 사용자의 예측이 반드시 일치하지않기때문에 ESLint등에서는 붙이는것을 권장한다. 

## 표현식과 표현식이 아닌 문
- 표현식인 문과 표현식이 아닌 문을 구별하는 가장 간단하고 명료한 방법은 변수에 할당해 보는 것이다. 
    - 표현식인 문은 값으로 평가될 수 있으며 문은 값으로 평가될 수 없다. 
    - 표현식은 값으로 평가되므로 변수에 할당할 수 있으나 문은 값으로 평가할 수 없어 할당시 에러가 발생한다. 