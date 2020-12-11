# InnoRules User's Guide of Rule Builder

![CI](https://github.com/rundocs/jekyll-rtd-theme/workflows/CI/badge.svg?branch=develop)
![jsDelivr](https://data.jsdelivr.com/v1/package/gh/rundocs/jekyll-rtd-theme/badge)

Just another documentation theme compatible with GitHub Pages

## 제 1장. 룰 문법

이 장에서는 InnoRules 룰 문법을 구성하는 기본 사항과, 룰 내용 작성에 필요한 룰 표현식 기술 문법에 대해 설명한다.

- 룰을 구성하는 룰 식별자, 룰 템플릿, 룰 버전, 룰 리턴, 룰 표현식 등
- 룰 표현식의 구성 요소
- 룰 표현식의 구성 요소와 룰 표현식의 실행 결과가 가지는 데이터 타입과 데이터 형식
- 룰과 룰 표현식의 작성 규칙

## 1. 기본 사항

업무 분석을 통해 도출된 하나의 비즈니스 룰은, 문법 규칙이나 재활용, 성능, 유지보수 효율성 등을 고려하여, InnoRules 룰 시스템(이하 InnoRules 또는 룰 시스템)에서의 최소 정의 단위인 룰로 분해되고, 이들 룰 간 일련의 호출 및 결과 참조, 연산 등을 통해 구현된다.

## Usage

Documentation that can guide how to create with Github pages, please refer to [rundocs.io](https://rundocs.io) for details

## Features

- Shortcodes (Toasts card, mermaid)
- Pages Plugins (emoji, gist, avatar, mentions)
- Auto generate sidebar
- [Attribute List Definitions](https://kramdown.gettalong.org/syntax.html#attribute-list-definitions) (Primer/css utilities, Font Awesome 4)
- Service worker (caches)
- SEO (404, robots.txt, sitemap.xml)
- Canonical Link (Open Graph, Twitter Card, Schema data)

## Options

| name          | default value        | description       |
| ------------- | -------------------- | ----------------- |
| `title`       | repo name            |                   |
| `description` | repo description     |                   |
| `url`         | user domain or cname |                   |
| `baseurl`     | repo name            |                   |
| `lang`        | `en`                 |                   |
| `direction`   | `auto`               | `ltr` or `rtl`    |
| `highlighter` | `rouge`              | Cannot be changed |

```yml
# folders sort
readme_index:
  with_frontmatter: true

meta:
  key1: value1
  key2: value2
  .
  .
  .

google:
  gtag:
  adsense:

mathjax: # this will prased to json, default: {}

mermaid:
  custom:     # mermaid link
  initialize: # this will prased to json, default: {}

scss:   # also _includes/extra/styles.scss
script: # also _includes/extra/script.js

translate:
  # shortcodes
  danger:
  note:
  tip:
  warning:
  # 404
  not_found:
  # copyright
  revision:
  # search
  searching:
  search:
  search_docs:
  search_results:
  search_results_found: # the "#" in this translate will replaced with results size!
  search_results_not_found:

plugins:
  - jemoji
  - jekyll-avatar
  - jekyll-mentions
```

## The license

The theme is available as open source under the terms of the MIT License
