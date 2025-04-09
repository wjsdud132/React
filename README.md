# 202130129 전진영

# 4월 3일 (5주차)

## 화면 업데이트하기
- component가 특정 정보를 "기억"해 두었다가 표시하기를 원하는 경우가 있습니다.

- 예를 들어 버튼이 클릭된 횟수를 세고 싶을 수 있습니다.

- 이렇게 하려면 component에 state를 추가하면 됩니다.

- 먼저, React에서 useState를 import합니다.

- 이 코드를 보면 useState는 react 파일 안에 Named Exports로 선언되어 있는 여러 개의
component 중 하나는 것을 알 수 있습니다.

- 이제 component 내부에 state 변수를 선언할 수 있습니다.

- useState로부터 현재의 state를 저장할 수 있는 변수인 count와 이를 업데이트할 수 있
는 함수인 setCount를 얻을 수 있습니다.

- 이름은 자유롭게 지정할 수 있지만 [something, setSomething]으로 작성하는 것이 일반
적입니다.

- 즉, 변수 이름과 변수 이름 앞에 set을 붙인 업데이트 함수를 관용적으로 사용합니다.

## Hook 사용하기

use로 시작하는 함수를 Hook이라고 합니다.

- useState는 React에서 제공하는 내장 Hook입니다.

- 다른 내장 Hook은 API 참고서에서 찾아볼 수 있습니다.

- 또한 기존의 것들을 조합하여 자신만의 Hook을 작성할 수도 있습니다. 사용자 Hook.

- Hook은 다른 함수보다 더 제한적입니다.

- component 또는 다른 Hook의 상단에서만 Hook을 호출할 수 있습니다.

- 조건이나 반복문에서 usestate를 사용하고 싶다면 새 컴포넌트를 추출하여 그곳에 넣으
세요.


## Hooks의 사용 규칙(Rules of Hooks)
### 왜 이런 제한이 필요한가?
- React의 동작을 예측 가능하고, 안정성을 높이기 위해 필요한 규칙입니다.

1. rendering 순서를 보장하기 위해
조건문이나 반복문 안에서 Hooks를 사용하면 매 rendering마다 Hook의 호출 순서가 달
라질 수 있기 때문에 React가 상태를 제대로 추적할 수 없습니다.

2. 불필요한 사이드 이펙트 방지
component가 여러 번 rendering될 때마다 동일한 순서로 Hook이 실행되어야 React가
의도한 동작을 수행할 수 있습니다.

# 3월 20일 (3주차)

### node_modules
- git으로 관리하지 않기 때문에 디렉토리 이름이 흐릿하게 나와 있는 것을 확인할 수 있습니다. 

### public  
- 정적(static) 파일을 저장하는 디렉토리 입니다.   
- build 후 배포할 html, CSS, JavaScript 등이 보관되는 곳입니다.   
- 개발하면서 특별히 수정할 코드는 없습니다.

### public/index.html   
- React 앱이 마운트 되는 HTML 파일.   

### src/   
- React 프로젝트의 주요 코드가 위치하는 디렉토리 입니다.    
- 개발하면서 대부분의 작업이 이루어지는 곳입니다.

### src/App.js   
- 메인 component 로 필요한 sub component 를 모아서 관리합니다.   
- 출력을 위해서 index.js 로 전달됩니다.

### src/App.css   
- App.js에 적용되는 스타일을 정의하는 스타일 파일입니다.

### src/index.js   
- React 앱의 진입 점(entry point)으로 최종 렌더링이 되는 곳입니다.   
- ReactDOM.createRoot 를 사용하여 App.js를 렌더링합니다.

### src/index.css   
- 전역 스타일을 정의하는 스타일 파일입니다.

## 의존성 관리와 package.json
- package.json은 패키지의 의존성을 관리하는 파일입니다.
- 의존성(Dependency) 이란, 하나의 소프트웨어가 다른 소프트웨어(라이브러리, 패키지, 모듈 등) 에 의존하여 동작하는 관계를 말합니다.
- 즉, 어떤 프로젝트에 사용된 각종 패키지 등의 버전을 동일하게 유지하기 위한 것입니다.


# 3월 13일 (2주차)


## Node.js활용


- 웹서버
  * REST API, GraphQL API

- 실시간 애플리케이션
  * 실시간 알림, 채팅, 스트리밍


### Node.js의 장단점


## 장점

- JavaScript 풀스택 개발이 가능하여 생산성이 향상됨

- npm의 방대한 생태계를 활용 가능함

- 실시간 데이터 처리가 강력함

## 단점

- 콜백 지옥의 문제점

- 보안 취약의 문제점

