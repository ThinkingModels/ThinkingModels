---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---
<h1>Models</h1>
{% for category in site.categories %}
<ul>
    {% assign posts = category[1] | sort: "title" %}
    {% for post in posts %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
{% endfor %}
