---
layout: default
title: Books
permalink: /books/
---

<div class="container">

    <div class="page-header">

        <a class="back-link" href="/">
            ← Thinking Better
        </a>

        <h1>Books</h1>

    </div>


    <section>

        <p class="section-intro">
            Books that have influenced how I think, build and
            understand the world.
        </p>


        <div class="list">

            {% assign books = site.books | sort: "title" %}

            {% for book in books %}

                <div class="list-item">

                    <h3>
                        <a href="{{ book.url | relative_url }}">
                            {{ book.title }}
                        </a>
                    </h3>

                    {% if book.author %}
                        <p>
                            {{ book.author }}
                        </p>
                    {% endif %}

                    {% if book.status %}
                        <p>
                            <strong>Status:</strong>
                            {{ book.status }}
                        </p>
                    {% endif %}

                </div>

            {% endfor %}

        </div>

    </section>

</div>
