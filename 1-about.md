---
layout: page
permalink: /about
title: About Ravi Udeshi
description: "Ravi Udeshi is an election administrator in Santa Clara County, California, an Oscars Death Racer, and a longtime tinkerer who builds web projects about elections and movies."
redirect_from:
  - /contact
  - /contact/
  - /subscribe
  - /subscribe/
social:
  - name: LinkedIn
    url: https://www.linkedin.com/in/rkudeshi
    icon: linkedin
  - name: X (Twitter)
    url: https://x.com/rkudeshi
    icon: x
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

<p class="about-lede">Hi, I’m Ravi Udeshi. I’m an election administrator who loves technology, movies, and building things.</p>

### Follow or contact me {#follow}

<nav class="social-links" aria-label="Follow me">
  {% for s in page.social %}<a href="{{ s.url }}" rel="me"><img src="{{ site.baseurl }}/public/social/{{ s.icon }}.svg" alt="" width="18" height="18">{{ s.name }}</a>{% endfor %}
</nav>

I’m **@rkudeshi** on all of them, and you’re welcome to message me there.

Have an idea or a suggestion? Spot a typo, a broken link, or an issue on this site or one of [my projects](/projects)? I’d like to hear about it. You can also email me:

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

### About me {#about-me}

I’m an election administrator, and I’ve worked in two of the largest election jurisdictions in America: Santa Clara County, California, home to nearly 2 million people, and Fairfax County, Virginia, home to more than 1.1 million. For the full rundown, see my [LinkedIn](https://www.linkedin.com/in/rkudeshi).

<ol class="timeline">
  <li>
    <span class="timeline-dates">2026 – present</span>
    <strong class="timeline-office">Santa Clara County Registrar of Voters’ Office</strong>
    <span class="timeline-title">Assistant Registrar of Voters</span>
    <p>I’m part of the three-person executive team that runs elections for more than a million voters, with 112 vote centers and materials in 17 languages. I also started the county’s first “I Voted” sticker design contest.</p>
  </li>
  <li>
    <span class="timeline-dates">2017 – 2025</span>
    <strong class="timeline-office">Fairfax County Office of Elections</strong>
    <span class="timeline-title">Deputy Director and Deputy General Registrar</span>
    <p>I helped run elections in Virginia’s largest county, with 6,000 poll workers each election. I led the county’s $9 million replacement of its voting equipment, and built in-house tools that replaced vendor software.</p>
  </li>
</ol>

Projects from these two offices have won 17 national awards from the U.S. Election Assistance Commission and the Election Center, and I led or worked on nearly all of the Fairfax ones, from poll worker training to tools for running Election Day. I’m proud of that work.

Elections shape a lot of what I build in my spare time, like an [early voting tracker](/projects#voteflow), a [recount watch](/projects#recountwatch), and a [database of “I Voted” stickers](/projects#stickers).

The other big thing in my life is movies. I’m an Oscars Death Racer: every year I try to watch every film nominated in every category before the ceremony. I used to track that here with [Oscars checklists](/blog), and now I track it with [Oscars Watch](/projects#oscars).

I’m also a bit of a minimalist. For a while I tried [living with 75 things](/11/02/75-things).

### About this site {#about-the-site}

I started this site in 2005, when WordPress wasn’t even two years old. I ran it on WordPress for years before moving it to [Jekyll](https://jekyllrb.com), which turns plain text files into a fast, simple website. For most of that time, I wrote the site’s code by hand. It’s hosted on [GitHub Pages](https://pages.github.com), and the [source code](https://github.com/rkudeshi/rkudeshi.github.io) is public.

I write posts in [Markdown](https://commonmark.org). I usually jot down ideas in [nvALT](https://brettterpstra.com/projects/nvalt/) and flesh them out in [Sublime Text](https://www.sublimetext.com). These days I also build a lot of side projects with the help of AI coding tools, which has made it possible to finally build the tools I’ve wanted for years.

This version of the site was built on {{ site.time | date: "%B %-d, %Y" }} (revision <span title="{{ site.time | date: '%c' }}">{{ site.time | date: "%a" | truncate:1,'' | upcase }}{{ site.time | date: "%I%M" }}</span>). I use [Cloudflare Web Analytics](https://www.cloudflare.com/web-analytics/) to count visits. It doesn’t use cookies or follow you around the web.
