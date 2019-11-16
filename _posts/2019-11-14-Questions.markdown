---
layout: post
title: "Pre-Compiled CSS"
date: 2019-11-14 02:50:11 -0600
categories: jekyll questions
comments: true
author: "Jimmy Truong"
---

## What do you think of static site generators?

## What type of projects are they suitable for?

## What is humans.txt and how have you configure it for your site?

## How did you implement comments to blog posts?

I used disqus for my blog. The guideline were very simple. Everything can be found on https://disqus.com/admin/install/platforms/jekyll/

## What is Open Graph and how do you make use of it?

{% if page.comments %}

<div id="disqus_thread"></div>
<script>

    (function() {
        var d = document, s = d.createElement('script');

        s.src = '//jimmytruong-1.disqus.com/embed.js';  // IMPORTANT: Replace EXAMPLE with your forum shortname!

        s.setAttribute('data-timestamp', +new Date());
        (d.head || d.body).appendChild(s);
    })();

</script>

<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript" rel="nofollow">comments powered by Disqus.</a></noscript>

{% endif %}
