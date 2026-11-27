---
layout: default
permalink: /projects
title: Projects
---

<article class="page projects-intro">
  <h1 class="page-title">{{ page.title }}</h1>

<p>In my spare time, I enjoy building things. Most of these projects grew out of my work in election administration: tools I wished existed, so I made them. Each one lives on its own corner of raviudeshi.com.</p>

<nav class="project-jump" aria-label="Jump to a project">
  <span class="project-jump-label">Jump to</span>
  {% for p in site.data.projects %}<a href="#{{ p.id }}"><img src="{{ site.baseurl }}{{ p.logo }}" alt="" width="18" height="18">{{ p.name }}</a>{% endfor %}
</nav>
</article>

{% for p in site.data.projects %}
<article class="page project-entry" id="{{ p.id }}">
  <div class="project-entry-header">
    <img class="project-entry-logo" src="{{ site.baseurl }}{{ p.logo }}" alt="" width="56" height="56">
    <div>
      <h2 class="project-entry-title">{{ p.full_name | default: p.name }}</h2>
      {% if p.coming_soon %}<span class="project-badge">Coming soon</span>{% else %}<a class="project-entry-url" href="{{ p.url }}">{{ p.url | remove: "https://" }}</a>{% endif %}
    </div>
  </div>

  {% if p.screenshot %}
  <a class="project-entry-shot" href="{{ p.url }}"><img src="{{ site.baseurl }}{{ p.screenshot }}" alt="Screenshot of {{ p.full_name | default: p.name }}" loading="lazy"></a>
  {% endif %}

  {% case p.id %}
  {% when 'voteflow' %}
  <p>VoteFlow tracks early voting and mail ballot turnout day by day, locality by locality, and compares it with past elections. It started in Virginia, where voters get 45 days of early voting and the state publishes daily files for every locality, and now covers every county in California too.</p>
  <p>When I worked in a local Virginia elections office, I kept detailed spreadsheets of these numbers to see how early voting was unfolding and how busy the days ahead would be. VoteFlow is the modern version of those spreadsheets. It updates automatically throughout the day, and for places like Fairfax County it goes all the way down to individual early voting sites.</p>
  {% when 'recountwatch' %}
  <p>In Santa Clara County, where I now work, local contests decided by fewer than 25 votes or less than 0.25% of ballots cast get an automatic hand recount. Recount Watch follows every local contest as results are updated after Election Day and flags the ones that are in recount range, getting closer, or somewhat close.</p>
  <p>Each contest shows how its margin has moved with every results update, so you can see whether a race is tightening or pulling apart.</p>
  {% when 'stickers' %}
  <p>The I Voted Sticker Database collects "I Voted" sticker designs from across the country: more than 2,500 designs so far, from all 50 states. You can browse them by theme, state, or design contest, find designs on a map, and even turn your favorites into a phone or desktop wallpaper.</p>
  <p>I love seeing all the unique stickers that come out of the design contests counties hold, and the site tells the stories behind many of the winners. Know of a sticker that's missing? You can submit it.</p>
  {% when 'oscars' %}
  <p>Every year I try to watch every movie nominated in every category at the Oscars, a challenge known as the Oscars Death Race. For years I tracked it here with my <a href="{{ site.baseurl }}/archives">Oscars checklists</a>. Oscars Watch turns those checklists into a live site.</p>
  <p>It lists every film with a real shot at a nomination, using Gold Derby's combined odds, and shows where to watch each one in the US, whether in theaters or streaming. You can mark the films you've seen to track your own progress, and follow the odds as they move toward nominations in January.</p>
  {% endcase %}

  {% unless p.coming_soon %}<p><a class="project-entry-visit" href="{{ p.url }}">Visit {{ p.name }}&nbsp;&rarr;</a></p>{% endunless %}
</article>
{% endfor %}
