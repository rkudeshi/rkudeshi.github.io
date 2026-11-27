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

<h2 class="about-section" id="about-me">About me</h2>

I’m an election administrator who loves technology, movies, and building things. I’ve worked in two of the largest election jurisdictions in America: Santa Clara County, California, home to about 2 million people, and Fairfax County, Virginia, home to about 1.2 million.

<nav class="social-links" aria-label="Follow me">
  <span class="social-links-label">Follow me</span>
  <div class="social-links-list">{% for s in page.social %}<a href="{{ s.url }}" rel="me"><img src="{{ site.baseurl }}/public/social/{{ s.icon }}.svg" alt="" width="18" height="18">{{ s.name }}</a>{% endfor %}</div>
</nav>

<ol class="timeline">
  <li>
    <span class="timeline-dates">2026 – present</span>
    <strong class="timeline-office">Santa Clara County Registrar of Voters’ Office</strong>
    <span class="timeline-title">Assistant Registrar of Voters</span>
    <p>I’m part of the three-person executive team that runs elections for more than a million voters, with ballots and materials in 17 languages. I also started the county’s first “I Voted” sticker design contest.</p>
  </li>
  <li>
    <span class="timeline-dates">2017 – 2025</span>
    <strong class="timeline-office">Fairfax County Office of Elections</strong>
    <span class="timeline-title">Deputy Director and Deputy General Registrar</span>
    <p>I helped run elections in Virginia’s largest county. I led the county’s $9 million replacement of its voting equipment, and built in-house tools that replaced vendor software.</p>
  </li>
</ol>

Projects from these two offices have won 17 national awards from the U.S. Election Assistance Commission and the Election Center, and I led or worked on nearly all of the Fairfax ones, from poll worker training to tools for running Election Day. I’m proud of that work. My [LinkedIn](https://www.linkedin.com/in/rkudeshi) has more.

Elections shape a lot of what I build in my spare time, these days often with the help of AI coding tools: an [early voting tracker](/projects#voteflow), a [recount watch](/projects#recountwatch), and a [database of “I Voted” stickers](/projects#stickers).

Another big thing in my life is movies. I’m an Oscars Death Racer, part of a community of film fans who try to watch every movie nominated in every category before the ceremony. I used to track my progress here with [Oscars checklists](/blog), and now I track it with [Oscars Watch](/projects#oscars).

I’m also a minimalist. I don’t own just [75 things](/11/02/75-things) anymore, but I don’t own many more than that. I still try to keep as few things as possible and focus on memories, not things.

<h2 class="about-section" id="contact">Contact me</h2>

Have an idea or a suggestion, or spot an issue somewhere on this site or one of my projects? I’d like to hear about it. Message me on any of the networks above, or email me:

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

<h2 class="about-section" id="about-the-site">About this site</h2>

I started this site in 2005, when WordPress wasn’t even two years old. I ran it on WordPress for years before moving it to [Jekyll](https://jekyllrb.com), which turns plain text files into a fast, simple website. For most of that time, I wrote the site’s code by hand. It’s hosted on [GitHub Pages](https://pages.github.com), and the [source code](https://github.com/rkudeshi/rkudeshi.github.io) is public.

I write posts in [Markdown](https://commonmark.org). I usually jot down ideas in [nvALT](https://brettterpstra.com/projects/nvalt/) and flesh them out in [Sublime Text](https://www.sublimetext.com).

I’m a bit of a privacy nut, and I don’t like being tracked around the web, so I try not to do it here. I use [Cloudflare Web Analytics](https://www.cloudflare.com/web-analytics/) only to see how many people visit. It doesn’t use cookies or follow you across sites. Even the share links under each post are plain, handwritten links, so Facebook and Twitter don’t hear about your visit unless you click one.

<p class="page-meta">Built {{ site.time | date: "%b %-d, %Y" }} · Rev <span title="{{ site.time | date: '%c' }}">{{ site.time | date: "%a" | truncate:1,'' | upcase }}{{ site.time | date: "%I%M" }}</span></p>
