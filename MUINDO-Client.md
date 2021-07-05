# MUINDO - Client



## ⚙ 기술 스택

+ Language :  **Javascript**, **HTML5**, **CSS3**
+ Library : **React**,  **Redux**, **styled-Compoent**, **axios**, **Firebase-auth**
+ UI Framework : **Material-UI**
+ Code Tools :  **ESLint**, **Prettier**
+ Tools : **Git**, **Github**, **Gitlab**, **Notion**, **Discord**, **Figma**
+ Environment : **npm**, **CRA(Create React App)**



## 📂 폴더 구조

```bash
│── client/			- 클라이언트 루트 디렉터리
│   |── public/
│   |   |── images/		- 클라이언트사이드 이미지 디렉터리
│   |   |── index.html		- root index.html
│   |
│   |── src/				
│   |   |── actions/		- 액션 정의
│   |   |── reducers/		- 리듀서 정의
│   |   |── components/	        - 페이지별 컴포넌트 디렉터리
│   |   |── pages/		- 페이지 디렉터리
│   |   |── url/		- root API URL 디렉터리 
│   │   │── App.css		- root css
│   |   |── App.js		- root route js 
│   |   |── index.js		- root index js
│   │
│   │── .env		        - 외부 API 키 저장
│   │── firebase.json		- firebase 설정
│   │── .prettierrc		- prettier 설정파일
│   │__ package.json		- npm 설정
│
│── README.md		        - 리드미 파일
```



## 📄 실행 스크립트

```bash
cd client
npm i	// node_module 설치

npm run start	// for run
npm run build	// for build
```



## 개선사항

**Ver 2.0**

+ useContext 기반 State 관리 👉 Redux 기반 State 개편

  > ( 유지님 부탁좀..^^ )

+ 사용자 친화적 UX 개선 ( 컨펌하기 & 컨펌받기 )

  > Ver.1 에서 비교적 짧은 시간내에 구현에 급급해서 놓쳤던 부분을 수정했습니다.
  >
  > +  전체적인 UI 통일성을 수정했습니다.
  >   + 예를 들어, 마이페이지의 기능을 담당하는 버튼의 구성을 통일 시키고, 회원과 비회원이 사용할 수 있는 기능을 UI적으로 구분되도록 배치시켰습니다
  >   + 컨펌받기의 경우, 특정 기능에 구분을 위해 Border 사용에 대해 과함이 있었는데, 유저입장에서 의도치 않은 답답함을 유발할 수 있다는 판단하에 Border 사용을 줄이고, 해당 컨텐츠에 전체적인 UI적 안정감을 맟췄습니다.
  >   + 컨펌하기의 경우, Confirm 과 Nope 버튼을 emoji 를 사용했었는데, OS에 따른, emoji 버튼의 형태 차이가 발생하는 것을 확인해서, 저희 컨텐츠에 좀 더 어울리는 icon 컴포넌트를 커스텀해서 사용해서 해당 문제를 해결했습니다.
  >     또한, 타인의 특정 패션 룩 이미지를 나의 옷장에 저장하고 싶을 때, 사용가능한 찜하기 버튼의 위치가 UI 해상도마다 위치가 무분별하였는데, 이는 룩 이미지의 좌측상단에 고정하는 것이 좋다고 판단하여 수정했습니다.

+ 컨텐츠 추가 : 스타일 솔루션

  > 기존 Ver.1 에서의 메인기능은 크게 2가지였습니다.
  >
  > + **1. 컨펌하기** : 타 유저들이 등록한 패션 룩이미지를 Confirm OR Nope 으로, 평가를 해주는 컨텐츠
  > + **2. 컨펌받기** : 본인이 컨펌을 받기위해, 패션 룩이미지를 등록하는 컨텐츠
  >
  > 이에 추가하여, 컨펌받기 등록이후, 특정 Confirm 포인트를 지속적으로 받지 못한 유저의 경우, 평균적으로 호감적인 가이드 패션 스타일 룩을 본인의 스타일 취향기반 사전조사를 통해 추천받을 수 있는 **3. 스타일 솔루션** 컨텐츠를 추가하게 되었습니다. 



## 배운점
