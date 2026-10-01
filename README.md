# UiPath AI News Scraper

UiPath로 인기 기사와 키워드 기사를 수집하고, 생성형 AI로 유의성을 판단·요약한 뒤 Excel로 저장하고 Gmail로 발송하는 RPA 실습 프로젝트입니다.

## 주요 기능

- 인기 기사 및 키워드 검색 결과 수집
- 기사 본문 추출과 생성형 AI 요약
- 부적합 기사와 중복 URL 제외
- `HeadLineArticle`, `SearchArticle` 시트로 Excel 저장
- Gmail 결과 메일 발송

## 실행 전 설정

1. UiPath Studio에서 `project.json`을 엽니다.
2. 프로젝트 의존성을 복원합니다.
3. 두 개의 `Content Generation` 액티비티에 본인의 UiPath Integration Service 연결을 지정합니다.
4. `Use Gmail` 액티비티에 본인의 Gmail 계정을 연결합니다.
5. 발신·수신 메일 주소를 실제 사용할 주소로 변경합니다.

보안을 위해 원본 Gmail 주소와 UiPath 연결 ID는 저장소에서 제거했습니다. 실행 결과인 `ArticleList_*.xlsx`, 임시 파일과 UiPath 로컬 캐시는 커밋하지 않습니다.

