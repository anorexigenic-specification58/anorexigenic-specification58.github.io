---
layout: default
title: Residual Plots
category: Statistics

tags:
  - regression
  - diagnostics
  - statistics

related:
  - Q-Q Plots
  - Regression
  - Heteroscedasticity

status: evergreen
---

<div class="container">

    <div class="page-header">

        <a class="back-link" href="/notes/">
            ← Notes
        </a>

        <h1>{{ page.title }}</h1>

    </div>


    <section>

        <p>
            A residual is the difference between an observed value
            and the value predicted by a model.
        </p>


        <h2>What is a residual?</h2>

        <p>
            For an observation with actual value
            <em>y</em> and predicted value
            <em>ŷ</em>, the residual is:
        </p>

        <p>
            <strong>e = y − ŷ</strong>
        </p>


        <h2>Why plot residuals?</h2>

        <p>
            Residual plots help us determine whether the assumptions
            behind a model are reasonable and whether the model is
            systematically missing structure in the data.
        </p>


        <h2>What I look for</h2>

        <ul>
            <li>Non-linearity</li>
            <li>Heteroscedasticity</li>
            <li>Outliers</li>
            <li>Clusters or unexplained structure</li>
            <li>Patterns over time</li>
        </ul>


        <h2>My understanding</h2>

        <p>
            A useful way to think about a residual plot is that it
            shows us what the model failed to explain.
        </p>

    </section>

</div>
