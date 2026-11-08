# 김지성 · 백엔드 개발자 포트폴리오

폐쇄망 엔터프라이즈 고객사에 설치되는 데이터 카탈로그 솔루션을 만들고 있습니다.
최근에는 이 솔루션에 **RAG 기반 AI 검색**을 붙이는 일을 리더 없이 기획·설계·평가까지 맡고 있습니다.

- 데이터트리코리아 솔루션개발팀 선임 (2023.05 – 현재) · 금융·유통·물류 대기업 고객사 8곳
- 주력: TypeScript, Node.js (NestJS), Elasticsearch, MongoDB, RDB, Docker
- AI: RAG, Hybrid Search (BM25 + Vector), vLLM 기반 로컬 LLM, NL2SQL, Claude Code
- 연락: jisungableee@gmail.com

> 회사 코드는 공개할 수 없어, 실제 작업을 설계 판단과 측정 결과 중심으로 정리했습니다.
>
> 내부 이름은 일반화했고, 수치는 개발 환경 기준입니다.

## 사례

| 사례 | 한 줄 요약 | 키워드 |
|---|---|---|
| [폐쇄망 카탈로그의 질의 해석 기반 AI 검색](01-ai-search-rag.md) | 질문을 해석한 뒤 하이브리드 검색으로 근거를 찾게 바꿔, 숨겨지던 근거를 62건 → 30건으로 줄임 | RAG, Hybrid Search, 정량 평가, vLLM, SSE |
| [메타데이터 RAG 기반 NL2SQL 설계](02-nl2sql-metadata-rag.md) | 고객사마다 다른 스키마를 카탈로그 검색으로 골라 SQL 생성 근거로 쓰는 구조 | Text-to-SQL, RAG, SQL 안전장치 |
| [설치형 솔루션의 운영 문제 해결](03-backend-cases.md) | 다중 노드 분산 락, 이벤트 루프 차단 해소, 저장소 전환 마이그레이션 | NestJS, MongoDB, worker_threads |

## 개인 프로젝트

| 프로젝트 | 한 줄 요약 | 키워드 |
|---|---|---|
| [proposal-mcp](https://github.com/jableee/proposal-mcp) | 실무에서 반복되던 제안서 작업을 MCP 서버로 만듦. RFP 요구사항마다 표준·커스터마이징·범위 외를 정의서 인용과 함께 판단하고, 서버가 인용을 원문과 대조해 검증. 사람이 추적표와 초안을 승인해야 PPT가 나옴. 샘플 RFP 14건에서 판단 14건이 정답과 일치 | MCP, Tool Calling, Human-in-the-loop, TypeScript |

## 일하는 방식
- **측정하고 결정합니다.** 질문 세트와 평가 스크립트로 바꾸기 전·후를 비교한 뒤 결정합니다.
- **고객 환경의 제약을 먼저 봅니다.** 폐쇄망, 고객사마다 다른 LLM, 의존성 검증 비용 같은 조건이 설계를 정합니다.
- **AI와 함께 일하는 방식을 팀에 퍼뜨립니다.** 사내에 Claude Code를 추천해 전사 도입으로 이어졌고, 개념 교육·실습 과제·개별 피드백으로 팀의 사용 방식을 만들었습니다.
