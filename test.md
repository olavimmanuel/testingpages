---
layout: default
---


**I am markdown**

<div markdown="1">
    Hey **markdown** is working! :D
</div>

<div>
    **markdown** works even *without* the markdown tag in the div! ;)
</div>


{% include mymarkdown.md %}

<div class="posts">
  {% for post in site.posts %}
    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>

      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>
