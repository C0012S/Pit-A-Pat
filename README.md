# Pit-A-Pet

<div align="center">
  <img src="https://github.com/B2-O2/Pit-A-Pet/assets/66476874/513fae16-e775-4a1e-8a31-d0d5b073d76a">
  <br/>
  <p>https://b2-o2.github.io/Pit-A-Pet/main.html</p>
</div>

<br/>
<br/>

## 개요

### 기획 및 개발 배경

팀원 모두 동물을 좋아하거나 반려동물을 키운다는 공통점을 가짐  
동물을 좋아하고, 동물이 삶에 밀접하게 관련이 있는 사람들을 타깃으로 **반려동물 또는 자신이 좋아하는 동물을 소개하는 블로그 형식의 반응형 웹 페이지 Pit A Pet** 제작

<br/>

### 블로그 형식의 웹 페이지

동물과의 소중한 기억 또는 유용한 정보를 공유하기 위해서 네이버 블로그, 벨로그, 티스토리 등 자유롭게 글을 작성할 수 있는 블로그 형식으로 각자의 개성을 살린 반응형 블로그 페이지 구현

<br/>

### Pit A Pet의 의미?

‘두근두근’의 의미를 가진 ‘Pit A Pat’과 ‘반려동물’을 의미하는 ‘Pet’과 합쳐 반려동물과 함께라면 심장이 두근거린다는 의미의 단어를 만들어 해당 프로젝트의 프로젝트명으로 결정

<br/>
<br/>

## 역할

| 이름   | 개발 파트               | 파일명                                    |
| ------ | ----------------------- | ----------------------------------------- |
| 박상희 | 본인 블로그 상세 페이지 | sh_detail.html, sh_detail.css, sh_detail.js |
| 박진은 | 메인 페이지             | main.html, main.css, hambuger.js         |
| 안정민 | 본인 블로그 상세 페이지 | jeongmin_detail.html, jeongmin_detail.css |
| 이수빈 | 본인 블로그 상세 페이지 | subin_detail.html, subin_detail.css       |

<br/>

### 박상희

- 오븐을 이용한 본인 블로그 상세 페이지 와이어프레임 작성
- 피그마를 이용한 본인 블로그 상세 페이지 프로토타입 작성
- 프로젝트명 결정
- 로고 디자인
- 마지막 디자인 점검 및 수정
- 폴더 구조 관리
- 프로젝트 개요 작성
- 전반적인 README 작성
- 전반적인 GitHub 관리
- 배포

<br/>

#### Trouble Shooting

- Trouble  
  : 데스크탑과 태블릿 화면에서는 프로필 메뉴 영역과 블로그 영역을 한번에 같이 볼 수 있도록 했고, 모바일 화면에서는 블로그 영역만 보이게 하고 왼쪽 상단에 메뉴 버튼을 만들어 클릭 시 프로필 메뉴를 볼 수 있게 만들었다.
  그런데 프로필 메뉴 영역과 블로그 영역을 같은 div 태그 내에 작성해서 메뉴 버튼 클릭 시 프로필 메뉴가 블로그 영역 위로 보이는 게 아니라 블로그 영역과 같은 영역에 삽입되어 보이는 문제가 있었다.

<br/>

- Shooting  
  : 모바일 화면에서 메뉴 버튼을 클릭했을 때, 프로필 메뉴 영역이 화면에 보일 때는 position 값을 absolute로 지정함으로써 해결했다.  
  그리고 데스크탑 화면과 태블릿 화면에서는 position 값을 기본값인 static으로 다시 지정해 줌으로써 데스크탑 화면과 태블릿 화면의 CSS 값이 모바일 화면의 CSS 값을 덮어쓰지 않도록 했다.

<br/>

### 박진은

- 수빈과 정민이 작성한 메인 페이지의 와이어프레임 요소를 합쳐 메인 페이지의 데스크탑, 태블릿, 모바일 버전의 와이어프레임 작성

<br/>

#### Trouble Shooting

- Trouble  
  : 모바일 버전을 제작하면서 중첩된 div 태그 구조에서 자식 div에 margin-top을 주었다. 그런데 부모 div에 margin-top이 적용되어 원하는 view 생성이 어려웠던 상황이 있었다.

<br/>

- Shooting  
  : 이러한 현상이 부모 블록에 테두리, 패딩 등이 없고 별도의 min-height, max-height 등이 설정되지 않은 경우, 자식의 margin-top은 부모의 margin-top으로 적용되는 margin collapse 현상임을 뒤늦게 인지하고 부모의 div에 padding과 border 1px를 주어서 해결할 수 있었다.

<br/>

### 안정민

- 오븐을 이용한 본인 블로그 상세 페이지 와이어프레임 작성
- 자동 슬라이드 애니메이션 코드 제공
- 마지막 디자인 점검 및 수정
- 프로젝트 개요 작성
- 와이어프레임 취합 및 피드백
- PPT 제작

<br/>

#### Trouble Shooting

- Trouble  
  : 첫 화면에서 나타나는 배경 이미지 위에 부드럽게 본문이 올라오는 방식을 JavaScript 없이 CSS만으로 해결해야 하는 문제가 있었다. 그리고 배경 이미지가 데스크탑, 태블릿, 모바일 화면에서 모두 같은 시작 위치에서 시작하면 모바일에선 배경 이미지의 끝 부분만 보이는 문제가 있었다.

<br/>

- Shooting  
  : JavaScript를 사용하는 대신 배경 이미지와 커버의 position을 fixed로 맞춘 뒤 본문의 z-index를 배경 이미지보다 높게 설정하여 구현하는 것으로 해결하였다. 또한 배경 이미지의 위치도 반응형 모니터에 맞게 위치를 각각 수정해 줌으로써 해결하였다.

<br/>

### 이수빈

- 오븐을 이용한 본인 블로그 상세 페이지 와이어프레임 작성
- 메인 페이지 로고 및 카드 텍스트 정렬
- 마지막 디자인 점검 및 수정

#### Trouble Shooting

- Trouble
  : 로드시 로딩 스크린 개발 이후 타 요소 애니메이션 적용 시 DEFAULT 0초에 적용되어 애니메이션이 적용되지 않는 것처럼 보이는 문제
- Shooting  
  : 애니메이션 요소 시작시간 설정
<br/>
- Trouble
  : JavaScript를 사용하지 않고 반응형 게이지바 구현
- Shooting  
  : 2개의 div를 사용하여 겹친 후 width를 부모요소에 적용하고 애니메이션을 적용하여 구현, margin을 vw로 주어 각 요소의 height와 무관하게 반응형으로 구현
<br/>

### Together

- 기획
- 발표 내용 구성
- 발표
