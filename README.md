# Visual Studio code (VScode)
* vs code 실행 시 가장 먼저 확인해야할 것!
* 왼쪽 탐색기가 작업 폴더로 연결되어 있는지 확인하기!
* (위) 안돼있다면 -> 파일 -> 작업폴더 닫기 후 -> 폴더열기 다시 진행!
# html 시작
* git, github 개념공부
* `<태그>` 웹페이지에서 의미적인 정보를 가지는 대상
## HTML5 버전선언
* `<!doctype html>`
## HTML 구조태그
* html : 웹의 시작과 끝. 문서 자체의 의미
* head : 웹 문서의 정보, 제목 포함
* meta : 웹 문서의 정보 기록
* title : 웹 문서의 제목 (브라우저 상단 표시)
* body : 웹 문서 내용 (실제 대부분의 서비스가 들어가는 본문)
## 구조 태그 속성
* `lang="ko"` html 문서 언어 설정
* `charset="utf-8"` 다국어 문자열 설정
* `description` 사이트 요약 설명
* `keywords` 사이트 검색 키워드 설정
## 속성 문법
* `<태그 속성="값" 속성="값"></태그>`
* 태그와 속성 사이 공백
* 속성과 속성 사이 공백 (속성 개수 제한없음)
* 속성은 시작태그에만 작성하기!
## 구조태그의 'title'작성방법
* 메인페이지 -> 사이트명
* 메인페이지 -> 사이트명 | 광고문구 추가
* 서브페이지 -> 페이지명 | 사이트명
* ex) 책 이름-저자명 | 서점명
* ex) 판매 아이템명 | 사이트명
## h1~h3 제목태그(block tag)
* h1~h3 태그는 meta keywords와 동일한 검색 키워드로 활용된다. (대제목일수록 높음)
* h4~h6 태그는 거의 사용하지 않는다.
* h1 대제목은 사이트의 로고 및 서브 페이지 제목에 주로 사용한다.
* h 제목의 1~6레벨은 순서대로 작성해야 한다.
## 단락 p (block tag)
* 한 줄 또는 여러 줄 단락 묶을 때 사용하는 태그
* 제목(h)태그 종류와는 형제 태그 관계로 사용해야 한다. 부모-자식(x)
## 인라인태그 br, em, strong, del, s, sup, sub
* `br` : 블록 내 줄바꿈 태그
* `em` : 블록 내 강조 태그, 주로 내용 태그(p) 등에서 자식으로 사용
* `strong` : 블록 내 경고용 강조 태그 (위와 특징 동일)
* `del` : 삭제 텍스트, 쇼핑몰의 할인 전 가격 등에 사용
* `s` : 교체 텍스트, 쇼핑몰의 할인 전 가격 등에 사용 (del 자주사용)
* `sup, sub` : 윗첨자(sup) 아래첨자(sub) 수학, 과학등의 기호에 사용
## 인용문 처리 blockquote, q
* `blockquote(block)` : 단락 자체가 인용문에 해당할 때 사용, p태그와 부모-자식 관계로 사용해서는 안된다.
* `q(inline)` : 단락(p) 내에서 일부가 인용문에 해당할 때 사용
* 공통속성 `cite="URL"` : `blockquote`, `q`로 인용문 처리할 경우 출처 표시용도로 주소(URL)을 담아주는 속성.
## 특수문자 태그
* `&`시작 `;`종료
* `& copy ;` &시작과 copyright의 copy ;종료
## 주소태그
* `adress` footer영역에서 들어가는 본 사이트 주소
* inline을 주소태그 안에 넣을 수 있다.
## 수평선 태그
* `hr (block)` 복잡한 html 태그 경계 구분
* 주석과 같이 구조 이해를 위해 사용하고 CSS에서는 대부분 표현하지 않고 숨긴다.
## 컴퓨터 명령어 태그
* `code (inline)` : 웹 강의 사이트에서 주로 사용하는 태그
## 링크 태그
* block, inline 특징을 모두 가지낟.
* 절대경로와 상대경로를 href 속성에 작성한다.
* 상대경로는 a태그 작성중인 파일 위치 기준 연결하고자 하는 목적지 파일이 같은 위치에 있는지, 하위 위치에 있는지, 상위 위치에 있는지에 따라 다르게 작성한다.
* ./ 현재 위치에서 시작
* ../ 상위 폴더로 나가기
* `./doll.jpg` : 현재 위치에서 doll.jpg 파일 찾기
* `../doll.jpg` : 상위 폴더로 한 단계 나가서 doll.jpg 파일 찾기
* `../a/doll.jpg` : 상위 폴더로 한 단계 나가고 a폴더로 들어가서 doll.jpg 파일 찾기
* `./b/doll.jpg` : 현재 위치에서 b폴더로 들어가서 doll.jpg 파일 찾기
## 바로가기 링크란?
* 단순 페이지 이동이 아닌, 특정 위치로 스크롤 이동하는 바로가기 기능
## 바로가기 링크 제작 순서 및 주의사항
1. 이동 목적지에 가장 가까운 태그에 `id` 적용하기
2. 링크 대상에  `#id` href 송성값에 담기
* 주의사항 : #은 아이디 이동 링크에만 사용하기
## 파비콘 적용 순서
1. 파비콘 크기로 이미지 다운 받거나 편집하기
2. html에서 head안에 link태그로 `favicon` href 주소 연결하기
3. `href` 값에 저장해둔 파비콘 경로를 입력
## 이미지태그 `img`
* 인라인 요소
* src속성에는 이미지 경로를 입력한다 (상대경로 입력 방식)
* alt속성에는 이미지에 대한 설명을 객관적으로 입력한다
## figure, figcaption 태그 (block)
* 문서 안에 사진을 감싸는 틀로 활용
* 캡션에 사진을 정의할 수 있음
## video태그 (blcok)
* 비디오를 웹사이트에 올리는 태그 `img`태그랑 다르게 닫히는 태그가 존재
* 추가속성 없이 작성 시 정지 상태로 올라감
* `autoplay` 영상 자동 재생 값 / `muted` 영상 자동 재생 시 소리가 나지 않게 / `loop`반복 재생값 / `controls`영상 컨트롤 버튼 활성 값
* 유튜브 동영상을 가져올 경우 링크를 사용하는 것이 가벼움
* 유튜브 영상을 가져올 때 `src`안의 영상 고유 링크값 뒤에 `?autoplay`,`&mute`,`&loop`,`&controls`값들을 추가해서 설정
## class, id 많이 사용하는 키워드
* wrapper, wrap, area 전체 묶는 영역
* contents, container 중~소 묶는 영역
* group, g 간단한 소그룹 영역
* top, btm, left, right 레이아웃 방향을 의미하는 키워드
* 예 : 의미 있는 단어_영역명
* 예시 : product_wrap, item_area, price_g, main_contents, top_btn
## div, span 그룹태그
### div
* 인라인과 블록이 2개 이상 형제일 경우 묶어주는 그룹 태그
* 레이아웃 기준 1행에 2열 이상 배치일 경우
* 특정 의미를 가진 행에 같은 디자인 요소가 배치된 경우
### span
* 인라인이 2개 이상 형제일 경우 묶는 그룹 태그
* 의미 없는 디자인 요소 인라인 처리 필요 시 사용
## html5 semantic tag
### semantic tag란?
* HTML5에서 생성된 의미 있는 태그 
* 예를 들어 `<header></header>` `<nav></nav>`와 같이 작성해야 됨
### header
* 로고 및 내비게이션을 묶어주는 레이아웃 태그
* 제목, 로고, 검색 폼, 작성자, sns 등의 요소를 포함할 수 있음
### nav
* 로고 및 웹사이트 주요 내비게이션을 묶어주는 레이아웃 태그
* 다른 페이지로 가는 링크를 보여주는 구획을 나타냄
* 메뉴, 목차, 색인과 같은 곳에 자주 쓰임
### gnb, lnb, snb
* gnb(global navigation bar) - nav 묶이는 대상
* lnb (local navigation bar) 주로 서브 메뉴가 나오는 영역
* snb (side navigation bar) 보조 메뉴 영역
### section
* 문서의 독립적인 구획을 나타냄
* 제목을 자식으로 포함하는 것을 권고함
### aside
* 문서의 주요 내용과 간접적으로만 연관되는 부분을 나타냄
* 사이드바 혹은 콜아웃 박스로 표현
### article
* 사이트 안에서 독립적으로 구분해 배포하거나 재사용할 수 있는 구획을 나타냄
* 게시판, 블로그 글, 매거진, 뉴스 기사 등
* 제목(H)를 자식으로 권고하지는 않음 (section과 다른 부분)
## ul, ol, li
### ul
* 순서가 없는 목록을 묶어주는 그룹 태그
* 목록이 순서와 연관이 없을 경우 사용
* 형제 태그로 block요소 태그를 사용할 수 있지만 자식 혹은 자손으로는 사용할 수 없음
### ol
* 순서가 있는 목록을 묶어주는 그룹 태그
* 목록이 순서와 연관될 경우 사용
* 형제 태그로 block요소 태그를 사용할 수 있지만 자식 혹은 자손으로 사용할 수 없음
### li
* `ul` `ol` 의 자식으로 사용됨
* 추가로 목록을 만들고 싶을 때 `ul``ol`에 자식으로 쓰는 게 아니라 `li`의 자식으로 `ul 또는 ol` 태그를 넣어서 사용함
## details, summary
* 열림 상태일 때 내부 정보를 보여주는 정보 공개 위젯을 생성함.
* 요약이나 레이블은 `summary` 요소를 통해 제공함
* `<details><summary>`요약`</summary>`내용`</details>`
## footer, mark, main, time
* `footer` : 웹페이지 가장 하단에 위치함. 작성자, 저작권 정보, 관련문서 증의 내용을 담으며 제목 태그는 사용X
* `mark` : 맥락에 중요한 곳을 표시, 하이라이트한 부분을 나타냄
* `main` : 문서 `body`의 주요 콘텐츠를 나타내며 핵심 주제 혹은 기능에 직접적으로 연결됐거나 확장하는 콘텐츠로 이루어짐
* `time` : 시간의 특정 지점 또는 구간을 나타냄, datetime 속성을 넣어서 날짜 혹은 시간 값을 입력. 적절한 검색 결과나 특정 기능을 구현할 때 사용할 수 있음
## dl, dt, dd 정의형 목록태그
* `dl` 정의형 제목과 내용을 묶어주는 그룹 태그
* `dt` dl안의 자식으로 배치. 정의형 목록 태그의 제목을 의미함. `dd`의 앞에서 먼저 시작함
* `dd` dl안의 자식으로 배치. 정의형 목록 태그의 내용을 의미함. `dt`의 다음 형제 요소로 배치되거나 기존 `dd`의 형제로도 배치 가능
* 다른 태그와 조합 시 제목 또는 내용의 위치에 따라 `dt` `dd`안에만 추가 태그가 들어갈 수 있음
