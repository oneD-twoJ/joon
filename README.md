# joon — 가상 생산기술 사무실

AI 직원 7명이 일하는 가상 사무실입니다. Claude Code에서 이 저장소를 열고 말로 업무를 지시하면,
**실장(메인 Claude)** 이 알맞은 직원에게 배정하고 결과를 두괄식으로 보고합니다.

## 직원 명단

| 직원 | 직함 | 이런 일을 시키세요 |
|---|---|---|
| `process-engineer` | 공정기술 과장 | 병목 찾기, CT 단축, 라인 밸런싱, OEE |
| `equipment-analyst` | 설비보전 과장 | CMMS 고장 이력 분석, MTBF/MTTR, RCA, PM 계획 |
| `quality-engineer` | 품질 과장 | 불량 원인, Cpk/SPC, 8D, FMEA |
| `cost-analyst` | 원가기획 대리 | 원가 절감안, 투자 ROI, 회수기간 |
| `npi-manager` | NPI PM | 신제품 일정, APQP/PPAP, 이슈 트래킹 |
| `automation-dev` | 자동화 담당 | VBA 매크로, Python 스크립트 |
| `report-writer` | 기획 대리 | 보고서, PPT 구성안, Notion 문서 |

## 사용법

**방법 1 — 바로 말하기**
```
품질과장한테 office/data/불량이력.csv 분석시켜줘
설비과장이랑 원가대리 같이 붙여서 3번 로봇 교체 vs 수리 비교해줘
```

**방법 2 — 업무지시서**
1. `office/templates/업무지시서.md` → `office/inbox/` 에 복사해 작성
2. 데이터는 `office/data/` 에 넣기
3. "inbox 업무 처리해줘"

결과물은 `office/outputs/날짜_업무명/` 에 저장됩니다. 운영 규칙은 [`CLAUDE.md`](CLAUDE.md) 참고.
