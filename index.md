---
layout: home
permalink: /
title: "Main"
image:
  mainimage: main-image.jpg
---

<div class="tiles">

<div class="tile">
  <h2 class="post-title">ProBrain?</h2>
  <p class="post-excerpt">ProBrain(Professional Brain Group, 프로브레인)은 충남대학교 컴퓨터공학과 소속의 학술동아리 입니다. 저희는 차세대 웹 기술을 연구하는 동아리로서 이 기술에 창의적 아이디어와 디자인을 더해 많은 사용자들을 끌어들일 수 있는 웹 환경의 개발을 목표로 삼고 활동 중에 있습니다.</p>
</div><!-- /.tile -->

<div class="tile">
  <h2 class="post-title">News</h2>
  {% for post in site.categories.news limit: 5 %}
    <a href="{{ post.url }}"><p 
      {% if forloop.first %}
      style="margin-bottom: 0;"
      {% else %}
      style="margin: 0;"
      {% endif %}
      >{{ post.title }}</p></a>
  {% endfor %}
</div><!-- /.tile -->

<div class="tile">
  <h2 class="post-title">Gallery</h2>
  {% for post in site.categories.gallery limit: 5 %}
    <a href="{{ post.url }}"><p 
      {% if forloop.first %}
      style="margin-bottom: 0;"
      {% else %}
      style="margin: 0;"
      {% endif %}
      >{{ post.title }}</p></a>
  {% endfor %}
</div><!-- /.tile -->

<div class="tile">
  <h2 class="post-title">Event</h2>
  {% for post in site.categories.event limit: 5 %}
    <a href="{{ post.url }}"><p 
      {% if forloop.first %}
      style="margin-bottom: 0;"
      {% else %}
      style="margin: 0;"
      {% endif %}
      >{{ post.title }}</p></a>
  {% endfor %}
</div><!-- /.tile -->
</div><!-- /.tiles -->
