# Weekly Review

## Service Topic
여행 계획을 관리할 수 있는 **My Travel List**를 제작했습니다.  
가고 싶은 여행지와 여행 날짜, 기간, 비용 등의 정보를 확인하고 추가하거나 수정할 수 있도록 구성했습니다.
## Data Fields
총 8개의 데이터 Field를 사용했습니다.
여행지 이름 : 여행할 장소의 이름
국가 : 여행지가 위치한 국가
도시 : 여행할 도시
여행 날짜 : 여행을 시작하는 날짜
여행 기간 : 여행하는 기간
여행 목적 : 관광, 휴식, 음식, 쇼핑 등의 여행 목적
예상 비용 : 여행에 필요한 예상 금액
방문 상태 : 방문 예정 또는 방문 완료 상태
## List Page
index.html에서는 여행지 목록을 Table 형태로 만들었습니다.
목록에는 다음 항목을 표시했습니다.
번호  
여행지 이름  
국가  
여행 날짜  
여행 기간  
방문 상태  
여행지 이름을 누르면 상세 페이지인 view.html로 이동하고, Add 버튼을 누르면 add.html로 이동하도록 만들었습니다.
## Validation
add.html과 edit.html의 Form에 HTML Validation을 적용했습니다.
`required` : 필수 항목을 입력하도록 설정
`minlength` : 여행지와 도시 이름의 최소 글자 수 설정
`maxlength` : 입력할 수 있는 최대 글자 수 설정
`min`, `max` : 여행 기간과 예상 비용의 입력 범위 설정
`type="date"` : 여행 날짜를 날짜 형식으로 입력
`select` : 여행 목적, 방문 상태를 선택하도록 구성
## RWD
Bootstrap Grid와 Media Query를 이용해서 Desktop과 Mobile 화면에 맞게 구성했습니다.
Desktop에서는 Form을 2열로 표시하고, 화면이 작아지면 1열로 표시되도록 했습니다.  
또한 `table-responsive`를 사용해서 Mobile에서도 Table의 내용을 확인할 수 있도록 했습니다.
## Bootstrap
이번 과제에서 사용한 주요 Bootstrap Class는 다음과 같습니다.
`container`
`row`
`col-md-6`
`navbar`
`table`
`table-responsive`
`form-control`
`form-select`
`btn`
`card`
`badge`

## Problem & Solution
처음에는 아무것도 없는 상태에서 구조를 생각하고 디자인을 어떻게 해야할지 막막했지만 ai를 이용해서 만들고 그것을 따라 하는 방식으로 하니 더 편하고 빠르게 할 수 있었지만, 아직 기획을 하는 단계가 보족함을 느꼈습니다. 처음에는 여러 HTML 페이지를 만들면서 각 페이지의 디자인을 비슷하게 만드는 것이 어려웠습니다.  
공통적인 디자인은 my.css에 작성하고 Bootstrap의 같은 Class를 사용해서 페이지들의 디자인을 통일했습니다.
또한 Table의 내용이 많아지면 Mobile 화면에서 화면 밖으로 넘어가는 문제가 있어서 Bootstrap의 `table-responsive`를 사용했습니다.
## Reflection
이번 과제를 하면서 코딩을 시작하기 전에 페이지의 구조와 영역을 먼저 생각하는 것이 중요하다는 것을 알게 되었습니다.
Bootstrap을 사용해보면서 CSS를 직접 전부 작성하지 않아도 Form, Button, Table 등을 쉽게 만들 수 있다는 것도 알게 되었습니다.
아직 Bootstrap의 Class 이름이나 몇몇 용어들이 익숙하지 않아서 코드를 작성할 때 헷갈리는 부분이 있습니다. 
또한, Bootstrap안에서 제가 찾고 싶은 스타일을 일일이 찾는 것도 어느 정도 시간이 걸렸습니다.
앞으로 수업을 들으면서 자주 사용하는 Class와 웹페이지의 구조를 빨리 익히고 싶습니다.