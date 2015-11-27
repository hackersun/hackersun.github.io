---
layout: home
---
<div id="homepage">
    <div class="index-content project">
        <div class="section">
            <ul class="artical-cate">
                <li><a href="/"><span>Blog</span></a></li>
                <li class="on" style="text-align:center"><a href="/project"><span>Project</span></a></li>
                <li style="text-align:right"><a href="/about"><span>About</span></a></li>
            </ul>

            <div class="cate-bar"><span id="cateBar"></span></div>

            <ul class="artical-list">
            {% for post in site.categories.project %}
                <li>
                    <h2>
                        <a href="{{ post.url }}">{{ post.title }}</a>
                    </h2>
                    <div class="title-desc">{{ post.description }}</div>
                </li>
            {% endfor %}
            </ul>
        </div>
        <!--<div class="aside"></div>-->
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
