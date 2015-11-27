---
layout: home
---
<div class"homepage">
    <div class="content blog">
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
