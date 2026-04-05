# Interstellagram

GitHub Pages에서 바로 배포할 수 있는 Jekyll 기반 개인 블로그입니다.

## 글 쓰는 방법

`_posts` 폴더에 아래 형식으로 Markdown 파일을 추가합니다.

```text
YYYY-MM-DD-title.md
```

예시:

```text
2026-04-06-my-post.md
```

파일 상단에는 front matter를 넣습니다.

```yaml
---
title: "글 제목"
date: 2026-04-06 12:00:00 +0900
description: "짧은 소개"
---
```

## 배포

이 저장소에는 GitHub Pages 배포용 워크플로가 포함되어 있습니다.

1. GitHub 저장소에 푸시합니다.
2. GitHub 저장소의 `Settings > Pages`에서 소스를 `GitHub Actions`로 맞춥니다.
3. `main` 브랜치에 푸시하면 자동 배포됩니다.
4. 몇 분 뒤 `https://kjs36202.github.io` 에서 사이트를 확인합니다.

## 로컬 미리보기

Ruby와 Bundler가 설치되어 있다면 아래 순서로 확인할 수 있습니다.

```bash
bundle install
bundle exec jekyll serve
```

참고로 현재 이 작업 환경의 Ruby는 `2.6.10`이라 최신 `github-pages` gem 의존성 설치가 실패했습니다. 로컬 미리보기가 필요하면 Ruby를 더 최신 버전으로 올린 뒤 실행하는 편이 안전합니다.
