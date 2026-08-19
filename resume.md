---
layout: default
permalink: /resume/
title: Resume
description: "Everything on this site, condensed. Grab the PDF, or email me if you'd rather just talk."
eyebrow: Resume
heading: "The short version"
intro: "Everything on this site, condensed. Grab the PDF, or email me if you'd rather just talk."
resume_pdf: Emilie-Rezendes-Resume.pdf
highlights:
  - "BA Technical Communication: Content Strategy, UNT — 4.0 GPA, graduating 2027"
  - "Content creator at Travel on Purpose · summer intern at Tirzah International"
  - "Content audits, stakeholder interviews, and analytics on a live site"
---
<main class="page-main">
  <p class="eyebrow">{{ page.eyebrow }}</p>
  <h1 class="page-title">{{ page.heading }}</h1>
  <p class="page-intro" style="max-width:52ch">{{ page.intro }}</p>

  <div class="resume-actions">
    <a class="btn btn--primary" href="{{ page.resume_pdf | relative_url }}" download>
      <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" aria-hidden="true"><path d="M12 3v12M7 11l5 5 5-5M4 21h16"></path></svg>
      Download PDF
    </a>
    <a class="btn btn--secondary" href="mailto:{{ site.email }}">Email me instead</a>
  </div>

  <ul class="resume-list">
    {% for point in page.highlights %}
    <li>
      <svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="#1E4B42" stroke-width="1.8" aria-hidden="true"><path d="M20 6L9 17l-5-5"></path></svg>
      <span>{{ point }}</span>
    </li>
    {% endfor %}
  </ul>
</main>
