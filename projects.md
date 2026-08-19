---
layout: default
permalink: /projects/
title: Projects
description: "Each one follows the same shape: what was broken, what I did about it, and what the results were."
eyebrow: Projects
heading: "Two case studies, start to finish"
intro: "Each one follows the same shape: what was broken, what I did about it, and what the results were."
shelf_note: "Also on the shelf: a topic-based help page hand-coded in DITA, a group proposal recommending a change to a UNT campus space, a rewritten home page for a pest control company, a memo comparing Coca-Cola's content strategy in the US and Guatemala, and three interview-based articles for a school paper."
---
<main class="page-main page-main--wide">
  <div class="container">
    <p class="eyebrow">{{ page.eyebrow }}</p>
    <h1 class="page-title">{{ page.heading }}</h1>
    <p class="page-intro">{{ page.intro }}</p>
  </div>

  {% include case-studies.html %}

  {% include more-work.html %}
</main>
