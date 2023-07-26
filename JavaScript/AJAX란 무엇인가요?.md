# AJAX란 무엇인가요?

## 답변

Asynchronous Javascript And XML의 약자로, 비동기적으로 JS를 사용해서 데이터를 받아와 동적으로 DOM을 갱신 및 조작하는 웹 개발 기법을 의미합니다.

사용자가 AJAX가 적용된 UI와 상호작용하면, 서버에 AJAX 요청을 보내게 됩니다. 그러면 서버는 DB에서 데이터를 가져와서 JS 파일에 정의되어 있는 대로 HTML/CSS와 데이터를 융합하여 만든 DOM 객체를 UI에 업데이트 시킵니다.
비동기로 이루어지며, 기존의 페이지를 전부 로딩하는 방식이 아닌 일부만 업데이트 하는 방식입니다.
장점은 SPA와 마찬가지로 웹페이지를 업데이트시 새로고침 없이 필요한 부분만 업데이트 되어서 UX가 향상되지만 단점으로는 SEO가 까다롭고, 동적화면에서 History 관리와 북마크가 어려울 수 있습니다.
사용 방법은 XMLHttpRequest객체를 이용하는 것과 Fetch API를 이용하는 방법이 있습니다.

> **참고자료 및 꼬리질문 대비 자료**
>
> [AJAX란 무엇인가?](https://github.com/baeharam/Must-Know-About-Frontend/blob/main/Notes/javascript/ajax.md)
