---
layout: home
---
<div class"homepage">
    <div class="index-content blog">
        <div class="section">
            <ul class="artical-cate">
                <li class="on"><a href="/"><span>Blog</span></a></li>
                <li style="text-align:center"><a href="/project"><span>Project</span></a></li>
                <li style="text-align:right"><a href="/about"><span>About</span></a></li>
            </ul>

            <div class="cate-bar"><span id="cateBar"></span></div>

            <ul class="artical-list">
            {% for post in site.categories.blog %}
                <li>
                    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
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
        <div class="touch-me">
            <a href="https://www.linkedin.com/in/sunguoli" target="_blank"><img src="https://static.licdn.com/scds/common/u/images/logos/favicons/v1/favicon.ico" alt="" width="25"/></a>
            <a href="http://blog.csdn.net/doc_sgl" target="_blank"><img src="http://blog.csdn.net/favicon.ico" alt="" width="25"/></a>
            <a href="https://github.com/hackersun" target="_blank"><img src="https://github.com/favicon.ico" alt="" width="25"/></a>
        </div>
        <p>^_^</p>
    </div>
    <div class="sidenav">
        <h2>Blog</h2>
        <ul class="artical-list">
        {% for post in site.categories.blog%}
            <li><a href="{{ post.url }}">{{ post.title }}</a></li>
        {% endfor %}
        </ul>

        <h2>Project</h2>
        <ul class="artical-list">
        {% for post in site.categories.project%}
            <li><a href="{{ post.url }}">{{ post.title }}</a></li>
        {% endfor %}
        </ul>
    </div>
</div>
