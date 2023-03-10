## 코드 생성과 타입이 관계없음을 이해하기
- 타입스크립트 컴파일러의 2가지 역할
  - 최신 Typescript/ Javascript 가 브라우저에서 동작할 수 있도록 구버전의 Javascript 로 transpile.
  - 컴파일은 타입 체크와 독립적으로 동작, 타입 오류가 있는 코드도 컴파일이 가능.
    - 오류가 있을때, 컴파일하지 않으려면 'noEmitOnError' 옵션을 사용하면 된다.
    - https://www.typescriptlang.org/tsconfig#noEmitOnError
  - 런타임에는 타입체크가 불가능함.
    - 실제로 자바스크립트로 컴파일 되는 과정에서 모든 인터페이스, 타입, 타입구문은 그냥 제거됨.
      - instanceof 인터페이스는 소용없지만, instanceof abstract class 하면 쓸모있어짐
  - 타입연산은 런타임에 영향을 주지 않음.
  - 런타임의 타입은 선언된 타입과 다를 수 있음.
  - 타입스크립트의 타입으로는 함수를 오버로드 할 수 없음
    - 선언문을 여러개써서 할 수는 있는데, 결국 구현체는 하나임.
  