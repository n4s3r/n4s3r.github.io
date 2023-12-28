<nav>
  <ul>
    <li><a href="/">Homepage</a></li>
  </ul>
 <ul>
  {% assign built_dirs = '' %}
  {% assign sorted_pages = site.pages | sort: 'path' %}
  {% for page in sorted_pages %}
  {% assign parts = page.path | split: '/' %}
    {% if parts[0] == "mainfolder" %}
      {% if parts.size == 2 %}
        <li>
          <a href="{{ page.url }}">{{ page.title }}</a>
        </li>
	<br>
      {% else %}
	{% for ident in (4..parts.size) %}
	  <ul>
	{% endfor %}
	{% assign temp_parts = parts | reverse | slice: 1, parts.size %}
	<ul>
	{% unless built_dirs contains temp_parts %}
	  <h3>{{ parts[-2] }}</h3>
	  {% assign built_dirs = built_dirs | append: temp_parts %}
          {% assign built_dirs = built_dirs | append: ' ' %}
	{% endunless %}
	<ul>
	<ul>
	  <li>
            <a href="{{ page.url }}">{{ page.title }}</a>
          </li>
	</ul>
	</ul>
	</ul>
	{% for ident in (4..parts.size) %}
          </ul>    
        {% endfor %}
	<br>
      {% endif %} 
    {% endif %}
  {% endfor %}
  </ul>
</nav>
