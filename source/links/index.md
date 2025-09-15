---
title: 友情链接
date: 2020-10-03 21:17:39
type: "links"
toc: false
---

------

<div class="links-content">
    <div class="link-navigation" id="friendLinks">
        <!-- 友情链接将通过 JavaScript 动态加载 -->
    </div>
</div>

<script>
document.addEventListener('DOMContentLoaded', function() {
    // 友情链接数据
    const links = [
        {
            name: '風雪城',
            info: '浩繁星空下的一场稚嫩的梦',
            site: 'https://blog.chyk.ink/',
            avatar: 'https://q1.qlogo.cn/g?b=qq&nk=3526514925&s=640'
        }, 
        {
            name: 'dasasdhba',
            info: 'Moonstruck Blossom',
            site: 'https://dasasdhba.github.io/',
            avatar: 'https://kevinh.wang/img/friends/dasasdhba.jpg'
        },
        {
            name: 'WSW 的小屋',
            info: 'WSW 的个人空间',
            site: 'https://zh.wsw233.com/',
            avatar: 'https://kevinh.wang/img/friends/wsw.jpg'
        },
    ];

    const container = document.getElementById('friendLinks');
    
    links.forEach(function(link) {
        // 创建可点击的链接容器
        const linkElement = document.createElement('a');
        linkElement.href = link.site;
        linkElement.target = '_blank';
        linkElement.style.textDecoration = 'none';
        linkElement.style.color = 'inherit';
        
        // 创建卡片元素
        const cardElement = document.createElement('div');
        cardElement.className = 'card';
        
        // 创建图片元素
        const imgElement = document.createElement('img');
        imgElement.className = 'avatar nomediumzoom';
        imgElement.src = link.avatar;
        
        // 添加图片加载失败的 fallback
        imgElement.onerror = function() {
            this.src = '/images/error.gif';
            this.onerror = null; // 防止无限循环
        };
        
        // 创建头像信息容器
        const headerElement = document.createElement('div');
        headerElement.className = 'card-header';
        headerElement.innerHTML = 
            '<div class="link-name">' + link.name + '</div>' +
            '<div class="link-info">' + link.info + '</div>';
        
        // 组装卡片
        cardElement.appendChild(imgElement);
        cardElement.appendChild(headerElement);
        linkElement.appendChild(cardElement);
        container.appendChild(linkElement);
    });
});
</script>

------

(Last update: 2024-09-29)

如需添加链接或更新，请在评论区留言，或通过侧边栏中的联系方式私信我。

```
名称：Kevin Huang 的小站
链接：https://kevinh.wang/
简介：一个不太靠谱的「三无人士」
头像：Gravatar 头像 (huangyf9883@gmail.com)
```