---
layout: about
title: about
permalink: /
subtitle: PhD Candidate @University of Stuttgart

profile:
  align: right
  image: me.JPEG
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>🥐 I do like croissants!</p>

selected_papers: true # includes a list of papers marked as "selected={true}"
social: false # big social icons at the bottom disabled; minimal inline links are rendered after the bio instead

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: # blank = render all items in `_news` (needed for the scroll box to have anything to scroll)

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

<link rel="stylesheet" href="{{ '/assets/css/pub-badges.css' | relative_url }}">

<style>
  /* shrink the profile picture column (theme default: 30%) */
  @media (min-width: 576px) {
    .profile {
      width: 22%;
    }
  }

  /* news box: the theme caps it at an inline max-height of 60vw, which is taller
     than the whole list on desktop, so it never actually scrolls */
  .news .table-responsive {
    max-height: 20rem !important;
    overflow-y: auto;
  }
</style>

I am a PhD candidate at the [University of Stuttgart](https://www.ias.uni-stuttgart.de/) with a background in electrical engineering. I am interested in building autonomous systems based on machine learning and deep learning. Currently, my research focuses on generative AI and how it can be leveraged for variability-intensive software systems, exploring the exciting semantic capabilities of these models.
As part of this research, I recently spent time as a visiting researcher at [Inria](https://www.inria.fr/en) in Lille France.

Away from the keyboard (the computer one), I make music, some of it might end up on [SoundCloud](https://soundcloud.com/keller4ssel).

<!-- Beyond my research, I work with [PEPLY.ai](https://www.peply.ai/), where I build their app and develop new full-stack features for the platform.

<!-- Minimal inline social links, driven by _data/socials.yml (add a `when` branch below for any new key you use there). -->
<div class="contact-links" style="display: flex; flex-wrap: wrap; column-gap: 1.5rem; row-gap: 0.35rem; margin-top: 1rem;">
  {%- for social in site.data.socials -%}
    {%- assign key = social[0] -%}
    {%- assign value = social[1] -%}
    {%- case key -%}
      {%- when 'github_username' -%}
        <a href="https://github.com/{{ value }}" title="GitHub"><i class="fa-brands fa-github"></i> github</a>
      {%- when 'scholar_userid' -%}
        <a href="https://scholar.google.com/citations?user={{ value }}" title="Google Scholar"><i class="ai ai-google-scholar"></i> scholar</a>
      {%- when 'orcid_id' -%}
        <a href="https://orcid.org/{{ value }}" title="ORCID"><i class="ai ai-orcid"></i> orcid</a>
      {%- when 'linkedin_username' -%}
        <a href="https://www.linkedin.com/in/{{ value }}" title="LinkedIn"><i class="fa-brands fa-linkedin"></i> linkedin</a>
      {%- when 'email' -%}
        <a href="mailto:{{ value }}" title="Email"><i class="fa-solid fa-envelope"></i> email</a>
      {%- when 'cv_pdf' -%}
        <a href="{{ value | relative_url }}" title="CV"><i class="ai ai-cv"></i> cv</a>
      {%- when 'inspirehep_id' -%}
        <a href="https://inspirehep.net/authors/{{ value }}" title="Inspire HEP"><i class="ai ai-inspire"></i> inspirehep</a>
      {%- when 'stackoverflow_id' -%}
        <a href="https://stackoverflow.com/users/{{ value }}" title="Stack Overflow"><i class="fa-brands fa-stack-overflow"></i> stackoverflow</a>
      {%- when 'kaggle_id' -%}
        <a href="https://www.kaggle.com/{{ value }}" title="Kaggle"><i class="fa-brands fa-kaggle"></i> kaggle</a>
      {%- when 'x_username' -%}
        <a href="https://twitter.com/{{ value }}" title="X"><i class="fa-brands fa-x-twitter"></i> x</a>
      {%- when 'rss_icon' -%}
        <a href="{{ '/feed.xml' | relative_url }}" title="RSS"><i class="fa-solid fa-square-rss"></i> rss</a>
      {%- else -%}
        {%- if value.url and value.title -%}
          <a href="{{ value.url }}" title="{{ value.title }}"><i class="{{ value.logo | default: 'fa-solid fa-link' }}"></i> {{ value.title | downcase }}</a>
        {%- endif -%}
    {%- endcase -%}
  {%- endfor -%}
</div>
