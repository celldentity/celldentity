<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1e3a8a,100:0ea5e9&height=230&section=header&text=celldentity&fontSize=56&fontColor=ffffff&fontAlignY=34&desc=%EC%97%91%EC%85%80%EA%B3%BC%20%EC%A2%85%EC%9D%B4%EB%A1%9C%20%EB%8F%8C%EB%8D%98%20HR%C2%B7%EA%B2%BD%EC%98%81%EC%A7%80%EC%9B%90%20%EC%97%85%EB%AC%B4%EB%A5%BC%20%EC%A7%81%EC%A0%91%20%EB%A7%8C%EB%93%A0%20%EC%8B%9C%EC%8A%A4%ED%85%9C%EC%9C%BC%EB%A1%9C%20%EB%B0%94%EA%BF%89%EB%8B%88%EB%8B%A4&descAlignY=53&descSize=16" />

**HR·경영지원 실무자이면서, 그 업무를 자동화하는 시스템을 직접 만들어 운영합니다.**

[![Website](https://img.shields.io/badge/aibunker.kr-0ea5e9?style=for-the-badge&logo=vercel&logoColor=white)](https://aibunker.kr)
[![Gmail](https://img.shields.io/badge/ksb2116@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ksb2116@gmail.com)

</div>

---

## 👋 한눈에 보기

| | |
| --- | --- |
| **하는 일** | 제조업 HR·경영지원 실무 + 그 업무를 자동화하는 사내 포털 설계·개발·운영 |
| **강점** | 현업 요구를 개발자에게 전달하는 게 아니라, **문제를 아는 사람이 직접 화면과 DB까지** 만듭니다 |
| **대표 성과** | 사내 업무 포털 **HSMnT** — 근태·급여명세서·채용·입퇴사·생산 현장까지 하나의 시스템으로, 실제 업무에 사용 중 |
| **그 밖에** | 개인 서비스 [AI Bunker](https://aibunker.kr)를 기획부터 배포·운영까지 혼자 운영 중 |

## 🏭 HSMnT — 사내 경영지원·생산 통합 포털 *(비공개 · 업무 시스템)*

흩어진 엑셀·종이·여러 시스템을 **한 곳의 데이터(DB)로 모으고, 그 위에서 일하게** 만들었습니다.

| 업무 | 어떻게 바꿨나 |
| --- | --- |
| **근태·연차** | 업무일지를 매일 DB에 적재하고, 화면 숫자가 엑셀 수식 결과와 같은지 자동 대조 |
| **급여명세서** | 사원이 모바일로 본인 내역 확인. PDF는 근태 서명 후에만 내려받도록 서버에서 검증 |
| **채용·수습평가** | 직무별 기준표로 이력서 스크리닝, 부서장·인사 평가를 합산하는 수습평가, 면접 기록 |
| **입사·퇴사** | 신규 입사자의 조직도·비상연락망·좌석 자동 반영, 퇴직 체크리스트 → 본인 작성 → 부서장 전자결재 |
| **사원 소통** | 웹 푸시 공지, 모바일 사원포털, 정기 행사·건강검진 안내 |
| **규정·법령** | 취업규칙·급여규정 열람, 퇴직금 기간 산정, 외국인 체류자격별 처리 가이드 |
| **생산 현장** | 설비 태블릿 포털, 도면 관리(DWG 미리보기), 작업·재고 장부 |

### HR 실무자라서 다르게 만든 것

- **법정 기준부터 계산합니다.** 채용공고 급여를 "사내 자료와 일치"만 보고 올렸다가 최저임금 기준(주휴수당 누락)으로 반려된 적이 있습니다. 그 뒤로 외부에 나가는 숫자는 법정 하한을 먼저 검산하는 규칙을 만들었습니다.
- **재직 여부는 상태가 아니라 날짜로 판단합니다.** 퇴직 "예정"을 미리 입력해도 퇴직일 전에는 재직자로 취급합니다. 상태값만 믿었다가 아직 근무 중인 사람이 집계에서 빠진 사고에서 나온 설계입니다.
- **엑셀은 재료, DB가 원장입니다.** 엑셀을 한 번 옮겨 적재하고 나면 이후 모든 화면·집계는 DB만 봅니다.
- **개인정보는 열어 두지 않습니다.** 민감 컬럼 암호화, 서류는 비공개 저장소 + 2분짜리 임시 주소로만, 화면별 권한은 서버가 검사합니다.

기술 구조와 운영 방식(배포·백업·권한 감사)은 **[PROJECTS.md](PROJECTS.md)** 에 정리했습니다.

## 🤝 일하는 방식

- **AI 코딩 에이전트(Claude Code)와 협업합니다.** 무엇을 만들지, 결과가 맞는지의 판단과 검증은 제가 하고, 사고가 날 때마다 **재발 방지 규칙을 문서와 스크립트로 남깁니다.**
- **배포했다고 끝내지 않고, 실제로 뜨는지 확인합니다.** 빌드 성공과 서비스 정상은 다르다는 걸 장애로 배웠고, 배포 후 헬스 체크를 직접 합니다.
- **혼자 만들고 혼자 운영합니다.** 기획 → 개발 → 배포 → 운영 → 사용자 문의 대응까지 한 사람이 끝까지 돕니다.

## 🧪 그 밖의 프로젝트

| 프로젝트 | 설명 |
| --- | --- |
| **[AI Bunker](https://aibunker.kr)** | 갤러리·블로그·캘린더·GIS·타자 게임·심리 검사·가계부 등 25개+ 기능을 한 앱으로 묶은 개인 포털. 서버리스(Vercel) + DB 운영, 로그인 무차별 대입 방어, DB 전체 백업·권한 감사 스크립트 (커밋 1,800+) |
| **[drivelog](https://github.com/celldentity/drivelog)** | 안드로이드 1초 단위 주행 기록 → CSV/JSON 내보내기 앱. GitHub Actions로 APK 자동 빌드 |
| **[crack_project](https://github.com/celldentity/crack_project)** | YOLO 기반 포트홀 감지 PWA. 촬영 → 추론 → 위치 기록까지 구현 |

<details>
<summary><b>🛠 사용 기술</b> (펼치기)</summary>

<table>
<tr>
<td align="right" width="110"><b>Backend</b></td>
<td width="56" align="center"><a href="https://www.python.org" title="Python"><img src="https://skillicons.dev/icons?i=py&theme=dark" width="40" height="40" /></a></td>
<td width="56" align="center"><a href="https://flask.palletsprojects.com" title="Flask"><img src="https://skillicons.dev/icons?i=flask&theme=dark" width="40" height="40" /></a></td>
<td width="56" align="center"><a href="https://www.mysql.com" title="MySQL"><img src="https://skillicons.dev/icons?i=mysql&theme=dark" width="40" height="40" /></a></td>
<td width="56"></td>
</tr>
<tr>
<td align="right" width="110"><b>Frontend</b></td>
<td width="56" align="center"><a href="https://developer.mozilla.org/docs/Web/HTML" title="HTML5"><img src="https://skillicons.dev/icons?i=html&theme=dark" width="40" height="40" /></a></td>
<td width="56" align="center"><a href="https://developer.mozilla.org/docs/Web/CSS" title="CSS3"><img src="https://skillicons.dev/icons?i=css&theme=dark" width="40" height="40" /></a></td>
<td width="56" align="center"><a href="https://developer.mozilla.org/docs/Web/JavaScript" title="JavaScript"><img src="https://skillicons.dev/icons?i=js&theme=dark" width="40" height="40" /></a></td>
<td width="56" align="center"><a href="https://getbootstrap.com" title="Bootstrap"><img src="https://skillicons.dev/icons?i=bootstrap&theme=dark" width="40" height="40" /></a></td>
</tr>
<tr>
<td align="right" width="110"><b>Frontend (SPA)</b></td>
<td width="56" align="center"><a href="https://www.typescriptlang.org" title="TypeScript"><img src="https://skillicons.dev/icons?i=ts&theme=dark" width="40" height="40" /></a></td>
<td width="56" align="center"><a href="https://react.dev" title="React"><img src="https://skillicons.dev/icons?i=react&theme=dark" width="40" height="40" /></a></td>
<td width="56" align="center"><a href="https://vitejs.dev" title="Vite"><img src="https://skillicons.dev/icons?i=vite&theme=dark" width="40" height="40" /></a></td>
<td width="56" align="center"><a href="https://tailwindcss.com" title="Tailwind CSS"><img src="https://skillicons.dev/icons?i=tailwind&theme=dark" width="40" height="40" /></a></td>
</tr>
<tr>
<td align="right" width="110"><b>Mobile</b></td>
<td width="56" align="center"><a href="https://kotlinlang.org" title="Kotlin"><img src="https://skillicons.dev/icons?i=kotlin&theme=dark" width="40" height="40" /></a></td>
<td width="56" align="center"><a href="https://developer.android.com/studio" title="Android Studio"><img src="https://skillicons.dev/icons?i=androidstudio&theme=dark" width="40" height="40" /></a></td>
<td width="56"></td>
<td width="56"></td>
</tr>
<tr>
<td align="right" width="110"><b>AI / Data</b></td>
<td width="56" align="center"><a href="https://opencv.org" title="OpenCV"><img src="https://skillicons.dev/icons?i=opencv&theme=dark" width="40" height="40" /></a></td>
<td width="56" align="center"><a href="https://firebase.google.com" title="Firebase"><img src="https://skillicons.dev/icons?i=firebase&theme=dark" width="40" height="40" /></a></td>
<td width="56"></td>
<td width="56"></td>
</tr>
<tr>
<td align="right" width="110"><b>Infra</b></td>
<td width="56" align="center"><a href="https://vercel.com" title="Vercel"><img src="https://skillicons.dev/icons?i=vercel&theme=dark" width="40" height="40" /></a></td>
<td width="56" align="center"><a href="https://www.docker.com" title="Docker"><img src="https://skillicons.dev/icons?i=docker&theme=dark" width="40" height="40" /></a></td>
<td width="56" align="center"><a href="https://cloud.google.com" title="Google Cloud"><img src="https://skillicons.dev/icons?i=gcp&theme=dark" width="40" height="40" /></a></td>
<td width="56" align="center"><a href="https://www.cloudflare.com" title="Cloudflare"><img src="https://skillicons.dev/icons?i=cloudflare&theme=dark" width="40" height="40" /></a></td>
</tr>
<tr>
<td align="right" width="110"><b>Tools</b></td>
<td width="56" align="center"><a href="https://git-scm.com" title="Git"><img src="https://skillicons.dev/icons?i=git&theme=dark" width="40" height="40" /></a></td>
<td width="56" align="center"><a href="https://github.com" title="GitHub"><img src="https://skillicons.dev/icons?i=github&theme=dark" width="40" height="40" /></a></td>
<td width="56" align="center"><a href="https://code.visualstudio.com" title="Visual Studio Code"><img src="https://skillicons.dev/icons?i=vscode&theme=dark" width="40" height="40" /></a></td>
<td width="56"></td>
</tr>
</table>

<sub>아이콘이 없는 것들 — <a href="https://www.pingcap.com/tidb/"><b>TiDB</b></a>(MySQL 호환 분산 DB) · <b>SQLAlchemy</b> · <b>TanStack Query</b> · <b>Cloudflare R2</b>(오브젝트 스토리지) · <b>Web Push</b> · <a href="https://docs.ultralytics.com"><b>YOLO</b></a> · <a href="https://ai.google.dev"><b>Gemini API</b></a> · <a href="https://www.oracle.com/cloud/"><b>Oracle Cloud</b></a> · <a href="https://www.atlassian.com/software/jira"><b>Jira</b></a></sub>

</details>

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0ea5e9,100:1e3a8a&height=120&section=footer" />

</div>
