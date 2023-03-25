---
layout: default
---

# 花影的博客

你好，我是花影，一名正在学习的网络空间安全研究生。

这里是我的博客：[blog](https://rongxiye.github.io/)

我会把我做过的ctf题目的wp以及一些文章放在博客上。它还处于一个未完工的状态，我会一致慢慢完善它的。



## CTF writeup

### reverse

#### buuoj

[刮开有奖](./2023/03/25/刮开有奖.md)





## iOS安全研究

bmalloc源码解读

libmalloc-nanozonev2结构解读









## 其他







## All blogs

<ul>
    {% for post in paginator.posts %}
      <li>
          <h2><a href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">{{ post.title }}</a></h2>
          <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date_to_string }}</time>
          <p>{{ post.content | strip_html | truncatewords:50 }}</p>
      </li>
    {% endfor %}
</ul>
