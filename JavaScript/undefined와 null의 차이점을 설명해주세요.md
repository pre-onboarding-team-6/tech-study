# undefined와 null의 차이점을 설명해주세요.

## 답변

undefined와 null 모두 값이 없음을 나타내지만, 할당하는 주체에 대한 차이가 있습니다.

undefined는 자바스크립트 엔진이 변수를 초기화할 때 사용하는 값으로, 변수를 선언했지만 값이 할당되지 않았을 때의 기본값입니다. 또한, 변수가 초기화되지 않았거나 존재하지 않는 객체 속성에 접근하려고 할 때도 undefined가 반환됩니다.

null은 개발자가 변수에 값이 없음을 의도적으로 명시할 때 사용합니다. 변수에 null을 할당함으로써 이전에 할당되어 있던 값에 대한 참조를 제거합니다.

요약하자면 undefined는 값이 할당되기 전인 초기화 상태, null은 값이 없는 상태를 의미합니다. 때문에 변수의 값을 지우기 위해 개발자가 직접 undefined를 할당하는 것은 지양되며, null을 사용하는 것이 권장됩니다.

> **참고자료 및 꼬리질문 대비 자료**
>
> [자바스크립트 기술면접 1편 - undefined와 null의 차이점](https://velog.io/@iamkjw/%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8-%EA%B8%B0%EC%88%A0%EB%A9%B4%EC%A0%91-1%ED%8E%B8)  
> [프론트엔드 개발자 면접 질문(기술면접) 정리 - null vs undefined ](https://sunnykim91.tistory.com/121)
