# 안녕하세요, 련입니다 👋

**데이터의 흐름과 정확성을 끝까지 검증하는 백엔드 개발자**를 목표로 하고 있습니다.
응용수학을 전공한 뒤 KB IT's Your Life 부트캠프(고용노동부 K-Digital Training)에서 Java/Spring, Vue.js 기반 풀스택 개발을 익혔고,
최종 프로젝트 **홀가(家)분**으로 **최우수상**을 받았습니다.

---

## 🏆 Highlights

- 🥇 **KB IT's Your Life 최종 프로젝트 최우수상** (2026.08)
- ⚡ 매물 11만 × CCTV 37만 건 공간 연산을 격자 기반 후보 축소로 **약 76배 단축** (약 52분 → 약 41초)
- 🧮 취득세·중개보수 계산을 **법령 기준으로 백엔드에 구현**, 심플택스와 **원 단위 교차검증** + 경계값 **단위 테스트** 고정
- 🎓 경성대학교 응용수학과 졸업 (단과대 수석)

## 🛠️ Tech Stack

![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/Spring-6DB33F?style=flat-square&logo=spring&logoColor=white)
![MyBatis](https://img.shields.io/badge/MyBatis-DC382D?style=flat-square&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=flat-square&logo=vue.js&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)

---

## 📌 Projects

### 🏠 홀가(家)분 — 🏆 최우수상
> 시니어 대상 부동산 다운사이징 플랫폼 · 팀 프로젝트 6인 (2026.07 ~ 2026.08)
> `Java` `Spring Legacy` `MyBatis` `MySQL` `Vue 3`

보유 주택을 정리하고 더 적합한 집으로 이주하려는 시니어를 위해, **설문 → 추천 매물 → 매물 비교 → 최종 선택 → 금융상품 추천 → 분석 보고서(PDF)** 로 이어지는 단일 플로우를 제공하는 서비스입니다.

**담당 역할 및 성과**
- **공간 연산 최적화**: 매물마다 반경 내 시설 수를 세는 전수 비교 방식의 계산량 문제를, 지도를 0.01° 격자로 나눠 인접 셀만 비교하도록 개편 → 실제 적재 규모 벤치마크에서 **약 76배 단축**
  - 반경이 셀보다 큰 시설(1km)은 3×3 탐색 시 경계 시설이 최대 0.3% 누락되는 트레이드오프를 직접 검증하고 3×5 탐색으로 보정
- **취득세·중개보수 백엔드 계산**: 지방세법·농어촌특별세법 기준 로직을 프론트에서 백엔드로 이관해 계산식 노출을 막고 기준을 한 곳에서 관리
  - 6~9억 구간 반올림 오차(`double` 부동소수점)를 정수 연산으로 제거, 계단이 바뀌는 **경계값 4개를 단위 테스트로 고정**
- **공공데이터 파이프라인**: 국토부 실거래가(11만여 건), CCTV·전통시장·대형마트·행정복지센터·은행·공원·약국 등 좌표 기반 반경 매칭
  - 실거래 데이터 **75.6% 중복** 발견 → `ROW_NUMBER() OVER(PARTITION BY ...)` 기반 중복 제거
  - 몇 주째 갱신되지 않던 배치 4종을 스케줄러·DB 스키마 확인으로 발견해 **직접 복원**
- **화면 개발**: 추천 매물 목록/상세, 지도·목록 토글 및 주변 시설 필터, 찜(관심 매물) 기능
- 평가 점수 산정 기준의 법령·공공연구 근거 조사 및 문서화

**Repo**: [PJT29-3team](https://github.com/PJT29-3team) ([backend](https://github.com/PJT29-3team/backend) · [frontend](https://github.com/PJT29-3team/frontend) · [database](https://github.com/PJT29-3team/database))

---

### 💰 KaratBook
> 가계부 웹 서비스 · 부트캠프 팀 프로젝트
> `Vue 3` `Pinia` `json-server`

부트캠프 초기 팀 프로젝트로, Vue 3 컴포넌트 구조와 Pinia 상태관리를 적용해 수입·지출 관리 화면을 구현하며 Git 기반 협업을 경험했습니다.

**Repo**: [KB-Skeleton-Project-5](https://github.com/KB-Skeleton-Project-5)

---

## 📚 Study Repos

| 저장소 | 내용 |
|---|---|
| [java_study](https://github.com/ryeon-xx/java_study) | Java 문법 및 OOP 학습 |
| [sql_study](https://github.com/ryeon-xx/sql_study) | SQL 실습 및 정리 |
| [jsp_study](https://github.com/ryeon-xx/jsp_study) | Servlet/JSP, MVC 패턴 학습 |
| [spring_study](https://github.com/ryeon-xx/spring_study) | Spring Framework 학습 |
| [study](https://github.com/ryeon-xx/study) | 웹 기초(HTML/CSS/JS) 학습 |

---

## 📊 GitHub Stats

![GitHub stats](https://github-readme-stats.vercel.app/api?username=ryeon-xx&show_icons=true&theme=default)
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=ryeon-xx&layout=compact)

## 📫 Contact

- Email: rlarkgus3415@gmail.com
