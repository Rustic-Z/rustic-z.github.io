---
layout: post
---

{% include head.html %}

<body>
    {% include header.html %}

    <div id="m-posts-content" class="container" style="margin:auto; width:50%;">
        <p style="font-size:30px;">Publications</p>
        {% for post in site.posts %}
            <h5>({{ post.date | date_to_string }}) &raquo; <a style="text-decoration:none;color:#8D2424;" href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></h5>
            <h6 style="color:#3E3E3E;font-style:italic;font-size:15px;">{{ post.tag }}</h6>
            <p style="color:#222222;font-size:12px;">{{ post.summary }}</p>
        {% endfor %}
    </div>
</body>