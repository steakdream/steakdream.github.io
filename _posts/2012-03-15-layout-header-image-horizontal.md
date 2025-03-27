---
title: "Layout"
header:
  image: /assets/images/unsplash-image-1.jpg
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
tags:

author_profile: false
share: false
---

This post should display a **header image**, if the theme supports it.

Non-square images can provide some unique styling issues.

<div id="gitalk-container"></div>

<script type="text/javascript">
  window.onload = function() {
    var rawPath = window.location.pathname;
    var pageId = md5(rawPath);  // 生成固定长度的哈希字符串
    
    var gitalk = new Gitalk({
      clientID: 'Ov23livLCw69zvvmm6ZD',
      clientSecret: '575ec7359cdcc9fa81ea3addd623f85f4c468737',
      repo: 'comments',
      owner: 'steakdream',
      admin: ['steakdream'],
      id: pageId,  // 使用处理后的 pageId
      distractionFreeMode: false,
      debug: true
    });
    gitalk.render('gitalk-container');
  }
</script>

<script src="https://giscus.app/client.js"
        data-repo="steakdream/steakdream.github.io"
        data-repo-id="R_kgDOODkdGg"
        data-category="General"
        data-category-id="DIC_kwDOODkdGs4Cog3q"
        data-mapping="pathname"
        data-strict="1"
        data-reactions-enabled="1"
        data-emit-metadata="0"
        data-input-position="bottom"
        data-theme="preferred_color_scheme"
        data-lang="en"
        crossorigin="anonymous"
        async>
</script>
