<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1e3a8a,100:0ea5e9&height=230&section=header&text=celldentity&fontSize=56&fontColor=ffffff&fontAlignY=34&desc=%EC%9D%B8%EC%82%AC%C2%B7%EC%B4%9D%EB%AC%B4%20%EC%9D%BC%EC%9D%84%20%ED%95%98%EB%8B%A4%EA%B0%80%2C%20%EB%B0%98%EB%B3%B5%EB%90%98%EB%8A%94%20%EC%9D%BC%EC%9D%84%20%EC%A7%81%EC%A0%91%20%EB%A7%8C%EB%93%A4%EC%96%B4%20%EC%97%86%EC%95%A0%EA%B3%A0%20%EC%9E%88%EC%8A%B5%EB%8B%88%EB%8B%A4&descAlignY=53&descSize=16" />

[![Website](https://img.shields.io/badge/aibunker.kr-0ea5e9?style=for-the-badge&logo=vercel&logoColor=white)](https://aibunker.kr)
[![Gmail](https://img.shields.io/badge/ksb2116@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ksb2116@gmail.com)

<img src="assets/commit-tree.gif" width="360" alt="커밋이 쌓이며 자라는 나무 (직접 만든 3D 모션)" />

</div>

---

## 소개

인사·총무 일을 하는 사람입니다. 매달 같은 엑셀을 열고, 같은 숫자를 옮겨 적고, 같은 안내를 사람마다 따로 보내는 일이 쌓여서 직접 만들기 시작했습니다.

지금은 회사에서 쓰는 업무 포털(HSMnT)을 혼자 만들고 운영하고 있고, 개인 서비스인 AI Bunker도 같이 돌리고 있습니다.

## HSMnT — 회사에서 실제로 쓰는 업무 포털 *(비공개)*

엑셀과 종이로 흩어져 있던 일을 한 시스템에 올렸습니다. 업무별로 이렇게 바뀌었습니다.

| 업무 | 바뀐 점 |
| --- | --- |
| 근태·연차 | 업무일지를 매일 DB에 옮겨 담고, 화면 숫자가 엑셀 수식 결과와 같은지 자동으로 맞춰 봅니다 |
| 급여명세서 | 사원이 모바일로 본인 내역을 봅니다. PDF는 근태 서명을 마친 사람만 받을 수 있습니다 |
| 채용·수습평가 | 직무별 기준표로 이력서를 거르고, 수습 기간에는 부서장과 인사 평가를 합산합니다. 면접 내용도 기록해 둡니다 |
| 입사·퇴사 | 신규 입사자는 조직도·비상연락망·좌석에 자동으로 들어가고, 퇴직자는 체크리스트를 쓰면 부서장 결재로 넘어갑니다 |
| 사원 안내 | 웹 푸시로 공지하고, 행사·건강검진 같은 안내는 사원포털에 올립니다 |
| 규정·법령 | 취업규칙·급여규정을 바로 찾아 보고, 퇴직금 기간 계산과 외국인 체류자격별 처리 방법을 정리해 뒀습니다 |
| 생산 현장 | 설비에 붙은 태블릿으로 작업을 걸고 끝내고, 도면과 재고도 같이 봅니다 |

### 겪고 나서 바꾼 것

채용공고에 월급을 적어 올렸다가 최저임금 기준 위반으로 반려된 적이 있습니다. 주휴수당을 빼고 계산한 게 원인이었습니다. 사내 자료와 맞는지만 확인했지, 법정 하한은 따져 보지 않았던 겁니다. 그 뒤로는 밖으로 나가는 숫자는 법 기준부터 계산합니다.

퇴사 예정자를 시스템에 미리 입력해 뒀더니, 아직 퇴직일이 안 지난 사람이 로그인도 안 되고 재직 인원에서도 빠진 일이 있었습니다. 지금은 입사일과 퇴직일만 보고 재직 여부를 정합니다. 상태값은 입력용으로만 씁니다.

엑셀은 한 번 DB로 옮겨 담고 나면 다시 열지 않습니다. 그다음부터는 모든 화면과 집계가 DB만 봅니다. 민감한 항목은 암호화하고, 개인 서류는 2분짜리 임시 주소로만 내려줍니다.

구조와 운영 방식(배포, 백업, 권한 점검)은 [PROJECTS.md](PROJECTS.md)에 적어 두었습니다.

## 일하는 방식

Claude Code 같은 AI 코딩 도구와 같이 일합니다. 무엇을 만들지, 결과가 맞는지는 제가 정하고 확인합니다. 배포한 뒤에는 대시보드가 아니라 실제 주소를 직접 열어 보고, 문제가 생기면 같은 일이 반복되지 않도록 규칙이나 스크립트로 남겨 둡니다.

## AI Bunker

<a href="https://aibunker.kr"><img src="assets/ai-bunker.gif" width="360" align="right" alt="AI Bunker 로고가 흩어졌다 모이는 3D 모션" /></a>

갤러리, 블로그, 일기, 캘린더, 지도, 타자 연습, 리듬 게임, 심리 검사, 가계부 같은 걸 한 앱에 담은 개인 서비스입니다. 기획부터 배포, 운영까지 혼자 하고 있습니다.

바로 써 볼 수 있습니다 → [aibunker.kr](https://aibunker.kr) · [타자 연습](https://aibunker.kr/typing)

<br clear="all" />

## 그 밖의 프로젝트

| 프로젝트 | 설명 |
| --- | --- |
| [drivelog](https://github.com/celldentity/drivelog) | 안드로이드로 1초 단위 주행을 기록해 CSV/JSON으로 내보내는 앱. GitHub Actions로 APK를 자동 빌드합니다 |
| [crack_project](https://github.com/celldentity/crack_project) | YOLO로 도로 포트홀을 찾는 PWA. 촬영, 추론, 위치 기록까지 만들었습니다 |

<details>
<summary>사용 기술 (펼치기)</summary>

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
