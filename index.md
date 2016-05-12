---
layout: default
---

<img src='/images/photos/camp-edwards-polar-swim.jpg' width='100%' />


<div class="page-content">
  <div class="wrapper">
    <div class="home">
      {% for post in site.posts %}
        {% if post.pin == true %}
          <article>

            <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
              <!-- <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a> -->
            {{ post.excerpt }}
            <!-- <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span> -->
          <a class='link-button' href="{{ post.url }}">Read More</i></a>
          </article>
        
        {% endif %}

      {% endfor %}
    <!--   <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p> -->

      

    </div>

    <a href='/posts/'>All Posts</a>

    
  </div>
</div>




{% include events.html %}
