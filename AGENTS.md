# AGENTS.md

## 프로젝트 개요

사무자동화산업기사 실기 시험 대비 정적 학습 사이트. 2026년 개정 출제기준 반영.

## 기술 스택

- 단일 HTML 파일 (`index.html`), 별도 빌드/의존성 없음
- 순수 HTML/CSS/JS (프레임워크 없음)
- 브라우저에서 직접 열거나 정적 서버로 서빙

## 실행 방법

```bash
# 로컬 서버 (선택)
python -m http.server 8000
# 또는
npx serve .

# 파일 직접 열기
start index.html
```

## 구조

- `index.html` — 모든 콘텐츠와 로직이 단일 파일에 포함
- 콘텐츠는 상수 객체(`questionDB`)로 관리

## 수정 시 주의사항

- 문제 데이터는 `questionDB` 객체 내 `category` 키로 분류 (`excel`, `access`, `powerpoint`, `sql`, `hw`, `automation`)
- 사용자는 개발자 출신, SQL 익숙, 엑셀 함수 약함 → 엑셀 함수 콘텐츠 우선 유지
- 사이트 언어: 한국어
- 스타일은 인라인 CSS, 스크립트는 인라인 JS
