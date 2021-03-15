---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

All models are wrong, but some are useful.

The thinking models that have been included here are based on our experience with teaching
and coaching new ways of working with [Okaloa Flowlab](https://www.okaloa.com) simulations.
We hope that the models collected here are useful to think about how work works,
and how to introduce new ways of working in organizations.

<h1>Models</h1>
{% for category in site.categories %}
<ul>
    {% assign posts = category[1] | sort: "title" %}
    {% for post in posts %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
{% endfor %}
