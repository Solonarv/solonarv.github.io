
{% for post in site.posts %}
  {% if post.categories contains page.cat }%
    - [[{{ post.date | date_to_string }}] {{ post.title }}]({{ site.baseurl }}/{{ post.permalink }})
  {% endif %}
{% endfor %}