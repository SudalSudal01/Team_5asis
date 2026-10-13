# 5ASIS | 김명현의 백엔드 포트폴리오

이 저장소는 **팀 프로젝트의 개인 포트폴리오용 포크**입니다. 팀 원본의 Git 이력과 구성원 기여를 보존하고, 김명현이 담당한 기능을 중심으로 소개합니다. 전체 코드를 혼자 개발한 개인 프로젝트가 아닙니다.

- 팀 원본: [https://github.com/PSK6262/Team_5asis](https://github.com/PSK6262/Team_5asis)
- 개인 GitHub: [SudalSudal01](https://github.com/SudalSudal01)

- 본인 담당: **메인 대시보드 · Steam API 연동 · 결과 발표**
- 기술: Java 11, Spring MVC, JSP, MyBatis, Oracle, RestTemplate, Steam Store API
- 팀 프로젝트이며 다른 구성원의 로그인·방송 API 등 담당 기능을 개인 기여로 표현하지 않습니다.

## 담당 기능의 코드 안내

| 기능 | 주요 코드 | 설명 |
| --- | --- | --- |
| 메인 대시보드 | [MainController](src/main/java/com/app/controller/MainController.java) · [main.jsp](src/main/webapp/WEB-INF/views/main.jsp) | 내부 인기 게임과 외부 할인·랜덤 게임 데이터를 메인 화면에 전달합니다. |
| Steam API 연동 | [SteamGameServiceImpl](src/main/java/com/app/service/api/impl/SteamGameServiceImpl.java) | 외부 응답을 화면용 데이터로 변환하고 중복과 재시도 범위를 제한합니다. |

## 검증 범위와 개선 과제

팀 결과보고서의 담당 기록과 저장소 코드를 대조했습니다. 개인 포크 생성 때 서비스 전체 자동 테스트나 실제 Steam 응답 재검증을 수행하지 않았습니다. 외부 API의 시간 제한·캐시와 호출 실패/정상 빈 결과 구분은 후속 개선 과제입니다.

## 실행과 원본 문서

기존 팀 README는 [README.team.md](README.team.md)에 그대로 보존했습니다. 설치·실행 방법 및 팀 서비스 전체 소개는 해당 문서를 참고해 주세요. 실제 환경설정·API 키·개인 데이터는 별도로 준비해야 하며 새로 커밋하지 않습니다. 이 포크의 개인화 작업은 소개 문서 정리이며 원본의 실행 코드 변경이나 새 기능 구현을 의미하지 않습니다.

원본에 포함된 문서와 코드의 저작권·출처는 기존 팀과 각 기여자에게 유지됩니다. 이 포크에서 별도 라이선스를 임의로 추가하지 않습니다.
