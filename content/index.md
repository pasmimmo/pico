# Welcome

Hello guys, come state?

## Secondo titolo


<section class="articles">
    {% for page in pages(current_page.id) if not page.hidden %}
        <article>
            <h2><a href="{{ page.url }}">{{ page.title }}</a></h2>
            {{ page.id|content }}
        </article>
    {% endfor %}
</section>