---
layout: home
---

<div id="homepage">
    <div class="index-content categories">
        <div class="section">
            <ul class="artical-cate">
                <li ><a href="/"><span>首页</span></a></li>
                <li class="on"><a href="/categories"><span>分类目录</span></a></li>
                <li ><a href="/archives"><span>文章归档</span></a></li>
                <li ><a href="/about-me"><span>联系我</span></a></li>
            </ul>

            <div class="cate-bar"><span id="cateBar"></span></div>

            <ul class="artical-list">
            {% for post in site.categories.category %}
                <li>
                    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
                    <div class="title-desc">{{ post.description }}</div>
                </li>
            {% endfor %}
            </ul>
        </div>
    </div>
    <div class="sidenav">
        <dd class="avatar-container clearfix">
            <div class="avator-image left" style="width:70px; height:70px;">
                <div class="avator">
                    <img src="../images/favicon.ico" height="60px" width="60px"/>
                </div>
            </div>
            <div class="avator-title">
                <h2>hackersun</h2>
                <a href="http://hackersun.github.io/about-me/"><b>About Me</b></a> 
            </div>
        </dd>
    </div>
</div>
