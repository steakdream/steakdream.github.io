---
title: "Home Page"
layout: splash
permalink: /
date: 2016-03-23T11:48:41-04:00
header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/images/IMG_3846.JPG
  actions:
    - label: "There is a link"
      url: "https://github.com/mmistakes/minimal-mistakes/"
  caption: "Photo credit: [**Unsplash**](https://unsplash.com)"
excerpt: "Bacon ipsum dolor sit amet salami ham hock ham, hamburger corned beef short ribs kielbasa biltong t-bone drumstick tri-tip tail sirloin pork chop."
intro: 
  - excerpt: 'Nullam suscipit et nam, tellus velit pellentesque at malesuada, enim eaque. Quis nulla, netus tempor in diam gravida tincidunt, *proin faucibus* voluptate felis id sollicitudin. Centered with `type="center"`'
---
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>{{ page.title }} - Site Title</title>
    <meta name="description" content="{{ page.excerpt }}">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <!-- Gitalk CSS -->
    <link rel="stylesheet" href="https://unpkg.com/gitalk/dist/gitalk.css">
  </head>
  <body>
    <!-- 页面其他内容 -->
    <header>
      <h1>{{ page.title }}</h1>
      <p>{{ page.excerpt }}</p>
    </header>

    <!-- 在需要显示评论的位置放置容器 -->
    <div id="gitalk-container"></div>

    <!-- Gitalk JS -->
    <script src="https://unpkg.com/gitalk/dist/gitalk.min.js"></script>
    <script type="text/javascript">
      // 等待页面所有资源加载完成后再初始化 Gitalk
      window.onload = function() {
        var gitalk = new Gitalk({
          clientID: 'Ov23livLCw69zvvmm6ZD',
          clientSecret: '575ec7359cdcc9fa81ea3addd623f85f4c468737',
          repo: 'comments',       // 存储评论的 GitHub 仓库
          owner: 'steakdream',
          admin: ['steakdream'],  // 管理员（评论 Issue 的所有者）
          id: window.location.pathname,  // 用当前页面路径作为唯一标识
          distractionFreeMode: false     // 是否启用无干扰模式
        });
        gitalk.render('gitalk-container');
      }
    </script>
  </body>
</html>
