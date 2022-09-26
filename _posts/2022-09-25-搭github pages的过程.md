---
layout: post
title:  "搭github pages & jekyll"
date:   2022-09-25 16:05:28 +0800
categories: pages
---
{% include toc %}
 之前在开源中国注册写博客的时候它的页面还是很干净的， 最近广告越来越多而且那搜索做的真的一言难尽
<figure style="width: 600px" class="align-center">
  <img src="{{ '/images/post_pictures/oschina上闪烁的代码托管.png' | absolute_url }}" alt="">
  <figcaption>笑了, 一直在闪烁引起你注意.</figcaption>
</figure> 
  
  试试搭个github pages, 跟着学一下下页面.

# 第一步. 跟着官网教程建仓库
[github pages官网链接](https://pages.github.com/ "github pages官网链接")<br />
需要个GitHub的账号, 在Github上建一个跟账号名一样的仓库, 格式是 username.github.io， 创建好了以后直接可以访问
如果是404就已经成功创建好了，如果是Site not found就检查一下账号名是不是对应上这个url

<figure style="width: 600px" class="align-center">
  <img src="/images/post_pictures/404SiteNotFound.png" alt="">
  <figcaption>看看是site not found还是page not found.</figcaption>
</figure> 

还需要懂一点点git知识, 在本地用git把新建的仓库拉下来, 接着添加一下官方推荐的Jekyll作为静态站点生成器

# 第二步. 生成Jekyll静态站点
[jekyll官网链接](https://jekyllrb.com/)
需要Ruby Gem的环境, 而且在Windows上很不好弄, 直接用Ubuntu生成好网站再上传到仓库就好了
因为只是生成了一些静态页面, 而且是基于配置的, 基本上照规则配置好生成一次拉回本地就好了, 每次上传到仓库的时候github会自动帮你部署的

![](/images/post_pictures/跟着命令在ubuntu上装RubyGem.png "跟着命令部署就好")
生成好后是这样子的，着重注意_config.yml就好
![](/images/post_pictures/生成后的jekyll.png "生成后的jekyll")

此时如果你把这些全部push到远程仓库, 那再访问页面就会有好东西了
