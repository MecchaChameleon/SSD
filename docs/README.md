# 프로젝트 문서 모음

처음 보는 분은 [프로젝트 소개](../README.md)와 [데모 영상](../assets/videos/demo.mp4)을 먼저 확인하세요.

## 통합 문서

| 문서 | 내용 |
|---|---|
| [통합본선 발표자료 PDF](../제주로컬타임AI_통합본선_발표자료.pdf) | 서비스 소개·검증·재무 시나리오를 담은 전체 26쪽 |
| [발표자료 부록 모음](presentation-appendix.md) | 18~25쪽 원문 이미지와 수치 해석 |
| [시스템 아키텍처](architecture.md) | FE·BE·AI의 역할, 가격 추천과 자연어 추천의 요청 흐름 |
| [AI 가격 추천 및 검증](ai-pricing.md) | 현재 운영 구조, XGBoost 비교 실험, 합성 가격정책 실험 |
| [개인정보처리방침](../index.html) | 기존 privacy 저장소에서 보존한 공개 문서 |

## 서비스별 개발 안내

| 영역 | 저장소 |
|---|---|
| 앱·웹 | [SSD_FE](https://github.com/MecchaChameleon/SSD_FE) |
| 비즈니스 API | [SSD_BE](https://github.com/MecchaChameleon/SSD_BE) |
| 수요 모델·가격 추천·실험 | [SSD_AI](https://github.com/MecchaChameleon/SSD_AI) |

## 기존 기술 자료와 검증 근거

상세 원본은 담당 코드와 함께 관리하고, 이 저장소에서는 링크와 요약을 제공합니다.

| 자료 | 원본 |
|---|---|
| AI 추천가 기술문서 | [AI_추천가_시스템_기술문서.docx](https://github.com/MecchaChameleon/SSD_AI/blob/main/docs/AI_추천가_시스템_기술문서.docx) |
| XGBoost 비교 성능 | [수요예측 성능표](https://github.com/MecchaChameleon/SSD_AI/blob/main/docs/PPT_XGB_성능표.md) |
| 가격정책 설계와 검증 | [가격정책 어펜딕스](https://github.com/MecchaChameleon/SSD_AI/blob/main/docs/PPT_가격정책_어펜딕스.md) |
| 합성 사용자 실험 | [시뮬레이션 설명](https://github.com/MecchaChameleon/SSD_AI/blob/main/simulation/README.md) |
| 폐기손실 반영 정책 비교 보고서 | [실험 보고서.docx](https://github.com/MecchaChameleon/SSD_AI/blob/main/simulation/합성_사용자_기반_가격정책_비교실험_보고서_폐기손실반영본.docx) |
| 동시접속 부하테스트 | [부하테스트 보고서.docx](https://github.com/MecchaChameleon/SSD_AI/blob/main/simulation/동시접속_부하테스트_결과_최종본.docx) |
| 인프라 측정 및 비용 추정 | [인프라 최종 보고서](https://github.com/MecchaChameleon/SSD_AI/blob/main/infrastructure_test/docs/infrastructure_cost_final_report.md) |

문서마다 작성 시점과 평가 조건이 다를 수 있습니다. 모델 종류와 실험 결과는 각 자료에 명시된 데이터 범위·평가 단위와 함께 확인하세요.

## 자료 추가

- 발표자료와 서비스 소개서: 현재 통합본선 PDF는 저장소 루트에서 관리합니다. 추가 자료는 이 폴더에 넣고 위 목록에 링크합니다. PDF를 수정하면 README의 검증 수치와 부록 페이지 이미지도 함께 갱신합니다.
- 데모 영상: README는 `assets/videos/demo.gif`를 바로 표시하고, `assets/videos/demo.mp4`를 원본 영상으로 연결합니다. 영상을 교체할 때는 GIF와 MP4를 함께 갱신합니다.
- 화면 이미지: `assets/images/`에 추가하고 README에서 상대경로로 참조합니다.

저장소 관리자는 [privacy → SSD 전환 안내](repository-setup.md)를 참고하세요.
