# Ch2. 자바스크립트란?

## 자바스크립트의 표준화
- 자바스크립트가 탄생후 얼마 지나지않아 자바스크립트의 파생버전인 JScript의 탄생 
- JScript와 자바스크립트가 자사 브라우저 시장점유율을 높이기 위해 자사 브라우저에서만 동작하는 기능을 추가 
    - 브라우저에 따라 웹페이지가 정상적으로 동작하지않는 **크로스 브라우징 이슈** 가 발생
    - 이로인해 표준화된 자바스크립트의 필요성이 대두되기 시작 
        - ESMAScrip로 명명된 표준화된 자바스크립트가 탄생 

## 자바스크립트 성장의 역사 
- 초창기 자바스크립트는 웹페이지의 보조적 기능을 수행하기 위한 용도로 사용. 

### Ajax
- 서버와 브라우저가 **비동기** 방식으로 데이터를 교환할수 있는 통신기능 **Ajax**가 **XMLHttpRequest** 라는 이름으로 등장 
- 이전에는 변경할 필요가 없는 html코드도 서버로 다시 전송받아 랜더링하는 방식으로 성능면에서 매우 불리했다. 
    - Ajax의 등장으로 서버로부터 필요한 데이터만 전송받아 변경해야하는 부분만 한정적으로 랜더링 

### jQuery
- jQuery의 등장으로 DOM을 더욱 쉽게 제어할수 있게 되었고 크로스 브라우징 이슈도 어느정도 해결. 

### V8 자바스크립트 엔진 
- 더욱 빠르게 동작하는 자바스크립트의 엔진의 필요성이 대두 
    - V8 자바스크립트 엔진은 이러한 요구에 부합하는 빠른 겅능을 보여줌
- 자바스크립트는 데스크탑 에플리케이션과 유사한 UX(사용자 경험)을 제공할 수 있는 웹애플리케이션 프로그래밍 언어로 정착 

### Node.js
- 구글 V8 자바스크립트 엔진으로 빌드된 자바스크립트 런타임 환경이다. 
- 브라우저 자바스크립트엔진에서만 동작하던 자바스크립트를 브라우저 이외의 환경에서도 동작할 수 있도록 자바스크립트 엔진을 브라우저에서 독립시킨 자바스크립트 실행환경이다. 
- 프론트엔드와 백엔드 영역에서 자바스크립트를 사용할 수 있다는 장점이 있따. 
- **비동기I/O**를 지원하면 **딘일 스페드 이벤트 루프** 기반으로 동작함으로써 요청 처리 성능이 좋다. 
    - CPU사용률이 높은 애플리케이션에는 권장하지않는다. 

### SPA 프레임워크
- 개발 규모와 복잡도 상승으로 이전의 자바스크립트만으로는 개발 과정을 수행하기가 어려워짐 
    - 이로 인해 많은 패턴과 라이브러리가 출현했다. 이는 개발엔 도움을 주었지만 확장하기 쉬운 아키텍쳐 개발을 어렵게했다
        - 이러한 요구에 Angular, React, Vue.js등 다양한 SPA프레임워크, 라이브러리가 탄생했다. 


## 자바스크립트와 ECMAScript
- ECMAScript는 자바스크립트 표준사양을 말하며 핵심 문법을 규정한다 
- 각 브라우저 제조사는 ECMAScript사양을 준수해서 브라우저에 내장되는 자바스크립트 엔진을 구성한다. 
- 자바스크립트는 ESMAScript 와 브라우저가 별도 지원하는 클라이언트사이드 Web API이다. 

## 자바스크립트의 특징 
- 자바스크립트는 웹브라우저에서 동작하는 유일한 프로그래밍 언어이다. 
- 기본문법은 C, Java와 유사하고 셀프에서는 프로토타입기반삳속을, 스킴에서는 일급함수 개념을 차용했다. 
- 자바스크립트는 개발자가 별도의 컴파일 작업을 수행하지 않는 인터프리터 언어다. 
- 명령형, 함수형, 프로토타입기반 개체지향프로그래밍을 지원하는 멀티패러다임프로그래밍 언어이다. 
