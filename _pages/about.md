---
layout: page
title: Home
permalink: /
---
<style>
  body:has(.fronthome-layout) h1 {
    display: none;
  }
</style>


<style>
  .fronthome-layout {
    display: grid;
    grid-template-columns: 1fr;
    gap: 1.5rem;
    align-items: start;
  }

  @media (min-width: 768px) {
    .fronthome-layout {
      grid-template-columns: minmax(0, 6fr) minmax(0, 6fr);
    }
  }
</style>

15+ years turning messy, high-stakes data into models and tools to improve user decision-making.



<div class="fronthome-layout">
  <div>
    {% include figure.liquid loading="eager" path="assets/img/Schneider-Headshot.jpg" title="Max Schneider" class="img-fluid rounded z-depth-1" %}
  </div>

  <div markdown="1">
<span style="font-size: 2em;"> I’m Max, a statistician, science & risk communicator and earthquake scientist based in San Francisco. </span>

Update: After completing my post-doc at the US Geological Survey, I am seeking a new role applying my data science and product skillsets to tough problems in industry and science. I am also open to consulting work - please see my [consulting page](https://maxdschneider.github.io/consulting/) and [get in touch](https://maxdschneider.github.io/contact/). 
  </div>

</div>
<br>


<div markdown="1">
<span style="font-size: 3em;">News</span> 
</div>
{% include news.liquid %}

<style>
  .social i {
    font-size: 1.4em;
  }
</style>

<div class="social">
  <a href="mailto:{{ site.data.socials.email }}" aria-label="Email">
    <i class="fa-solid fa-envelope"></i>
  </a>
  <a href="https://www.linkedin.com/in/{{ site.data.socials.linkedin_username }}/" target="_blank" rel="noopener" aria-label="LinkedIn">
    <i class="fa-brands fa-linkedin"></i>
  </a>
  <a href="https://scholar.google.com/citations?user={{ site.data.socials.scholar_userid }}" target="_blank" rel="noopener" aria-label="Google Scholar">
    <i class="ai ai-google-scholar"></i>
  </a>
  <a href="{{ site.data.socials.cv_pdf | relative_url }}" aria-label="CV">
    <i class="fa-solid fa-file-pdf"></i>
  </a>
</div>

