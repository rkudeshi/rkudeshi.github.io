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
---

<h2 class="about-section" id="about-me">About me</h2>

<div class="about-intro">
  <span class="about-photo"><img src="{{ site.baseurl }}/public/ravi-udeshi.jpg" alt="Ravi Udeshi" width="120" height="120"></span>
  <div class="about-intro-text">
    <p>I’m an election administrator who loves technology, movies, and building things.</p>
    <nav class="social-links" aria-label="Follow me">
      <span class="social-links-label">Follow me</span>
      <div class="social-links-list">{% for s in site.data.social %}<a href="{{ s.url }}" rel="me"><img src="{{ site.baseurl }}/public/social/{{ s.icon }}.svg" alt="" width="18" height="18">{{ s.name }}</a>{% endfor %}</div>
    </nav>
  </div>
</div>

I’ve helped lead two of the largest election jurisdictions in America, and I’m proud to have led or been part of teams that have won 17 national awards. My [LinkedIn](https://www.linkedin.com/in/rkudeshi) has more.

<ol class="timeline">
  <li>
    <span class="timeline-dates">2026 – present</span>
    <strong class="timeline-office">Santa Clara County, CA, Registrar of Voters’ Office</strong>
    <span class="timeline-title">Assistant Registrar of Voters</span>
    <p>Santa Clara County is the home of Silicon Valley and the largest county in the Bay Area, with about 2 million residents. I’m part of the executive team that runs its elections, with ballots and materials in 17 languages. I also started the county’s first “I Voted” sticker design contest.</p>
  </li>
  <li>
    <span class="timeline-dates">2017 – 2025</span>
    <strong class="timeline-office">Fairfax County, VA, Office of Elections</strong>
    <span class="timeline-title">Deputy Director and Deputy General Registrar</span>
    <p>Just outside Washington, D.C., Fairfax County is Virginia’s largest county, with about 1.2 million residents. I started as a poll worker, then joined the office full-time and worked my way up to deputy director. I led the county’s $9 million replacement of its voting equipment, and used my tech skills to build in-house tools that made the office’s work faster and more efficient.</p>
  </li>
</ol>

In my spare time, I enjoy building things, and a lot of them come back to elections: an [early voting tracker](/projects#voteflow), a [recount watch](/projects#recountwatch), and a [database of “I Voted” stickers](/projects#stickers).

Another big thing in my life is movies. I’m part of a community that does the Oscars Death Race each year, trying to watch every movie nominated in every category before the ceremony. I used to track my progress here with [Oscars checklists](/blog), and now I track it with [Oscars Watch](/projects#oscars).

I’m also a bit of a minimalist. I don’t own just [75 things](/11/02/75-things) anymore, but I don’t own much more than that. I still try to keep as few things as possible and focus on experiences, not things.

<h2 class="about-section" id="contact">Contact me</h2>

Have an idea or a suggestion, or spot an issue somewhere? Message me on one of the social networks above, or email me:

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

I started this site in 2005. I ran it on WordPress for years before moving it to [Jekyll](https://jekyllrb.com), a static site generator that turns plain text files into a fast, simple website. It’s hosted on [GitHub Pages](https://pages.github.com), and the [source code](https://github.com/rkudeshi/rkudeshi.github.io) is public.

I write posts in [Markdown](https://commonmark.org),[^view-markdown] a simple plain-text format. I usually jot down ideas in [nvALT](https://brettterpstra.com/projects/nvalt/) and flesh them out in [Sublime Text](https://www.sublimetext.com).

I’m a bit of a privacy nut, and I don’t like being tracked around the web, so I try not to do it here. I use [Cloudflare Web Analytics](https://www.cloudflare.com/web-analytics/) only for basic visitor counts. It doesn’t use cookies or follow you across sites.

[^view-markdown]: If you want to see the original Markdown for any post, just click the `M↓` link below the post title!
