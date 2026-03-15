# 만나봄(mannabom)
![img.png](img.png)

만나봄은 더 자연스럽고 안전한 연결을 돕는 소개팅·매칭 서비스입니다.  
프로필 기반 추천, 호감/메시지 요청, 후기 및 별점 평가 등 매칭 이후의 경험까지 매끄럽게 이어지도록 설계했습니다.

## 핵심 기능

- 회원가입 및 로그인
- 프로필 등록 및 조회
- 추천 프로필 조회
- 호감 보내기
- 메시지 요청 보내기 (간단한 메시지 첨부)
- 후기 작성 및 별점 평가
- 푸시 알림(FCM) 기반 이벤트 안내
- 미팅 매칭
- 채팅

## 기술 스택

- Backend: Java, Spring Boot, Spring Data JPA
- Database: PostgreSQL, Flyway
- Infra: AWS (EC2, S3)
- Push: Firebase Cloud Messaging (FCM)
- Build/Dev: Gradle, Docker Compose, Github Actions

## 레포지토리 안내

- 서버: 백엔드 API 및 도메인 로직
- 인프라: 배포/환경 구성, Docker/스크립트
- 문서: 요구사항, 설계, API 명세, 규칙

※ 레포 구조와 링크는 프로젝트 진행에 맞춰 계속 정리됩니다.

## 로컬 실행

1. 저장소 클론
2. 환경 변수 설정 (예: `.env.local` 또는 `application-local.yml`)
3. DB/Redis 등 의존 서비스 실행 (Docker Compose 사용 권장)
4. 애플리케이션 실행

프로젝트별 실행 방법은 각 서브 레포지토리의 README를 참고해주세요.

## 라이선스

라이선스는 추후 정리 예정입니다.

## 팀

- 김준언(BE): 백엔드 개발. Spring Boot 기반으로 API 설계와 구현을 담당했고, 도메인 모델링(JPA), 데이터베이스 설계/쿼리 최적화, 더미 데이터 구성 및 테스트 환경 정리를 진행했습니다. 또한 AWS 환경(EC2/S3) 기반 배포 흐름과 운영 관점에서 필요한 설정, 푸시 알림(FCM) 연동 및 전송 안정화 같은 인프라·연동 작업에도 참여했습니다.
- 임세희(BE): 백엔드 개발. Spring Boot 기반으로 API 설계와 구현을 담당했습니다. 운영 안정성을 위해 Flyway를 도입하여 DB 스키마 형상 관리를 자동화하고, 팀원 간의 데이터베이스 환경 불일치 문제를 해결했습니다. 또한 GitHub Actions와 Docker Compose를 연동하여 빌드부터 운영 서버(AWS EC2) 배포까지의 CI/CD 파이프라인을 구축하였습니다.
- 김동성(FE):
- 송성근(DS):
