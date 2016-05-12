<div class='about-links'>
  <h4>Pack 4496</h4>
  <ul>
    {% for page in site.pages %}
    {% if page.categories contains "about" %}
    <li><a href="{{ page.url }}">{{ page.title }}</a></li>
    {% endif %}
    {% endfor %}
  </ul>
</div>