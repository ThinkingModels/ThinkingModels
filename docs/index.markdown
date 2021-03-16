---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---
“Give me a firm place to stand on and I will move the earth” said Archimedes as he discovered the principle behind
levers that lift objects that are too heavy to lift. Archimedes’ insight is as valid as it ever was. For people, teams
and organizations to change their own ways of working often involves the type of heavy lifting that requires not just
levers but also solid foundations.

In a left-brain, analytic thinking, dominated world, the focus is on the lever provided by methods that codify new ways
of working based on past experience. As brain science teaches us, however, the left brain is a bad master; it provides
levers that are built on loose sand. Left unchecked, the left brain does not take context into account; it idealizes
solutions; and does not respond well when faced with its own limitations. Since the left brain has a hard time dealing
with change and novelty, this proves to be especially problematic for agile methods.

The agile mindset is better served by the right brain that recognizes the importance of context, looks at the whole (not
just the parts) and is better at dealing with novelty. While this kind of thinking provides a more solid foundation,
making the right brain a better master, this “whole” that “goes beyond the parts” is also notoriously hard to put into
words. The right brain is bad at verbalizing its thoughts. A mindset put into words seizes to be a mindset.

There is a need for a “whole-brain” way that covers the gap between left- and right-brain thinking. The models provided
here are an attempt to cover that gap. All of them are "Thinking models". They are useful not because they tell you what
to do, but, to the contrary, they help you to decide what to do for yourself. They are based on experience with teaching
and coaching new ways of working with [Okaloa Flowlab](https://www.okaloa.com) simulations.

<h1>Models</h1>
{% for category in site.categories %}
<ul>
    {% assign posts = category[1] | sort: "title" %}
    {% for post in posts %}
    <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
{% endfor %}
