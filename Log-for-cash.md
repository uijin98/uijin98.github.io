---
layout: page
title: Projects
subtitle: 2022
share-img: /assets/img/aboutme.jpg
cover-img: /assets/img/bb.jpg

---

# Log for Cash

<br>

## 블록체인 기반 설문 리워드 및 데이터 NFT 거래 플랫폼

<br>

## 내 역할<br>
- DB에 올라가는 정보 암호화 및 설문 항목 데이터 저장

<br>

## 프로젝트 개요<br>
의뢰자는 설문을 의뢰하고, 응답자는 응답하여 보상받는 설문형 앱테크 플랫폼.<br>
완성되는 데이터는 NFT로 발급되어 제3자간 거래되며, 그에 대한 로열티가 다시응답자에게 돌아옴.

<br>

## 프로젝트 목표<br>
1. 블록체인(솔라나)을 기반으로 한 스마트 컨트랙트로, 설문 의뢰 및 보상 시스템을 투명하게 제공.<br>
2. 종료된 설문조사 데이터를 NFT로 민팅<br>
3. 민팅될 NFT의 지분을 정하고, 응답자에게 나눈 비율만큼 설문 의뢰비용 할인

<br>

## 프로젝트 내용

<br>

띄우는 서버 2개 : express(api 서버), DB(mysql)
<br>

본 플랫폼은 node js의 미들웨어 백엔드 프레임워크 express js로 구현되었음.
<br>

하나의 노드에 express로 구현된 api 서버와 mysql 서버를 띄움.
프론트 엔드는 따로 존재하지 않으며. express js에서 제공하는 view engine을 통해 프론트엔드 역할도 같이 처리

![Log](/assets/img/LogforCash/1.PNG)
<br>

1. view engine은 ejs 옵션으로 설정되어있으며, html파일이 ejs라는 확장자로 작성된다.<br>
2. ejs 파일에서는 api서버단의 변수를(DB값 등) 넘겨주어 사용할 수 있다.<br>
3. ejs에서는 js로 반복문, 조건문 처리도 가능하다.<br>
4. 즉, express가 ejs파일의 ejs문법을 서버단에서 처리하고 알아서 html 파일로 변환하여 유저에게 보여준다. (동적 서버 구현 가능) 

<br>

## 모듈<br>
모든 모듈의 기본 동작

<br>

![Log](/assets/img/LogforCash/2.PNG)
<br>

<b>1. User 생성, 인증 관련 모듈</b><br>

![Log](/assets/img/LogforCash/3.PNG)
<br>

![Log](/assets/img/LogforCash/4.PNG)

<br>

<b>2. 설문 관련 모듈</b><br>

![Log](/assets/img/LogforCash/7.PNG)
<br>

![Log](/assets/img/LogforCash/8.PNG)

<br>

<b>3. NFT 관련 모듈</b><br>

![Log](/assets/img/LogforCash/12.PNG)
<br>

![Log](/assets/img/LogforCash/13.PNG)