---
layout: page
title: Projects
subtitle: 2022
share-img: /assets/img/aboutme.jpg
cover-img: /assets/img/bb.jpg

---

<br>

## 뉴얼스 (NewEarth)

<br>

### 팀 이름
<b>팀 이름 : 뉴얼스</b><br>
올해 데뷔한 하이브 걸그룹 '뉴진스'에서 영감을 받아 지었다.

<br>

### 프로젝트 배경
요즘 환경 오염과 관련된 이슈들이 계속 발생하고 있다. 사람들이 환경오염에 대한 자각은 하고 있지만, 구체적으로 어떠한 환경 문제가 발생하고 있는지 모르고, 환경 보호를 위해서도 어떠한 행동을 실천해야 하는지 모르고 있다. 
이러한 이유로 환경 오염에 대한 심각성과 구체적인 환경 보호에 대한 방법을 알려주는 웹 사이트를 구상하게 되었다.
그냥 정보를 알려주는 사이트는 식상하고, 접근성이 적을 것 같아서 지구와 세계를 그래픽적으로 표현하는 것을 기획하였다.

<br>

### 목표 및 필요성

- 환경 오염에 자각이 없는 사람들에게 환경 오염의 심각성을 알려준다.
- 투두 리스트를 제공해서, 환경 보호를 실천하도록 장려한다.
- 구체적인 환경활동을 제공한다.
- 환경 보호에 쉽게 접근할 수 있도록 실천 목록과 정보를 제공한다.
- 전세계의 자원 사용량을 시각적으로 제공하여 환경 오염의 심각성을 뚜렷하게 파악할 수 있도록 한다.

<br>

### 내 역할<br>
1. 환경일지 디자인 및 파이어베이스<br>
2. 환경보호방법 디자인 및 파이어베이스

<br>

### User Interface
<br>
#### 1. 시작 페이지<br>
- js 3D 라이브러리인 Three.js를 사용하여 돌아가는 지구본을 구현<br>
- 지구본 클릭 시 세계지도 페이지로 이동<br>
![Pro](/assets/img/newearth/1.PNG)

<br>

#### 2. 세계지도 페이지
<br>
- html, css, javascript를 이용해서 세계지도 페이지 구현.<br>
- 이미지맵을 사용하여 지역을 설정하고 지역에 마우스오버 시 깃발애니메이션이 발생하게 구현.<br>
- 지역 클릭 시 관련 환경오염 정보 팝업창이 나타나게 구현.<br>
- 세계지도페이지 우측상단에 위치한 버튼을 이용해 커뮤니티 페이지로 이동가능.
<br>

![Pro](/assets/img/newearth/2.PNG)
<br>

![Pro](/assets/img/newearth/3.PNG)
<br>

![Pro](/assets/img/newearth/4.PNG)
<br>

![Pro](/assets/img/newearth/5.PNG)

<br>

### 3. 커뮤니티 페이지

<br>
- Google 로그인 기능 제공 --> firebase Auth 사용.<br>
- uid를 이용해 사용자 데이터 저장.<br>
- firebase Cloud Firestore를 이용해 데이터 베이스 저장.

<br>

<b>3 – 1. 환경일지 및 환경보호방법</b>

<br>

- html, css, javascript를 이용해서 페이지 구현.<br>
- 상단의 버튼을 통해 환경일지, 환경보호방법 페이지로 이동가능.<br>
- [작성하기] 버튼을 눌러 글 작성 가능.<br>


![Pro](/assets/img/newearth/6.PNG)<br>
![Pro](/assets/img/newearth/7.PNG)<br>

<b>3 – 2. 환경 발자국 및 to do list</b><br>

- html, css, javascript를 이용해서 페이지 구현.<br>
- 날짜에 맞는 밭구역을 클릭하면 그 날짜의 to-do-list 페이지 이동가능.<br>
- to-do-list 달성에 따라 ‘씨앗-새싹-줄기-꽃’ 으로 성장가능.<br>

![Pro](/assets/img/newearth/9.PNG)<br>
![Pro](/assets/img/newearth/8.PNG)<br>


### 수행 코드

<br>

