---
layout: default
---

<div class="home">
  <h2>
  	Welcome to ShugeAsks! 
  </h2>
  <h3>
  Here's some general information about our podcast. More information to get you hyped. We're targeting to release in Summer of 2018 on YouTube, iTunes, and wherever quality podcasts are hosted. This site is currently under construction, so please stay tuned!
  </h3>
{% for post in site.posts %}
    <h3>
      <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title | escape }}</a>
	</h3>
      <time> {{ post.date | date_to_string }}</time>
    
    {{ post.excerpt }}
{% endfor %}

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | relative_url }}">via RSS</a></p>

</div>
