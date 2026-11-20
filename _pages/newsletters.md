---
title         : Newsletters
description   : "The back catalog of Jesus Joshua 24:15 Newsletters"
permalink     : "/newsletters/"
redirect_from :
  - /jj_newsletter.asp
---

{% assign newsletters = site.newsletters | sort: "path" | reverse %}

<ul class="newsletter-list">
  {% for newsletter in newsletters %}
    <li>
      <a href="{{ newsletter.url | relative_url }}">
        {{ newsletter.title }}
      </a>
    </li>
  {% endfor %}
</ul>
