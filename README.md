<img src="./assets/main.gif">

## 📋 프로젝트 개요

> **프로젝트명** : 크롬앱 <br/> > **개발 기간** : 2022년 10월 1일 ~ 2022년 10월 14일 (2주) <br/> > **분류** : 개인 프로젝트 <br/> > **역할 및 기여도** : UI/UX 디자인 및 개발 100%<br/> > **사용 기술** : `HTML`, `CSS`, `JavaScript`

<br/>
<br/>
<br/>

## 🔍 프로젝트 소개

노마드 코더의 ['바닐라 JS로 크롬 앱 만들기'](https://nomadcoders.co/javascript-for-beginners) 강의를 수강한 후 만든 프로젝트입니다.
강의에서 구현하는 내용 외에 기능을 추가하였고 직접 Figma를 사용해 UI를 디자인하여 진행했습니다. 강의 내용에 더해 추가한 기능들은 아래와 같습니다.
<br/>
<br/>
<br/>

## ✨ 결과물

#### 배포 링크

[https://angie-momentum.vercel.app/](https://angie-momentum.vercel.app/)
<br/>
<br/>
<br/>

## 👩🏻‍💻 기술 스택

- `HTML`, `CSS`, `JavaScript`
  <br/>
  <br/>
  <br/>

## 💡 주요 기능

1. 북마크

   - 북마크 추가
   - 북마크 삭제
     - 북마크 수정

2. 투두리스트

   - 카테고리 태그 추가
   - 카테고리 태그 삭제
     - 할일을 추가할 때 카테고리 태그 선택
     - 태그가 있는 할일, 태그가 없는 할일 모두 추가 가능
     - 카테고리가 추가된 할일은 리스트에 태그 보이기

3. 음악 플레이어 (iframe API 사용)

   - 유튜브 URL로 음악 추가
     - 플레이리스트 상의 음악 삭제
     - 플레이리스트 상의 음악 클릭하면 해당 음악 재생
     - 현재 재생 중인 음악 표시
     - 음악 재생 및 일시정지
     - 이전 곡, 다음 곡 재생

4. 날씨

   - 4일 동안의 날씨 예보

5. 랜덤 명언 - 새로고침 시 랜덤으로 영어 명언 표시
   <br/>
   <br/>
   <br/>

## 🌃 기능 상세 및 실제 화면

#### 투두리스트

<img src="./assets/todolist.gif">

투두리스트의 +버튼을 누르면 버튼이 입력창(form)으로 바뀌는 애니메이션을 구현했습니다. 각각 다른 높이를 지정할 수 있는 클래스를 CSS에서 정의하여 버튼 클릭시 더 큰 높이를 지정하는 클래스를 추가햤습니다. CSS에서 transition을 설정하여 애니메이션을 구현했습니다.

할일을 추가하는 입력창 안에서 카테고리 태그를 추가할 수 있는 form을 넣었습니다. html 구조 상 form안에 form을 넣을 수 없기 때문에 CSS에서 position을 absolute로 하여 할일 추가 form 안에 있는 것처럼 보이도록 했습니다.
<br/>

#### 음악 플레이어

<img src="https://velog.velcdn.com/images/94applekoo/post/d068176d-85b5-4dd4-8449-f8150bb52692/image.gif">

유튜브 영상의 URL을 입력하면 URL에서 정규표현식으로 영상 id를 받아왔습니다. 영상 id로 유튜브 영상 ID, 영상 제목, 썸네일 URL을 가져와 로컬 스토리지에 저장하고 각각 플레이리스트에 보여질 수 있게 했습니다.

플레이리스트에서 현재 재생되고 있는 음악을 표시하도록 했습니다. 음악을 선택하면 해당 영상의 id로 로컬 스토리지의 값을 업데이트하고, 각 음악의 id가 현재 재생 중인 영상의 id와 같으면 하이라이트하는 CSS 속성을 가진 클래스가 추가되도록 했습니다.
<br/>

#### 북마크

<img src="https://velog.velcdn.com/images/94applekoo/post/2eae8b63-d0eb-4f0a-adbc-bd83b1d37405/image.gif">

음악 플레이어와 마찬가지로 +버튼을 누르면 버튼이 입력폼으로 변화하는 애니메이션을 구현했습니다. 북마크 링크의 입력이 완료되면 해당 링크의 생성과 동시에 입력폼이 버튼으로 되돌아가는 애니메이션을 구현했습니다.
<br/>
<br/>
<br/>

## 💭 프로젝트 회고

### 나의 고민들

> 효율적이고 가독성이 높은 코드란?

변수명과 클래스명을 어떻게 하면 가독성있게 작성할 수 있을지에 대한 고민을 하기 시작했다. 내 생애 처음으로 '코드'로 이루어진 프로젝트이기 때문에 **일단 어떻게든 만들어내는 것이** 목표였다. 그래서 맨땅에 헤딩하는 기분으로 다소 주먹구구식으로 코드를 짰기 때문에 기능이 더해질수록 코드가 지저분해지는 걸 느꼈다.
<br/>

> 그래서 다음 프로젝트에선?

이러한 경험을 통해 다음 프로젝트에선 기능별로 CSS 파일을 분할하고 **BEM** 규칙에 지켜 가독성 있게 클래스명을 쓰고자 한다!
<br/>

> 기능적인 구조를 먼저 생각해보자

필요한 기능을 먼저 리스트업하고 그에 따라 코드 구조를 먼저 생각했으면 좋았을 것 같다. 음악 플레이어 구현시 다양한 경우의 수(음악 재생 중에 음악을 삭제하는 경우, 음악이 재생되는 중에 모든 음악이 삭제되는 경우 등...)를 고려해야했는데, 코드를 짤수록 다양한 변수들을 맞이하며 코드 구조가 뒤죽박죽되는 경험을 했다. 무작정 키보드를 두들기기 보다는 전체적인 구조를 먼저 고민하고 코드를 작성하면 좋을 것 같다.
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
