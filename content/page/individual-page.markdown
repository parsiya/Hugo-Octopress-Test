---
date: "2018-01-01T20:35:00-04:00"
draft: false
title: "Individual Page"
url: "/page1"
categories:
- test
- category1
tags:
- tag1
toc: false
---

This is an individual page.

1. Make a new file in `content\page`. For example: `content\page\mypage.markdown`.
2. Add frontmatter, URL can be designated in frontmatter. For example this page has `url: "/page1/"`.
    * Alternatively, create the page anywhere inside `content` and set the type of it to `page` in frontmatter `type: page`.

URL of page can be set in the frontmatter with `url: "/page1/"`. If this URL is not set, page is created at `baseURL/page/file-name/`.