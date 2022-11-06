---
title: 短文
type: 短文
noDate: 'true'
comments: 'false'
aside: false
---


{% note success %}
短文内容来自 乔一禾 的自言自语。🤪🤪
{% endnote %}
<div id='speak'>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/kuole-o/bber-ispeak@main/dist/ispeak-bber.min.js" charset="utf-8" ></script>
<script>
ispeakBber
    .init({
        el: '#speak', // 容器选择器
        name: '乔一禾 🦄', // 显示的昵称
        envId: 'cloudbase-baas-6g56sw0n48c42844', // 环境id
        region: 'ap-shanghai', // 腾讯云地址，默认为上海
        limit: 7, // 每次加载的条数，默认为5
        avatar: 'https://www.yyisq.com/img/avtar.webp', // 头像地址
        fromColor:'rgb(245, 150, 170)', // 下方标签背景颜色 默认 rgb(245, 150, 170)
        loadingImg: 'https://7.dusays.com/2021/03/04/d2d5e983e2961.gif', // 自定义loading的图片，示例值为默认值
        dbName:'talks' // 数据的名称，默认talks，避免有人的命名不是这个，所以加入此配置字段。
    })
    .then(function() {
        // 哔哔加载完成后的回调函数，你可以写你自己的功能
        console.log('哔哔 加载完成')
    })
</script>
</div>