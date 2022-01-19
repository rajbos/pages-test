### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}



<a
        class="tag"
        href="/tag/{{ tag }}"
        title="{{ site.data.tagDescriptions[tag] }}">
        {{ tag }}
    </a>


