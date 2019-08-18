---
layout: home
permalink: /
title: "Main"
image:
  mainimage: main-image.jpg
---

<div class="tiles">
{% for post in site.posts %}
	{% include post-grid.html %}
{% endfor %}
<div class="tile">
  <h2 class="post-title">ProBrain?</h2>
  <p class="post-excerpt">ProBrain(Professional Brain Group, 프로브레인)은 충남대학교 컴퓨터공학과 소속의 학술동아리 입니다. 저희는 차세대 웹 기술을 연구하는 동아리로서 이 기술에 창의적 아이디어와 디자인을 더해 많은 사용자들을 끌어들일 수 있는 웹 환경의 개발을 목표로 삼고 활동 중에 있습니다.</p>
</div><!-- /.tile -->

<div class="tile">
  <h2 class="post-title">Content First</h2>
  <p class="post-excerpt">Designed to put the focus on you and your writing. Headers, navigation, sidebars, and footers have been purposely deemphasized.</p>
</div><!-- /.tile -->

<div class="tile">
  <h2 class="post-title">Customizable</h2>
  <p class="post-excerpt">Packed with layouts and modules. Include Disqus comments, social sharing buttons, and table of contents on one or all pages.</p>
</div><!-- /.tile -->

<div class="tile">
  <h2 class="post-title">Extensible</h2>
  <p class="post-excerpt">Compatible with popular libraries like <a href="http://bourbon.io">Bourbon</a>, <a href="http://neat.bourbon.io/">Neat</a>, and <a href="http://github.com/octopress/octopress">Octopress</a> to help build and deploy your site with ease.</p>
</div><!-- /.tile -->
</div><!-- /.tiles -->
