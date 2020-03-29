---
title: 
menus:
  main:
    title: Posts
    weight: 2
layout: page
---


<section id="{{ include.section.section_id }}" class="posts">
  <ul>
    {% for post in site.posts %}
      <a href="{{ post.url }}" class="article-teaser">
        <div class="copy">
            <h2>{{ post.title }}</h2>
            <h3 class="publish-date">Published on {{ post.date | date: '%B %d, %Y' }}</h3>

            <p class="summary">{{ post.excerpt }}</p>
            <div class="text-link">Read more</div>
        </div>
      </a>
    {% endfor %}
  </ul>
</section>
