## aicc project team2
> 프로젝트 소개
> - team1로부터 의뢰받은 runnging app을 개발
> - 회원가입 후 러닝코스를 등록하고 다른사람과 공유할 수 있는 웹
> - 2030세대에서 러닝에 대한 관심도가 꾸준히 증가하고 있으며 온라인 커뮤니티도 자주 방문하는 세대이므로 2030을 타겟으로 개발한 프로젝트
> - 프로젝트 개발 기간: 2주

---

### 1. 팀소개
- 팀장
  - kakao map api를 이용하여 맵과 관련된 핵심 기능들을 구현
  - 의뢰받은 팀과의 커뮤니케이션, 조율 등 프로젝트 전반을 관리
  - [팀장 깃헙](https://github.com/Noveled)
  - [팀장의 블로그](https://siina.tistory.com)
- 팀원1(본인)
  - 로그인, 로그아웃 기능 구현
  - 추천코스, 보관함 기능 및 UI 구현
  - [나의 블로그](https://velog.io/@homeless_snail/posts)
- 팀원2
  - 마이페이지 구현
  - 프로젝트의 전반적인 디자인 구성
  - [팀원2의 깃헙](https://github.com/mjk2024-dementia)

---

### 2. 프로젝트에 사용한 기술
<img src="https://img.shields.io/badge/JavaScript-black?style=for-the-badge&logo=JavaScript&logoColor={로고 색깔}"/> <img src="https://img.shields.io/badge/React-black?style=for-the-badge&logo=react&logoColor={로고 색깔}"/><br>
<img src="https://img.shields.io/badge/Node.js-black?style=for-the-badge&logo=nodedotjs&logoColor={로고 색깔}"/><br>
<img src="https://img.shields.io/badge/PostgreSQL-black?style=for-the-badge&logo=postgresql&logoColor={로고 색깔}"/>

---

### 3. 기능
- 본인이 작성한 코스 CRUD 기능
- 다른사람이 등록한 코스 확인 가능
- 본인 코스를 다른사람이 볼 수 없도록 비밀코스로 설정 가능
- 지역별 거리별 등 추천코스 확인 가능
- 본인 위치 주변 물품보관함, 버스정류장 등 편의시설 위치 제공

---

### 4. 추후 업데이트 기능
- 좋아요 기능 추가: 다른사람 코스에 좋아요 버튼을 클릭하면 보관함(즐겨찾기)에서 확인가능
- 검색기능 추가: 제목, 위치, 코스 설명 내용을 바탕으로 검색 기능 구현

---

### 5. 프로젝트 배포
- [프로젝트 배포 사이트(Running Hi)](https://aiccrunningapp.microdeveloper.co.kr)
- [배포과정 정리](https://velog.io/@homeless_snail/deploy-process1)

---

### 6. 시작 가이드
- 요구사항
  - node 20.15.1
  - npm 10.7.0
- 설치
```shell
git clone https://github.com/sonjuhyeon/aicc-team-pjt-running-app-front.git
```
- front-end
  - 루트 디렉토리에 .env 파일을 생성
  - 아래 환경변수 내용을 입력
```
REACT_APP_MAP_KEY = <카카오 맵 api key>
REACT_APP_MY_DOMAIN = "http://localhost:8080"
```
```shell
npm install
npm start
```
- back-end
  [back-end github으로 이동 후 시작 가이드 참고](https://github.com/sonjuhyeon/aicc-team-pjt-running-app-back)

---

### 7. 아키텍쳐
- Components Structure
<img width="934" alt="Components_Structure" src="https://github.com/user-attachments/assets/41dcf8cd-f0f8-4e2a-a3ed-67a6fbaf3675">

---

### 8. 수정해야할 사항
- 근처추천코스 -> 현재위치를 기준으로 출발지와 가까운 순으로 정렬
- 지역추천코스 -> 조회수 순으로 정렬
- 산책추천코스 -> 3km 미만, 조회수 순으로 정렬

---

### 9. 버그 및 디버그
- 코스 수정 시 거리가 0km로 초기화 됨
- 코스 thumbnail을 변경하고 싶을 때 waypoint를 다시 찍어야 thumbnail이 변경 됨
- 브라우저 창에서 뒤로가기나 앞으로 가기 할 때 하단 내비게이션 적용 안됨

---

### 기타문서
