---
title: 読書フォルダ
---

<link href="https://satoshi-numata.github.io/notes/custom.css" rel="stylesheet">
<link href="https://use.fontawesome.com/releases/v6.7.2/css/all.css" rel="stylesheet">

## 読書フォルダ | 沼田 哲史のノート

このフォルダでは、読書に関するトピックを扱います。
深く読書を楽しむための工夫、おすすめの本や本の感想などを記事として公開していきます。

### コンテンツ一覧

<ul>
  {% for page in site.pages %}
    {% if page.path contains 'reading/' and page.path != 'reading/index.md' and page.name == 'index.md' %}
      <li><a href="{{ site.baseurl }}{{ page.url }}">{{ page.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>
