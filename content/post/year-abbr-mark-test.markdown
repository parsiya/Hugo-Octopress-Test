---
title: "Year Abbr Mark Test"
date: 2019-09-02T11:34:36-07:00
categories:
- test
- category5
tags:
- year
- abbr
- mark
---

[year](https://github.com/parsiya/Hugo-Shortcodes#year-yearhtml) shortcode:

This should display the current year: `{{< year >}}`

----------

[abbr](https://github.com/parsiya/Hugo-Shortcodes#abbr-html-tag-abbrhtml) shortcode:

This should create an `abbr` tag with title of `World Health Organization` and 
text of `WHO`.

{{< abbr title="World Health Organization" text="WHO" >}}

----------

This should highlight the work `this part is highlighted` in the following text:

This is some text, {{< mark text="this part is highlighted" >}} and this part
is not.

<!--more-->