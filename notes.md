---
layout: default
title: Notes
permalink: /notes/
---

<div class="container">

    <div class="page-header">

        <a class="back-link" href="/">
            ← Thinking Better
        </a>

        <h1>Notes</h1>

    </div>


    <section>

        <p class="section-intro">
            An evolving collection of things I'm learning,
            understanding and trying to make sense of.
        </p>


        <div class="list">

            {% assign notes = site.notes | sort: "title" %}

            {% for note in notes %}

                <div class="list-item">

                    <h3>
                        <a href="{{ note.url | relative_url }}">
                            {{ note.title }}
                        </a>
                    </h3>

                    {% if note.category %}
                        <p>
                            {{ note.category }}
                        </p>
                    {% endif %}

                </div>

            {% endfor %}

        </div>

    </section>

</div>
