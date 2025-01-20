![Header](https://github.com/user-attachments/assets/504cc37b-7dab-4a1a-9aaa-bf5ee1d60e86)

## 개요
선택한 의상들을 기반으로 좋아할 만한 코디를 추천하는 서비스(의 iOS 애플리케이션)

**리팩토링 2024.09**

<br/>

## 사용 기술
**디자인 패턴은 MVC를 사용했습니다.(워낙 소규모라..)**

| 이름 | 목적 |
| --- | --- |
| Alamofire | HTTP 통신 작업을 수행합니다. |
| SnapKit | AutoLayout 제약조건 코드의 가독성을 개선합니다. |

<br/>

## 문제 해결
<details>
  <summary>서버 접속 실패 시 재시도 로직 구현</summary>
  
  ### 문제 상황
  일정 횟수만 재시도 후 최종 접속 실패를 구현하고 싶었으나 재시도 횟수를 저장하는 프로퍼티를 메서드 외부에 선언하고 싶지 않았습니다.

  ### 해결 방법
  접속 메서드의 파라미터에 재시도 횟수를 전달하고, 메서드를 재귀 호출해 문제를 해결할 수 있었습니다.
</details>

<br/>

## 지원
[✉️ jjingeo1230@gmail.com](mailto:jjingeo1230@gmail.com)
