---
title: 友情链接
date: 2020-10-03 21:17:39
type: "links"
toc: false
---

------

<div class="links-content">
    <div class="link-navigation">
        {% for link in site.data.links %}
        <a href="{{ link.site }}" target="_blank">
        <div class="card">
            <img class="avatar nomediumzoom" src="{{ link.avatar }}" />
            <div class="card-header">
            <div class="link-name">{{ link.name }}</div>
            <div class="link-info">{{ link.info }}</div>
            </div>
        </div>
        </a>
        {% endfor %}
    </div>
</div>

------

(Last update: 2024-09-29)

如需添加链接或更新，请在评论区留言，或通过侧边栏（需要用电脑才能看到）中的联系方式私信我。

```
名称：Kevin Huang 的小站
链接：https://kevinh.wang/
简介：一个不太靠谱的「三无人士」
头像：Gravatar 头像 (huangyf9883@gmail.com)
```