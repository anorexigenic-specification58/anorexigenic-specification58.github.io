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


        {% assign categories = site.notes
            | map: "category"
            | uniq
            | sort %}


        {% for category in categories %}

            <div class="note-category-section">

                <div class="section-label">
                    {{ category }}
                </div>


                <div class="list">

                    {% assign category_notes = site.notes
                        | where: "category", category
                        | sort: "title" %}


                    {% for note in category_notes %}

                        <div class="list-item">

                            <h3>

                                <a href="{{ note.url | relative_url }}">
                                    {{ note.title }}
                                </a>

                            </h3>


                            {% if note.tags %}

                                <p>

                                    {% for tag in note.tags %}

                                        {{ tag }}{% unless forloop.last %}
                                        ·
                                        {% endunless %}

                                    {% endfor %}

                                </p>

                            {% endif %}

                        </div>

                    {% endfor %}

                </div>

            </div>

        {% endfor %}

    </section>

</div>
