---
layout: page
permalink: /about
title: About Ravi Udeshi
description: "Ravi Udeshi is an election administrator who likes technology, movies, travel, and building things. Follow or contact him, and learn about this site."
redirect_from:
  - /contact
  - /contact/
  - /subscribe
  - /subscribe/
social:
  - name: X (Twitter)
    url: https://x.com/rkudeshi
    icon: x
  - name: LinkedIn
    url: https://www.linkedin.com/in/rkudeshi
    icon: linkedin
  - name: Threads
    url: https://www.threads.com/@rkudeshi
    icon: threads
  - name: Bluesky
    url: https://bsky.app/profile/rkudeshi.bsky.social
    icon: bluesky
  - name: Instagram
    url: https://www.instagram.com/rkudeshi
    icon: instagram
---

<h2 class="about-section" id="follow">Follow or contact me</h2>

<nav class="link-list" aria-label="Follow me">
  <span class="link-list-label">Find me on</span>
  {% for s in page.social %}<a href="{{ s.url }}" rel="me"><img src="{{ site.baseurl }}/public/social/{{ s.icon }}.svg" alt="" width="18" height="18">{{ s.name }}</a>{% endfor %}
</nav>

I'm **@rkudeshi** everywhere above, and you're welcome to message me on any of them.

Have an idea or a suggestion? Spot a typo, a broken link, or a number that looks off on this site or one of [my projects](/projects)? I'd like to hear about it. You can also email me:

<p class="email-reveal">
  <button type="button" id="email-reveal">Show my email address</button>
  <noscript><img src="{{ site.baseurl }}/silo/images/contact-mail.png" alt="My email address, shown as an image"></noscript>
</p>

<script>
  // The address is put together in your browser, so it never appears in this page's source.
  (function () {
    var btn = document.getElementById('email-reveal');
    btn.addEventListener('click', function () {
      var addr = ['contact', ['raviudeshi', 'com'].join('.')].join('@');
      var link = document.createElement('a');
      link.href = 'mail' + 'to:' + addr;
      link.textContent = addr;
      btn.parentNode.replaceChild(link, btn);
      link.focus();
    });
  })();
</script>

<h2 class="about-section" id="about-me">About me</h2>

I'm an election administrator who likes technology, movies, travel, and building things. I've worked in two of the largest election offices in the country:

<ol class="timeline">
  <li>
    <span class="timeline-dates">2026 – present</span>
    <strong class="timeline-title">Assistant Registrar of Voters</strong>
    <span class="timeline-org">Santa Clara County, California</span>
    <p>I’m part of the three-person executive team that runs elections for nearly a million voters, with 112 vote centers, about a million mail ballots each election, and materials in 17 languages. I also started the county’s first “I Voted” sticker design contest.</p>
  </li>
  <li>
    <span class="timeline-dates">2017 – 2025</span>
    <strong class="timeline-title">Deputy Director and Deputy General Registrar</strong>
    <span class="timeline-org">Fairfax County, Virginia</span>
    <p>I helped run elections in Virginia’s largest county, with 6,000 poll workers each election. I led the recount of a November 2024 election with 350,000 ballots, and built in-house tools that replaced vendor software.</p>
  </li>
</ol>

I'm proud to have led or been part of teams whose projects have won 14 national awards from the U.S. Election Assistance Commission and the Election Center, for work like poll worker training, voter guides, and tools for running Election Day.

Outside of work, I like experimenting with technology and AI to build the tools I wish existed, and that's most of what you'll find here: an [early voting tracker](/projects#voteflow), a [recount watch](/projects#recountwatch), a [database of "I Voted" stickers](/projects#stickers), and a way to keep up with [every Oscar-nominated film](/projects#oscars).

I've had this site since 2005. I don't blog much these days, but [the old posts](/blog) are still here.

<h2 class="about-section" id="about-the-site">About this site</h2>

I write posts in [Markdown](https://commonmark.org), a simple plain-text format. I usually jot down ideas in [nvALT](https://brettterpstra.com/projects/nvalt/) and flesh them out in [Sublime Text](https://www.sublimetext.com). These days I also build a lot of the site, and my projects, with the help of AI coding tools.

The site is built with [Jekyll](https://jekyllrb.com) and hosted on [GitHub Pages](https://pages.github.com). The [source code](https://github.com/rkudeshi/rkudeshi.github.io) is on GitHub. This version was built on {{ site.time | date: "%B %-d, %Y" }} (revision <span title="{{ site.time | date: '%c' }}">{{ site.time | date: "%a" | truncate:1,'' | upcase }}{{ site.time | date: "%I%M" }}</span>).

I use [Cloudflare Web Analytics](https://www.cloudflare.com/web-analytics/) to count visits. It doesn't use cookies or follow you around the web, and there are no ads here.
