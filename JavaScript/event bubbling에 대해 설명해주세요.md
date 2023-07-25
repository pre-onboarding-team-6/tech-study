# event bubbling에 대해 설명해주세요.

## 답변

**event bubbling**이란 특정 요소에 이벤트 발생 시 이 요소를 자손으로 가지는 요소들의 이벤트 핸들러 또한 동작하는 것을 의미합니다.

어느 DOM 요소에서 이벤트가 발생하면 이 요소에 연결된 핸들러가 동작한 후 부모 요소의 핸들러도 동작하며, 요소가 속해있는 최상단 조상 요소 document에 다다를 때까지 이 과정을 반복합니다. event bubbling은 이벤트 위임의 작동 메커니즘입니다.

**이벤트 위임**은 하위 요소가 여럿 있을 때 상위 요소에 핸들러를 달아 하위 요소들을 제어하는 방식입니다. 이 방식의 이점으로 상위 요소에만 이벤트 핸들러를 연결하면 되기 때문에 코드가 깔끔해지고, 메모리상 이벤트 핸들러의 개수 또한 적어집니다. 또한 하위 요소가 추가되어도 핸들러를 고려할 필요가 없어집니다.

> **참고자료 및 꼬리질문 대비 자료**
>
> [Front End Interview Handbook - event bubbling에 대해 설명하세요](https://www.frontendinterviewhandbook.com/kr/javascript-questions#event-bubbling%EC%97%90-%EB%8C%80%ED%95%B4-%EC%84%A4%EB%AA%85%ED%95%98%EC%84%B8%EC%9A%94)  
> [javascript.info - 버블링과 캡처링](https://ko.javascript.info/bubbling-and-capturing)  
> [Must-Know-About-Frontend - 이벤트 위임](https://github.com/baeharam/Must-Know-About-Frontend/blob/main/Notes/javascript/event-delegation.md)
