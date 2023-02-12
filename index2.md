---
title: CyberBookDocs
---

<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>{{title}}</title>
</head>

{% assign doclist = site.data.navigation.docs | sort: 'title'  %}
<ol>
{% for item in doclist %}
    <li><a href="{{ item.url }}">{{ item.title }}</a></li>
{% endfor %}
</ol>

</html>