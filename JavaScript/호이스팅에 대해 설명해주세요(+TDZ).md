# 호이스팅에 대해 설명해주세요.(+TDZ)

## 답변

호이스팅은 변수 및 함수 선언문이 스코프 내의 최상단으로 끌어올려지는 현상입니다.

자바스크립트 엔진은 소스코드 평가과정에서 모든 선언문을 찾아내 먼저 실행합니다. 따라서 변수 선언이 소스코드의 어디에 위치하는지 상관없이 어디서든 변수를 참조할 수 있습니다.  
var의 경우 선언과 초기화 단계가 동시에 일어나서 선언문 이전에 호출하면 undefined를 반환합니다.  
let, const는 선언 단계와 초기화 단계가 나뉘어 있어 호이스팅으로 선언 단계는 진행하지만 초기화 단계는 선언문에 도달했을 때 실행합니다. 따라서 선언문 도달 전에 변수를 호출할 경우 초기화 단계가 실행되지 않아 변수에 메모리가 할당되지 않았기 때문에 ReferenceError가 발생하며 이를 TDZ(Temporary Dead Zone)라고 합니다.

> **참고자료 및 꼬리질문 대비 자료**
>
> ```
> 변수
> 1. 선언 단계(Declaration phase): 변수가 스코프 내에서 정의되고, 메모리에 공간을 확보합니다. 이때 변수는 undefined로 초기화됩니다. 이 과정을 호이스팅이라고 합니다.
> 2. 초기화 단계(Initialization phase): 선언된 변수에 값을 할당하고, 메모리에 할당된 공간을 변수와 연결합니다.
> 3. 할당 단계(Assignment phase): 초기화 단계에서 할당된 메모리 공간에 실제 값을 저장합니다.
> ```
>
> [깃허브 Must-Know-About-Frontend](https://github.com/baeharam/Must-Know-About-Frontend/blob/main/Notes/javascript/hoisting.md8)  
> [자바스크립트 기술면접 1편](https://velog.io/@iamkjw/%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8-%EA%B8%B0%EC%88%A0%EB%A9%B4%EC%A0%91-1%ED%8E%B8)  
> [[면접준비] 프론트엔드 개발자 취업 면접 질문 및 답변 정리(64문)](https://amyhyemi.tistory.com/224)
