## 타입스크립트 설정 이해하기
- any type 사용 XXXX
  - 타입체커가 무력화됨.
  - 따라서 되도록 'noImplicitAny' 옵션을 사용하도록 하자.
- <a href= 'https://www.typescriptlang.org/tsconfig#strictNullChecks'>strictNullChecks</a> 옵션을 사용하면 null, undefined가 모든 타입에서 허용되는지 확인하는 설정
  - 쉽게 말해서 null 또는 undefined 를 참조하는걸 방지할 수 있음.
  - runtime에서 터지는걸 막을 수 있을듯?
  - 그리고 명시적으로 null을 허용함을 표기해서 좀 더 명확하게 코드를 짤 수 있을듯.
- 엄격한 체크를 위해 strict 설정을 고려하자
  