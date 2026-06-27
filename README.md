# Movie App 2021

노마드 코더(Nomad Coders) **「ReactJS로 영화 웹서비스 만들기 (React JS Fundamentals)」** 강의를 따라 만든 React 학습용 프로젝트입니다. (2021 Update 기준)

## 출처 (강의 정보)

- **강의명:** ReactJS로 영화 웹서비스 만들기 (React JS Fundamentals Course)
- **제공:** 노마드 코더 (Nomad Coders) — https://nomadcoders.co/
- **수강 시기:** 2021년
- **학습 형태:** 강의 챕터별로 커밋을 남기며 따라 만든 클론 코딩 프로젝트

## 소개

React의 기초 개념(컴포넌트, JSX, Props, State, 컴포넌트 생명주기, API 데이터 페칭)을 단계별로 학습하기 위한 토이 프로젝트입니다. [YTS](https://yts.mx/) 영화 API를 호출해 영화 목록을 받아오는 것을 목표로 합니다.

## 기술 스택

- React 17 (Create React App 기반)
- axios — HTTP 요청
- prop-types — 컴포넌트 props 타입 검증

## 실행 방법

```bash
npm install
npm start      # 개발 서버 실행 (http://localhost:3000)
npm run build  # 프로덕션 빌드
```

## 학습 진행 단계

커밋 단위로 강의 챕터를 따라가며 진행했습니다.

| 단계 | 내용 |
| --- | --- |
| #1 | Create React App 초기화 / 첫 실습 |
| #2.4 | Prop-Types로 props 타입 검증 |
| #3.0 | Class 컴포넌트와 State |
| #3.1 | State 다루기 |
| #3.2 | 컴포넌트 생명주기 (Component Life Cycle) |
| #3.3 | Movie 컴포넌트 설계 |
| #4.0 | API에서 영화 목록 가져오기 (async / await) |

## 현재 상태

- `#4.0` 단계까지 진행됨
- `componentDidMount`에서 YTS API(`https://yts-proxy.now.sh/list_movies.json`)를 호출하기 시작한 단계
- 받아온 데이터를 화면에 렌더링하는 단계 이전이라, 현재 화면에는 로딩 상태("Loading...")만 표시됨

> 참고: 이 프로젝트에서 사용하는 `yts-proxy.now.sh` 프록시는 현재 동작하지 않을 수 있습니다. 이어서 진행하려면 최신 YTS API 엔드포인트로 교체가 필요합니다.
