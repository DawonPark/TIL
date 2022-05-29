# 브라우저, 그리고 동작 방식
## 브라우저
### 정의
- HTML, CSS 명세에 따라 HTML 파일을 해석해서 표시하며 웹 표준화 기구인 과거에는 독창적인 브라우저가 있었지만 호환성에 심각한 문제를 겪으며 현재는 W3C(World Wide Web Consortium)의 표준명세를 따르게 되었다.


### 구조
![브라우저 컴포넌트](https://www.html5rocks.com/en/tutorials/internals/howbrowserswork/layers.png)

1. User Interface : 이전, 다음, 새로고침, 북마크와 같이 페이지가 보여지는 부분 이외에 모든 이용자에게 동일하게 보이는 부분이다.
2. Browser engine : 유저 인터페이스와 렌더링 엔진 사이에 쿼리를 전달할 수 있도록 조작을 담당한다.
3. Rendering engine : 사용자가 요청한 페이지를 나타내기 위한 HTML, CSS 분석한다.
4. Networking : HTTP를 요청하고 네트워크 호출에 이용한다.
5. JavaScript Interpreter : Javascript 코드 해석과 실행을 한다.
6. UI Backend : 기본적이 UI를 그리는데 사용하며, 보통 콤보 상자와 창과 같은 기본 위젯을 그리는데 사용한다.
7. Data Persistence : 쿠키와 같은 자원들을 저장한다.

### Rendering engine 의 동작 방식
- 렌더링 엔진은 브라우저마다 다를 수 있지만 동작 과정은 비슷하다.
![랜더링 엔진 기본 흐름](https://www.html5rocks.com/en/tutorials/internals/howbrowserswork/flow.png)
1. HTML 파싱 후 DOM 트리 구축
   -  HTML, CSS 각자의 파서를 이용하여 HTML은 각 태그들로 DOM트리 구성한다.
2. 렌더 트리 구축
   -  CCS는 스타일 규칙에 맞게 파싱 후 렌더트리 생성한다.
3. 렌더 트리 배치
   - - 각 노드 별 화면의 정확한 위치에 표시하는 작업한다.
4. 렌더 트리 그리기

![랜더링 엔진 플로우](https://www.html5rocks.com/en/tutorials/internals/howbrowserswork/webkitflow.png)
![랜더링 엔진 플로우](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FcLUQZs%2Fbtq0fkqwXxw%2FysRkZEkWwgR9RJRWxoBUNK%2Fimg.png)

- 위 두 그림 모두 HTML 파싱 후 돔트리를 만들고 CSS 파싱후 렌더 트리를 구축한 후 배치를 하고 그리는 과정을 확인 할 수 있다.