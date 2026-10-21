# Heroeki

> **Disclaimer / 고지**
>
> This is a **non-commercial, educational project** built as a school assignment to practice web app development.
> It is a learning exercise **inspired by the design of the "My Routines" app** and is **not affiliated with, endorsed by, or connected to** the developers of My Routines in any way.
> All code and visual assets in this repository were **written from scratch** for learning purposes; no source code, images, icons, or other assets from the original app were used.
> "My Routines" and its logo are trademarks of their respective owner. This project is not distributed on any app store and must not be used for commercial purposes.
>
> 이 프로젝트는 웹 앱 개발을 연습하기 위해 만든 **비상업적 학습용 과제**입니다.
> **"My Routines" 앱의 디자인을 참고**하여 UI를 직접 구현해 본 것으로, **해당 앱의 개발사와 어떠한 관련도 없습니다.**
> 이 저장소의 모든 코드와 시각 자산은 학습 목적으로 직접 작성·제작했으며, 원본 앱의 소스 코드·이미지·아이콘 등 어떤 자산도 사용하지 않았습니다.
> "My Routines" 및 로고의 권리는 해당 권리자에게 있습니다. 이 프로젝트는 앱스토어에 배포되지 않으며 상업적으로 사용할 수 없습니다.

## 소개

습관과 일과를 기록하고 통계로 돌아보는 웹 앱입니다. 설치 없이 브라우저에서 동작하며, 홈 화면에 추가하면 앱처럼 쓸 수 있습니다(PWA). 모든 데이터는 기기 안(IndexedDB)에만 저장되고 서버로 전송되지 않습니다.

## 기능

- 습관 4가지 방식: 체크 · 시간 · 수치 · 횟수
- 반복 주기: 매일 · 요일 지정 · 주간 목표 · 월간 목표
- 연속 달성(스트릭)과 하루 달성률
- 통계: 월간 · 주간 · 그린라이트 탭, 달력 보기
- 태그 · 필터 · 드래그로 순서 변경
- 이모지 아이콘 선택
- 설정: 달성 기준(기본 80%), 백업

## 기술

- 순수 HTML / CSS / JavaScript, 외부 라이브러리 없음
- IndexedDB 저장 (localStorage 폴백)
- `manifest.json` + Service Worker로 홈 화면 설치 및 오프라인 지원

## 파일 구성

```
routine.html    앱 전체 (HTML + CSS + JS)
manifest.json   PWA 설정
sw.js           Service Worker (오프라인 캐시)
icon-180.png    홈 화면 아이콘
```

## 실행

`routine.html`을 브라우저로 열거나, GitHub Pages에 올린 뒤 주소로 접속합니다.
아이폰 Safari에서는 **공유 → 홈 화면에 추가**로 설치할 수 있습니다.

## License

All rights reserved. This code is published for educational review only and may not be copied, modified, or redistributed.
