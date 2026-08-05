# 프롬프트 사용 안내

이 디렉터리에는 논문 작성 과정을 9개 단계로 나눈 핵심 프롬프트 27개가 있다. 각 프롬프트는 독립된 Markdown 파일이며, 단계별 상위 문서는 프롬프트를 정리하고 연결하는 인덱스 역할을 한다. 프롬프트를 사용할 때는 대괄호로 표시된 입력 변수를 실제 연구 정보로 바꿔야 한다.

## 디렉터리 구조

```text
prompts/
├─ 01-research-preparation-and-ethics.md
├─ 01-research-preparation-and-ethics/
│  ├─ PREP-01.md
│  ├─ PREP-02.md
│  └─ PREP-03.md
├─ 02-topic-and-research-question.md
├─ 02-topic-and-research-question/
│  └─ TOPIC-*.md
└─ ...
```

- `0N-stage-name.md`: 단계의 프롬프트를 표로 정리한 상위 인덱스
- `0N-stage-name/ID.md`: 하나의 프롬프트만 담는 독립 파일
- `README.md`: 전체 단계, 사용법과 기여 규칙

## 단계별 인덱스

| 단계 | 상위 인덱스 | 프롬프트 디렉터리 | 수 |
|---:|---|---|---:|
| 1 | [연구 준비와 윤리](01-research-preparation-and-ethics.md) | [`01-research-preparation-and-ethics/`](01-research-preparation-and-ethics/) | 3 |
| 2 | [연구 주제와 연구 문제](02-topic-and-research-question.md) | [`02-topic-and-research-question/`](02-topic-and-research-question/) | 3 |
| 3 | [문헌 탐색과 비판적 검토](03-literature-search-and-review.md) | [`03-literature-search-and-review/`](03-literature-search-and-review/) | 3 |
| 4 | [연구 방법 설계](04-methodology-design.md) | [`04-methodology-design/`](04-methodology-design/) | 3 |
| 5 | [자료 분석과 결과 해석](05-analysis-and-interpretation.md) | [`05-analysis-and-interpretation/`](05-analysis-and-interpretation/) | 3 |
| 6 | [논문 구조와 초안 작성](06-structure-and-drafting.md) | [`06-structure-and-drafting/`](06-structure-and-drafting/) | 3 |
| 7 | [인용, 논증과 문장 검토](07-citation-argument-and-editing.md) | [`07-citation-argument-and-editing/`](07-citation-argument-and-editing/) | 3 |
| 8 | [투고와 심사 대응](08-submission-and-peer-review.md) | [`08-submission-and-peer-review/`](08-submission-and-peer-review/) | 3 |
| 9 | [연구 커뮤니케이션](09-research-communication.md) | [`09-research-communication/`](09-research-communication/) | 3 |

## 메타데이터

각 프롬프트에는 다음 메타데이터를 기록한다.

| 필드 | 의미 |
|---|---|
| ID | 단계와 순서를 나타내는 고유 식별자 |
| 작업 | 프롬프트가 지원하는 구체적인 연구 작업 |
| 태그 | 분야 또는 탐색에 사용할 키워드 |
| 입력 유형 | 사용자가 준비해야 할 자료 유형 |
| 출력 형식 | 모델이 따라야 할 결과 구조 |
| 위험도 | `낮음`, `중간`, `높음` 중 하나 |
| 마지막 검토일 | 대표 입력으로 구조와 안전 조건을 검토한 날짜 |

## 프롬프트 기여 방법

1. 프롬프트가 속할 연구 단계를 선택한다.
2. 해당 단계의 ID 접두사와 다음 번호를 확인한다.
3. 단계 디렉터리에 `ID.md` 형식의 파일을 하나 추가한다.
4. 아래 템플릿의 모든 필수 섹션을 작성한다.
5. 같은 이름의 상위 단계 인덱스 표에 새 파일의 상대 링크를 한 줄 추가한다.
6. 대표 입력으로 드라이런한 뒤 `마지막 검토일`과 검증 기록을 갱신한다.

ID 접두사는 `PREP`, `TOPIC`, `LIT`, `METHOD`, `ANALYSIS`, `WRITE`, `EDIT`, `SUBMIT`, `COMM`을 사용한다. 기존 ID를 변경하거나 재사용하지 않는다.

### 개별 프롬프트 템플릿

````markdown
# ID. 프롬프트 제목

| 항목 | 내용 |
|---|---|
| 작업 | 구체적인 연구 작업 |
| 태그 | `태그 1`, `태그 2` |
| 입력 유형 | 사용자가 준비할 자료 |
| 출력 형식 | 결과 구조 |
| 위험도 | 낮음, 중간 또는 높음 |
| 마지막 검토일 | YYYY-MM-DD |

### 사용 목적

이 프롬프트를 언제 사용하는지 설명한다.

### 필요한 입력

- `[입력 변수]`

### 프롬프트

```text
복사하여 사용할 프롬프트 본문을 작성한다.
[입력 변수]
```

### 제한 조건

- 생성하거나 추정하면 안 되는 내용을 명시한다.

### 검증 체크리스트

- [ ] 연구자가 직접 확인할 항목을 작성한다.

### 출처와 라이선스

- 설계 참고: 참고한 자료 또는 `독립 작성`
- 작성 방식: 직접 개발, 번역, 각색 또는 종합
- 라이선스: CC BY 4.0 또는 원본 라이선스
````

## 사용 순서

1. 사용 목적이 현재 작업과 맞는지 확인한다.
2. 필요한 입력을 준비하고 개인정보와 미공개 정보를 제거한다.
3. 프롬프트의 대괄호 변수를 실제 정보로 바꾼다.
4. 출력 결과를 검증 체크리스트에 따라 확인한다.
5. 문헌, 인용, 수치와 연구 결과는 반드시 원자료에서 다시 확인한다.

## 공통 안전 원칙

- 자료가 부족하면 모델이 추측하지 않고 `확인 필요`라고 표시하게 한다.
- 제공하지 않은 문헌, DOI, 데이터, 분석 결과와 연구 절차를 만들지 않는다.
- 사실, 제공 자료의 요약과 모델의 제안을 구분한다.
- AI 출력은 연구자의 판단과 원자료 검증을 대신할 수 없다.
- 소속기관, 학술지와 연구 분야의 AI 사용 및 공개 정책을 별도로 확인한다.

## 출처와 라이선스

프롬프트는 [참고 저장소 분석](../sources/SOURCE_ANALYSIS.md)에 기록된 작업 아이디어를 종합하여 독립적으로 작성했다. 별도 표시가 없는 이 디렉터리의 콘텐츠에는 프로젝트의 [CC BY 4.0 라이선스](../LICENSE)가 적용된다.

대표 입력을 이용한 드라이런과 정적 검사 결과는 [프롬프트 검증 기록](../validation/PROMPT_VALIDATION.md)에서 확인할 수 있다.
