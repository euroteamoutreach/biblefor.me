---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

##### Thank you for reading the tract you received! We'd like to offer you one of the books below for free. Just choose the book you want and complete the [request form](/request).

{% assign sorted_pages = site.pages | sort:"position" %}
{% for page in sorted_pages %}
{% if page.categories contains 'give-away-books' %}
<div class="book-option {{ page.scheme }}" style="background-image: url('{{ page.background }}'); background-color: {{ page.color }}">
    <div class="book-option-inner">
    <a href="{{ page.url }}">
    <img class="" src="/{{ page.thumbnail }}"/>
    <h3 class="heading">{{ page.title }}</h3>
    <p>{{ page.short_description | truncate: 230 }}</p>
    <div class="">
        {% if page.one_sentence %}
        <p>{{ page.one_sentence }}</p>&nbsp;&nbsp;
        {% endif %}
    </div>
    </a>
    <a class="button" href="{{ page.url }}">Request</a>
    </div>
</div>
{% endif %}
{% endfor %}

<div class="clearfix"></div>

##### Got questions? [Use the contact form to get in touch with us](/contact)

