<div class='learn-more-links'>
  <h4>More About Cub Scouting</h4>

  <ul>
    {% for page in site.pages %}
    {% if page.categories contains "learn" %}
    <li><a href="{{ page.url }}">{{ page.title }}</a></li>
    {% endif %}
    {% endfor %}

    {% for link in site.data.learn-more-links %}
      <li><a href="{{ link.url }}" target='_blank'>{{ link.title }} <i class='fa fa-external-link'></i></a></li>
    {% endfor %}
  </ul>
</div>