# 온디바이스AI 실습 가이드 (3차)

[인공지능] 피지컬AI의 기초를 위한 임베디드·온디바이스 실습 · 2026-11-28 ~ 29 · 김덕우 강사

**→ https://kdw335552.github.io/ondevice-ai/**

| 파일 | 내용 |
|---|---|
| `index.html` | 첫 화면 (1일차 · 2일차 고르기) |
| `day1.html` | 1일차 — 라즈베리파이 설치 · 실습 1~3 |
| `day2.html` | 2일차 — **11-29 08:30 KST 전에는 안내 페이지** |
| `day2.html.enc` | 진짜 2일차(암호화 본) — 08:30 뒤 배포 때 풀려서 `day2.html` 로 올라감 |
| `.github/workflows/pages.yml` | GitHub Pages 배포 (push · 예약 2회 · 수동 실행) |
| `.gitattributes` | `*.enc` 를 binary 로 (윈도우 줄바꿈 변환 방지) |

## 처음 한 번 설정 (저장소 주인)

1. Settings → Pages → Build and deployment → Source: **GitHub Actions**
2. Settings → Secrets and variables → Actions → New repository secret → 이름 **`DAY2_KEY`**, 값은 비공개 폴더의 `DAY2_KEY.txt` 내용
3. Actions 탭 → `pages` → **Run workflow** 한 번 → 초록색이면 위 주소로 열림

## 2일차 시간 잠금

- 예약 실행: UTC 11-28 23:30 · 23:50 (= KST 11-29 08:30 · 08:50). GitHub 예약은 늦게 돌 수 있습니다.
  08:30 이 지나도 안내 페이지면 Actions → `pages` → Run workflow 를 한 번 누르면 됩니다.
- 08:30 뒤에 `DAY2_KEY` 가 없으면 배포가 실패합니다(진짜 2일차가 잘못 공개되지 않음).

## 주의

- 수강생판만 넣었습니다. 강사판(`[실습 가이드 웹] …`)은 넣지 않습니다.
- GitHub Pages 주소는 저장소가 비공개여도 누구나 열 수 있습니다.
- 그림은 html 안에 들어 있어 따로 올릴 파일이 없습니다. 글꼴만 Google Fonts 에서 받습니다.
- 고칠 때는 `50_배포/_수업진행용_웹가이드/[수강생 실습 가이드] …` 를 고친 뒤
  `20_교안/HTML/261117_실습가이드/make_site.py` 로 이 폴더를 다시 만듭니다.
