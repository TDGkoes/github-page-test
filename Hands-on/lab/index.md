---
layout: home
title: 홈
nav_order: 1
permalink: /
---

# Microsoft Copilot Studio GHCP Harness Hands-on Lab

{: .warning}
내용 검토용 초안: 실습 자료는 보완 중이므로 다운로드·참조 링크를 제외했습니다. 실습 자료 작업 완료 후 교안과 자료 링크를 수정하여 재배포할 예정입니다. 

**RFP 분석 및 제안서·WBS 생성 에이전트 구축**

업무를 Skill로 나누고 필요한 도구·지식을 연결해, 분석 결과에서 제안서와 WBS까지 이어지는 에이전트를 구성합니다. 결과와 실행 근거를 확인하며 개선하는 방법도 함께 알아봅니다.

## 1. 학습 목표와 준비사항

RFP 에이전트를 구성하며 다음 내용을 익힙니다.

- 업무를 Skill로 나누고 Instructions로 실행 순서와 공통 원칙을 연결합니다.
- 필요한 Tool·Knowledge를 선택하고, 앞 단계의 결과를 다음 단계에서 재사용하도록 구성합니다.
- 응답·근거·파일과 Activity Trace를 확인해 문제 원인을 찾고 개선합니다.

### 시작 전 확인

| 준비 항목 | 확인할 내용 |
|---|---|
| 계정·환경 | Copilot Studio에 로그인하고, 사용할 환경에서 GHCP 에이전트를 생성·편집할 수 있는지 확인 |
| 연결 기능 | 해당 환경에서 Skill 업로드, MCP 도구 연결, Knowledge 추가를 사용할 수 있는지 확인 |
| 지식 저장소 | Step4의 SharePoint 방식에 사용할 폴더와 접근 권한 준비. 파일 추가 방식은 해당 환경의 지원 여부 확인 |
| 제공 자료 | GHCP Harness 개요 페이지의 ‘사용할 자료’에서 지침·Skill 등록 파일·지식 샘플·테스트 RFP 확인 |
| 결과 확인 | 생성된 `.pptx`·`.xlsx`를 열어 내용과 서식을 확인할 수 있는 프로그램 준비 |

구체적인 화면 조작과 연결 방법은 각 Step에서 확인합니다.

## 2. 완성할 에이전트와 업무 흐름

RFP에서 요구사항·구축 청사진·추천 인력을 정리하고, 그 결과를 이어받아 제안서와 WBS를 작성하는 에이전트입니다.

![RFP 분석부터 상세 WBS까지의 에이전트 업무 흐름]({{ '/Hands-on_image/ProjectDeliveryAgent흐름도.png' | relative_url }})

**분석 → Draft WBS → 제안서 → 상세 WBS** 순으로 이전 결과를 재사용합니다. Draft WBS는 별도 Excel 파일 없이 중간 계획 데이터로 전달합니다. 청사진과 인력 후보를 일정·수행계획에 연결하고, 최종적으로 표준 양식을 적용한 제안서 `.pptx`와 WBS `.xlsx`를 생성합니다.

## 3. 전체 학습 경로

| 페이지 | 확인할 내용 |
|---|---|
| [GHCP Harness 개요]({{ '/lab/GHCP-Harness-Overview.html' | relative_url }}) | 하네스의 특징·Agentic Loop·Standard 비교·선택 이유·사용 자료 |
| [Step1. GHCP Harness 에이전트 생성 및 Instructions 작성]({{ '/lab/agent-instructions.html' | relative_url }}) | 에이전트 생성과 전체 목표·범위·공통 원칙 설정 |
| [Step2. Skills 구성]({{ '/lab/skills.html' | relative_url }}) | 업무 분리·입출력·완료 기준 설계와 세 Skill 등록 |
| [Step3. Tools 및 MCP 등록]({{ '/lab/tools-mcp.html' | relative_url }}) | 필요한 행동과 출처를 기준으로 Learn MCP 연결 |
| [Step4. Knowledge 구성]({{ '/lab/knowledge.html' | relative_url }}) | 인력·참고 자료의 역할과 검색 범위 구성 |
| [Step5. 테스트 및 Activity Trace]({{ '/lab/testing.html' | relative_url }}) | 기대 동작과 실행 증거를 대조하고 원인에 맞게 개선 |
| [Step6. 정리 및 마무리]({{ '/lab/wrap-up.html' | relative_url }}) | 설계·검증 기준을 정리하고 자신의 업무에 적용 |

---

<nav class="lab-page-nav" aria-label="페이지 이동">
  <a class="lab-page-nav__next" href="{{ '/lab/GHCP-Harness-Overview.html' | relative_url }}" rel="next">다음</a>
</nav>
