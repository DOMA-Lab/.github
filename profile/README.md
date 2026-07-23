<div align="center">

# 🩺 도마 · DOMA

### 멈춘 자동화 라인을 다시 살리는 제조 사후보전(RCA) AI

**PLC 라인이 멈춘 순간부터 복구까지 — 그 시간을 줄이고, 그 지식을 자산으로 남깁니다.**

<br>

`멈춘 라인 → 4시간이 아니라 15분 → 그 지식이 회사의 자산으로 남는다`

<br>

![Status](https://img.shields.io/badge/stage-Vertical_Slice_PoC-6E56CF?style=for-the-badge)
![Domain](https://img.shields.io/badge/domain-Factory_Automation-1F883D?style=for-the-badge)
![AI](https://img.shields.io/badge/AI-RCA_Copilot-F97316?style=for-the-badge)
![Deploy](https://img.shields.io/badge/deploy-On--Prem-0969DA?style=for-the-badge)

</div>

---

## 🎯 우리가 푸는 문제

> PLC는 50년간 공장 자동화의 표준이 되었습니다. **하지만 PLC는 자기가 제어하는 설비의 실제 상태를 직접 알지 못합니다.**

정의되지 않은 방식으로 설비가 고장 나면, PLC는 *"왜 멈췄는지"* 를 모른 채 그저 멈춰 섭니다. 그때부터 사람이 옵니다.

- 🔧 **자동화는 했지만, 운영은 아직 사람과 외주에 의존합니다.** 라인이 멈출 때마다 외주 청구서와 다운타임 손실이 쌓입니다.
- 🧠 **복구는 베테랑의 암묵지에 달려 있습니다.** 도면이 100% 최신화된 공장은 없고, 진짜 자산은 *"그 라인의 야사를 아는 사람"* 의 머릿속에 있습니다.
- ⏳ **그 베테랑은 은퇴하고, 새 인력은 오지 않습니다.** 지식이 사라지면 라인은 더 오래 멈춥니다.

**릴레이 시대의 페인이 "변경 비용"이었고 그 답이 PLC였다면 — 지금 PLC 시대의 페인은 "운영·진단·복구 비용"입니다. 도마는 그 다음 자리에서 일합니다.**

---

## 💡 도마의 해법

도마는 PLC를 대체하지 않습니다. **이미 깔린 PLC가 더 잘 운영되도록** 만듭니다.
안전과 결정론은 끝까지 PLC가 담당하고, 도마는 그 위에 **인지·맥락·이력** 레이어를 얹습니다.

```
PLC 알람 → 진단(RCA) → 복구 가이드(HITL) → 조치 · 감사 → 학습(의미사전 · 케이스 축적)
   └──────────────── 그 지식이 다시 진단 정확도로 환류됩니다 ────────────────┘
```

### 핵심 기능 6축

| | 기능 | 설명 |
|---|------|------|
| 🔍 | **진단 AI (RCA)** | 증상·알람 입력 → 추정 원인 Top3 + 신뢰도 + **근거 태그** + 유사 과거 케이스 |
| 🔧 | **복구 AI (HITL)** | 단계별 복구 가이드 · 안전 인터락 읽기전용 · **사람 승인 후** 조치 |
| 🧠 | **의미사전 (온톨로지)** | `M1234` → "실린더 전진 확인" 처럼 PLC 태그 의미를 매핑, **설비 간 재사용** ⭐해자 |
| 🗄️ | **데이터 레이어** | 온프렘 수집 커넥터 · 반출 통제 · 변경/조치 이력 감사 로깅 |
| 📊 | **대시보드 · KPI** | MTTR · MTBF · 다운타임 비용 · ROI 시각화 |
| 🏗️ | **플랫폼** | 멀티벤더 지원 · 구독 · 현장 대응 UI |

---

## 🧭 포지셔닝

> **예지보전(PdM)이 아닙니다.** 예지보전이 *"멈추기 전 예측"* 이라면, 도마는 *"이미 멈춘 라인을 빨리 살리는 지식 재사용 시스템"* 입니다.

예지보전이 **못 잡고**, 단일 벤더 플랫폼이 **안 품고**, SI가 **일회성으로만** 하는 자리 —
**멀티벤더 PLC 라인의 RCA(원인 진단) 운영자 도구.** 경쟁이 아니라 '빈틈'에 서는 전략입니다.

| 원칙 | 내용 |
|------|------|
| 🛡️ **HITL 기본** | AI는 '제안', 실행·승인은 '사람'. 안전 인터락 회로는 절대 건드리지 않습니다. |
| 🔎 **설명가능성** | 모든 추정에 근거 태그·케이스를 노출 — 신뢰가 쌓여야 확대합니다. |
| 🔒 **온프렘 우선** | 라인 데이터는 외부로 나가지 않습니다. 완전 로컬 모드 지원. |
| ♻️ **재사용이 곧 해자** | 첫 라인 구축물의 몇 %가 다음 라인에 그대로 가는지 — 이 수치를 KPI로 봅니다. |

---

## 📈 증명하려는 것 (수직 슬라이스 PoC)

<div align="center">

| 지표 | 목표 |
|------|:------:|
| ⏱️ **진단 시간** | `−80%` (약 4시간 → 30분 이내) |
| 🔁 **재조치율(재발·오진)** | `−30%` |
| 🙋 **주니어 단독 대응률** | `38% → 60%+` (베테랑 호출 없이 해결) |
| 🗂️ **의미사전 커버리지** | 고빈도 태그 `80%+` 매핑 |

</div>

---

## 🛠️ 기술 스택 (as-built)

<div align="center">

![Java](https://img.shields.io/badge/Java_21-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot_3-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL_+_pgvector-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker_Compose-2496ED?style=flat-square&logo=docker&logoColor=white)

</div>

- **백엔드** · Spring Boot 3 (Java 21) — RCA/복구/이력 API, RBAC, append-only 해시체인 감사
- **프런트** · React + TypeScript (Vite) — 현장 우선 데스크탑 UI (진단 → 복구 → 이력)
- **AI 추론** · Python FastAPI + LLM — RCA 파이프라인, 온톨로지 재사용 추론, 진단 품질 평가
- **데이터** · PostgreSQL + pgvector — 케이스 임베딩 유사검색(HNSW), 의미사전 지식그래프
- **수집** · PLC 더미 라인 시뮬레이터 — 실 PLC 없이 6스테이션 라인을 E2E로 검증
- **배포** · docker-compose 1커맨드 기동, 온프렘(망분리)

### 🏗️ 아키텍처

```
[PLC 라인 / 시뮬레이터]
        │  알람 push (ingest)
        ▼
[① 수집(Edge/온프렘)] ─→ [② 데이터·지식 계층]      의미사전(KG) · 벡터DB
        │                          │
        ▼                          ▼
[③ AI 추론(RCA)] ──────────→ [④ 애플리케이션(HITL UI)]
   근거 기반 추정원인            진단 · 복구 · 조치/감사 · 학습 환류
        │
        └── 횡단: 보안·권한(반출 통제) · 감사 추적 · HITL 승인 게이트
```

---

## 🚀 확장 로드맵

- **Phase 0 · 수직 슬라이스 PoC** — 1개 라인 / 시드 의미사전 / 진단→복구→이력 한 줄기 → KPI 증명
- **Phase 1 · 앵커 심화** — 다(多)라인 + 유료 전환, 멀티벤더 확장, 정답지·평가 루프 정착
- **Phase 2 · 레퍼런스 확산** — 동일 라인 구성 제조사, MES/SCADA 연동, KPI·ROI 대시보드 고도화
- **Phase 3 · 다운셀** — 2·3차 부품사 경량 온프렘/어플라이언스 구독, 저위험 자율복구(HITL 범위 확대)

> **로드맵 원칙:** 앵커로 신뢰·데이터·의미사전을 축적 → 복리 해자 → 저가 다운셀로 시장 확대.
> 기술 과투자보다 **검증된 수요를 따라 단계적으로 확장**합니다.

---

<div align="center">

**도마 · DOMA**

*PLC가 풀지 못한 단 하나 — 운영·진단·복구의 비용을 풉니다.*

</div>
