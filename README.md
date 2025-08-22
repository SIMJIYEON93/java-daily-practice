# Java Daily Practice
Daily Java practice repository — problem solving, unit testing, and clean code exercises with continuous growth logs.

- **시작일**: 2025-08-21 ~ (ongoing)  
- **목표**: 하루 1커밋, 작은 문제 풀이 및 리팩토링을 통해 Java 기본기와 TDD 습관화

## 구성
- **모듈**
  - `kata` : 순수 Java 연습(알고리즘/유틸/리팩토링)
  - `boot-app` : Spring Boot 실습(API, 미니 서비스)

- **디렉터리 규칙**
  - `kata/src/main/java/day/DayYYYY_MM_DD_<Topic>.java` : 매일의 연습 코드
  - `kata/src/test/java/day/DayYYYY_MM_DD_<Topic>Test.java` : 단위 테스트
  - `boot-app/src/main/java/com/<yourgroup>/bootapp/daily/yYYYY/mMM/dDD/...` : 일자별 샌드박스 API
  - `log/YYYY-MM-DD.md` : 오늘 배운 점과 회고 기록
 
  ## 예시 트리
  ```
  ├─ settings.gradle
  ├─ build.gradle
  ├─ log/
  │ ├─ 2025-08-21.md
  │ └─ 2025-08-22.md
  ├─ kata/
  │ ├─ build.gradle
  │ └─ src/
  │ ├─ main/java/day/
  │ │ ├─ Day2025_08_21_ReverseString.java
  │ │ └─ Day2025_08_22_Palindrome.java
  │ └─ test/java/day/
  │ ├─ Day2025_08_21_ReverseStringTest.java
  │ └─ Day2025_08_22_PalindromeTest.java
  └─ boot-app/
  ├─ build.gradle
  └─ src/
  ├─ main/java/com/yourgroup/bootapp/
  │ ├─ BootAppApplication.java
  │ └─ daily/y2025/m08/d21/SandboxController.java
  └─ test/java/com/yourgroup/bootapp/
  └─ daily/y2025/m08/d21/SandboxControllerTest.java
  ```

## 사용 방법
- 전체 테스트: `./gradlew test`
- kata만 테스트: `./gradlew :kata:test`
- Spring Boot 실행: `./gradlew :boot-app:bootRun` → `http://localhost:8080`

## 커밋 규칙 예시
- `feat(kata): Day2025-08-21 reverse string + tests`
- `feat(boot): /api/daily/2025-08-21/hello endpoint`
- `refactor(kata): extract method & rename`
- `docs(log): add 2025-08-21 daily notes`

## Weekly Summary
- [Week 1 Summary](log/week-1.md)
- [Week 2 Summary](log/week-2.md)

---

## Notes
- 가능한 작은 단위라도 **테스트 코드 포함**을 원칙으로 함  
- 매주 일요일에 1주차 요약(Log + 링크) 정리  
- 장기적으로 **알고리즘 → 자료구조 → Java 유틸/Stream → 백엔드 관련 미니 유틸** 순서로 확장 계획

