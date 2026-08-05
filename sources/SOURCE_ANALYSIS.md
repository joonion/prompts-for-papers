# 참고 저장소 분석

분석 기준일은 2026-08-06이며, 로컬에 복제한 저장소의 아래 커밋을 기준으로 했다.

| 저장소 | 기준 커밋 | 확인된 콘텐츠 | 이 프로젝트에서의 활용 |
|---|---|---:|---|
| ChatGPT Prompts for Academic Writing | `4029d94` | 코드 블록 기준 약 85개 | 연구 단계와 작업 유형을 발굴하는 참고 목록 |
| University of Basel Prompt Library | `577bb98` | 구조화된 프롬프트 2개 | 메타데이터, 입력·출력 예시, 버전과 권리 정보 설계 |
| Awesome Prompts for Academic Work | `f142a20` | 영어 113개, 한국어 11개 | 장문 프롬프트 구조, 평가 관점, 분야별 확장 아이디어 |

## 분석 결과

### ChatGPT Prompts for Academic Writing

- 장점: 연구 주제 탐색, 논문 섹션 작성, 문장 개선과 요약을 빠르게 훑을 수 있다.
- 한계: 입력 자료와 출력 기준이 짧거나 생략된 항목이 많다.
- 위험: 모델의 기억만으로 문헌과 링크를 생성하게 하는 항목은 허위 인용을 만들 수 있다.
- 적용: 원문을 복제하거나 번역하지 않고 작업 유형을 파악하는 데만 사용했다. 로컬 복제본에서 별도 라이선스를 확인하지 못했기 때문이다.

### University of Basel Prompt Library

- 장점: 식별자, 제목, 설명, 주제, 모델, 입력·출력 예시, 버전, 수정일과 라이선스를 함께 관리한다.
- 한계: 현재 항목 수가 2개이며 일반적인 논문 작성 전 과정을 다루지는 않는다.
- 적용: 프롬프트를 재사용 가능한 데이터로 관리하는 원칙과 명시적 출력 형식을 참고했다.

### Awesome Prompts for Academic Work

- 장점: 연구 질문, 검색 전략, 방법론, 분석, 글쓰기, 심사 대응과 연구 커뮤니케이션에 이르는 작업이 구체적이다.
- 한계: 프롬프트가 영어 `general.md`에 집중되어 있고, 한국어판과 여러 분야 파일은 실제 항목이 적거나 비어 있다.
- 위험: 저널 추천, 문헌 탐색, 통계 해석처럼 최신 정보나 원자료가 필요한 작업에는 별도 검증 장치가 필요하다.
- 적용: 작업 목표와 평가 관점을 참고하되, 문장은 복제하지 않고 이 프로젝트의 안전 원칙에 따라 새로 작성했다.

## 단계별 매핑

| 연구 단계 | 선별한 핵심 작업 | 주요 참고 아이디어 |
|---|---|---|
| 연구 준비와 윤리 | AI 활용 계획, 민감정보 점검, 연구윤리 사전 검토 | Ethics-Focused Research Designer, Data Management Planning Expert |
| 연구 주제와 연구 문제 | 주제 좁히기, 연구 질문 설계, 질문·가설 평가 | Academic Research Question Generator, Research Question Quality Assessor, Hypothesis Development Expert |
| 문헌 탐색과 비판적 검토 | 검색 전략, 근거표, 비판적 종합과 공백 | Advanced Literature Search Strategist, Evidence Table Designer, Multi-Source Literature Synthesizer |
| 연구 방법 설계 | 방법 적합성, 표본·자료수집, 설계 통합 점검 | Methodology Appropriateness Analysis, Sampling Strategy Designer, Mixed-Methods Design Expert |
| 자료 분석과 결과 해석 | 분석 계획, 결과 해석, 표·그림 점검 | Statistical Test Selection Guide, Statistical Output Interpreter, Data Visualization Strategy Advisor |
| 논문 구조와 초안 작성 | 전체 개요, 근거 기반 섹션 초안, 제목·초록 | Article Sections 및 Outline 작업 목록 |
| 인용, 논증과 문장 검토 | 논증 점검, 문장·구조 교정, 인용 감사 | Argument Strength Analyzer, Text Coherence Enhancer, Comprehensive Proofreader |
| 투고와 심사 대응 | 저널 적합성, 모의 심사, 답변표 | Academic Journal Selection Advisor, Comprehensive Manuscript Reviewer, Reviewer Response Table Creator |
| 연구 커뮤니케이션 | 학회 발표, 대중 요약, 정책 브리프 | Conference Presentation Designer, Academic-to-Public Translator, Research-to-Policy Communicator |

## 설계 결정

- 학문 분야가 아니라 연구 진행 단계를 기본 탐색 축으로 사용한다.
- 첫 버전은 단계별 핵심 프롬프트 3개, 총 27개로 제한한다.
- 모든 프롬프트에 목표, 입력, 출력 형식, 제한 조건, 검증 체크리스트와 출처를 포함한다.
- 문헌, 인용, 통계와 연구윤리 관련 작업은 위험도를 높게 표시한다.
- 외부 원문을 번역해 수록하지 않고 여러 작업 아이디어를 종합하여 독립적으로 작성한다.

## 라이선스 처리

- University of Basel 자료는 CC BY 4.0으로 공개되어 있다.
- Awesome Prompts for Academic Work는 MIT License로 공개되어 있다.
- ChatGPT Prompts for Academic Writing는 분석한 로컬 복제본에서 별도 라이선스를 확인하지 못했다.
- 새 프롬프트는 원문의 표현을 복제하지 않은 독립 저작물이며 프로젝트의 CC BY 4.0을 적용한다.
- 외부 자료의 권리는 원저작자에게 있으며 자세한 내용은 [`THIRD_PARTY_NOTICES.md`](../THIRD_PARTY_NOTICES.md)를 따른다.
