---
title: 友链
date: 2020-10-03 21:17:39
---

<div class="links-content">
<div class="link-navigation">
{% for link in site.data.links %}
<div class="card"><img class="ava nomediumzoom" src="{{ link.avatar }}"/>
<div class="card-header">
<div><a href="{{ link.site }}" target="_blank"> {{ link.name }}</a> </div>
<div class="info">{{ link.info }}</div>
</div>
</div>
{% endfor %}
</div>

<div id="qexo-friends"></div>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/qexo-static@1.1.3/hexo/friends/friends.css"/>
<script src="https://cdn.jsdelivr.net/npm/qexo-static@1.1.3/hexo/friends/friends.js"></script>
<script>loadQexoFriends("qexo-friends", "https://qexo.kevinh.wang")</script>

(Last update: 2024-09-28)

如需添加链接或更新，请在下方留言，或者 [私聊我](https://kevinh.wang/about/)。

## 本站信息
```
名称：Kevin Huang 的小站
链接：https://kevinh.wang/
简介：一个不太靠谱的「三无人士」
头像：Gravatar 头像 (huangyf9883@gmail.com)
```