<b>[index.html]</b><br>
- 카메라를 세팅(0,0,15)<br>
- SphereGeometry(5,32,16)위에 (“./imgs/globe.PNG”)를 입힘.<br>
- y축을 기준으로 돌아갈 수 있게 애니메이션 설정.


<br>
![co](/assets/img/newearth/01.PNG)

<br>

<b>[globe.js]</b>

<br>

![co](/assets/img/newearth/02.PNG)

<br>

![co](/assets/img/newearth/03.PNG)

<br>

<b>[worldmap.html]</b>

<br>

![co](/assets/img/newearth/04.PNG)

<br>

<b>[worldmap_hover.js]</b>

<br>

- 이미지맵을 통해 구역을 설정하고 그 구역에 마우스를 오버하면 display=none; 상태인 깃발이 보이게 자바스크립트 이벤트 함수를 설정.

<br>

![co](/assets/img/newearth/05.PNG)

<br>

<b>[worldmap.html]</b><br>

- style태그와 연결된 css(class태그) 로 모달창 구현.<br>
- html에 모달창에 나타날 환경오염정보 입력.
<br>

![co](/assets/img/newearth/06.PNG)

<br>

<b>[worldmap_markclick.js]<b><br>

- 구역(‘mark’) 클릭 시 모달창(‘modal’) 나타나게 설정.

<br>

![co](/assets/img/newearth/07.PNG)

<br>

![co](/assets/img/newearth/08.PNG)

<br>

<b>[firebase.js]</b><br>

- Google 로그인 연동

<br>

![co](/assets/img/newearth/09.PNG)

<br>

<b>[todolist_env_step.html]</b><br>

- Todolist 목록 DB에 저장하기, 불러오기

<br>

![co](/assets//img/newearth/010.PNG)

<br>

<b>[communityUI_환경보호방법작성.html]</b><br>

- 환경보호방법 작성 데이터를 이미지와 함께 DB에 저장하기

<br>

![co](/assets/img/newearth/011.PNG)

<br>

![co](/assets//img/newearth/012.PNG)

<br>

<b>[communityUI_환경보호방법목록.html]</b><br>

- 환경일지 목록  DB에서 불러오기

<br>

![co](/assets/img/newearth/013.PNG)

<br>

<b>[communityUI_환경일지작성.html]</b><br>

- 환경일지 작성 데이터 이미지와 함께 DB에 저장하기

<br>

![co](/assets/img/newearth/014.PNG)

<br>

![co](/assets/img/newearth/015.PNG)

<br>

<b>[communityUI_환경일지목록.html]</b><br>

- 환경일지 목록 DB에서 불러오기

<br>

![co](/assets/img/newearth/016.PNG)

<br>

<b>[communityUI_환경보호방법목록.css]</b>
<br>

![co](/assets/img/newearth/017.PNG)

<br>

![co](/assets/img/newearth/018.PNG)

<br>

<b>[content_env_step.js]</b>

<br>

- 밭 구역에 씨앗들 구현

<br>

![co](/assets/img/newearth/019.PNG)

<br>

<b>[content_env_step.js]</b><br>

- 클릭 이벤트 설정 (to-do-list 페이지로 이동)

<br>

![co](/assets/img/newearth/020.PNG)

<br>

<b>[todolist_env_step.html]</b>

<br>

- to-do-list 달성에 따라 ‘씨앗-새싹-줄기-꽃’ 으로 성장하능하게 설정

<br>

![co](/assets/img/newearth/021.PNG)

<br>

![co](/assets/img/newearth/022.PNG)

<br>

### 기대효과 및 활용방안<br>

- 환경 문제에 대한 정보를 그래픽적으로 제공해주어, 아이들을 포함해 글을 읽기 싫어하는 사람들에게 지루하지 않은 교육용 정보로 제공할 수 있다.<br>
- 환경 보호 활동에 대한 개인과 단체의 실천을 기대할 수 있다.<br>
- 나무 위키를 응용하여 전 세계 사람들이 자국의 나라에서 일어나는 환경문제에 대한 실시간 정보를 작성할 수 있도록 해, 환경 문제용 나무위키로 발전할 수 있도록 한다.











