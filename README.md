# Jekyll 개인 블로그

Jekyll과 GitHub Pages를 사용한 개인 블로그입니다. 다국어 지원(한국어/영어)과 다크모드 기능을 포함하고 있습니다.

## ✨ 주요 기능

- 📱 **반응형 디자인**: 모든 기기에서 최적화된 경험
- 🌙 **다크모드**: 라이트/다크 모드 자동 전환
- 🌍 **다국어 지원**: 한국어와 영어 지원
- ⚡ **빠른 로딩**: 정적 사이트로 매우 빠른 속도
- 🔍 **SEO 최적화**: 검색 엔진 최적화 적용
- 📝 **마크다운 글쓰기**: 간편한 마크다운 문법 지원
- 🎨 **코드 하이라이팅**: 다양한 언어의 코드 강조 표시

## 🚀 빠른 시작

### 1. 저장소 생성
GitHub에서 `username.github.io` 형태의 저장소를 생성합니다.

### 2. 코드 복사
이 프로젝트의 모든 파일을 생성한 저장소에 복사합니다.

### 3. 설정 수정
`_config.yml` 파일에서 다음 정보를 수정합니다:

```yaml
title: "내 블로그 제목"
description: "블로그 설명"
url: "https://your-username.github.io"
github_username: your-username
email: your-email@example.com
```

### 4. GitHub Pages 활성화
1. GitHub 저장소 → Settings → Pages
2. Source를 "GitHub Actions"로 설정

### 5. 푸시하기
```bash
git add .
git commit -m "Initial commit"
git push origin main
```

## 🛠 로컬 개발

### 필요 조건
- Ruby 3.0 이상
- Bundler

### 설치 및 실행
```bash
# 의존성 설치
bundle install

# 개발 서버 실행
bundle exec jekyll serve --livereload

# 브라우저에서 http://localhost:4000 접속
```

## 📝 글 작성하기

### 새 포스트 생성
`_posts/` 디렉토리에 다음 형식으로 파일을 생성합니다:
```
YYYY-MM-DD-title.md
```

### 포스트 헤더 예시
```yaml
---
layout: post
title: "포스트 제목"
date: 2024-01-01 10:00:00 +0900
categories: [category1, category2]
tags: [tag1, tag2, tag3]
lang: ko
author: "작성자 이름"
excerpt: "포스트 요약"
---

포스트 내용을 여기에 작성합니다...
```

## 🌍 다국어 지원

### 번역 추가
`_data/translations.yml` 파일을 수정하여 새로운 번역을 추가할 수 있습니다.

### 언어별 포스트
포스트의 front matter에 `lang: ko` 또는 `lang: en`을 추가합니다.

## 🎨 커스터마이징

### 색상 변경
`_sass/_variables.scss` 파일에서 색상을 수정할 수 있습니다:

```scss
$primary-color: #2c3e50;      // 기본 색상
$secondary-color: #3498db;    // 강조 색상
$background-color: #ffffff;   // 배경 색상
```

### 폰트 변경
`_sass/_variables.scss`에서 폰트를 수정할 수 있습니다:

```scss
$base-font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
```

## 📁 프로젝트 구조

```
├── _config.yml           # Jekyll 설정 파일
├── _data/
│   └── translations.yml  # 다국어 번역 데이터
├── _includes/
│   ├── header.html       # 헤더 컴포넌트
│   └── footer.html       # 푸터 컴포넌트
├── _layouts/
│   ├── default.html      # 기본 레이아웃
│   └── post.html         # 포스트 레이아웃
├── _posts/               # 블로그 포스트 디렉토리
├── _sass/                # SCSS 스타일 파일들
├── assets/
│   ├── css/
│   │   └── style.scss    # 메인 스타일 파일
│   └── js/
│       └── main.js       # JavaScript 파일
├── .github/
│   └── workflows/
│       └── pages.yml     # GitHub Actions 워크플로우
├── index.html            # 메인 페이지
├── about.md              # 소개 페이지
├── Gemfile               # Ruby 의존성 파일
└── .gitignore            # Git 무시 파일
```

## 🔧 고급 설정

### SEO 최적화
- `jekyll-seo-tag` 플러그인이 자동으로 SEO 메타 태그를 생성합니다
- 각 포스트에 `excerpt` 필드를 추가하여 검색 결과에 표시될 요약을 설정할 수 있습니다

### RSS 피드
- `jekyll-feed` 플러그인이 자동으로 RSS 피드를 생성합니다
- `/feed.xml`에서 확인할 수 있습니다

### 사이트맵
- `jekyll-sitemap` 플러그인이 자동으로 사이트맵을 생성합니다
- `/sitemap.xml`에서 확인할 수 있습니다

## 📧 문의

궁금한 점이나 개선 제안이 있으시면 언제든 연락해 주세요!

---

⭐ 이 프로젝트가 도움이 되었다면 별점을 눌러주세요! 