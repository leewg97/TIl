## Type Annotation

### 타입 어노테이션 (Type Annotation)

- 변수나 상수를 선언할 때 그 타입을 명시적으로 선언해 줌으로써 **어떤 타입의 값이 저장될 것인지**를 직접 알려주는 방법
- 프로그램은 수많은 함수, 클래스 등으로 복잡하게 얽혀있는 경우가 많은데, **변수 타입이 맞지 않으면 에러나 버그의 발생 가능성**이 높아짐
- 사용 시, **코드 가독성**과 **협업 효율성**이 높아짐
- Python 3.5 부터 기능이 지원되어 많은 라이브러리, 프로젝트에서 사용이 확산되는 추세
- 파이썬은 프로그램 실행 도중 변수 타입을 동적으로 바꿀 수 있는 **`동적 프로그래밍 언어(dynamic programming language)`**
- Java, C, C++ 등은 컴파일 시 변수 타입이 결정되는 **`정적 프로그래밍 언어(statically typed language)`**

💡동적 프로그래밍 언어의 장단점
- 장점
  - 타입에 자유로워 유연한 코딩이 가능하므로 쉽고 빠르게 프로그램을 만들 수 있음
  - 타입 체크를 위한 코드가 없으므로 비교적 깔끔한 소스 코드
- 단점
  - 프로젝트의 규모가 커질수록 잘못된 타입 사용으로 말미암은 버그가 생길 확률 높아짐
  - 타입 어노테이션이 없을 시, 정적 프로그래밍 언어와 타입 버그 발생 시 원인 찾기 어려움
  - 실행속도가 느림