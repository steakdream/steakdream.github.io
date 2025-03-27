---
title: "whatever Page"
layout: splash
permalink: /_pages/list
date: 2016-03-23T11:48:41-04:00
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/IMG_3846.JPG

excerpt: "Life is tough, and there are so many things I do not and cannot understand."
---

<!-- 在页面内容中直接插入 Gitalk 评论容器和初始化代码 -->
<div id="gitalk-container"></div>
<script type="text/javascript">
  window.onload = function() {
    var gitalk = new Gitalk({
      clientID: 'Ov23livLCw69zvvmm6ZD',
      clientSecret: '575ec7359cdcc9fa81ea3addd623f85f4c468737',
      repo: 'comments',
      owner: 'steakdream',
      admin: ['steakdream'],
      id: window.location.pathname,
      distractionFreeMode: false
    });
    gitalk.render('gitalk-container');
  }
</script>
