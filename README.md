# ProBrain 홈페이지 관리
## 레이아웃 수정
- 각 md 파일의 layout 속성 확인
- 해당 layout에 맞는 html 파일을 _layouts 폴더에서 찾아서 수정

## 카테고리 (게시판) 추가
1. categories 폴더에 추가하고자하는 카테고리 폴더를 생성
2. index.md 파일을 작성
### index.md 예시
```md
---
layout: archive
title: "News"
image:
  feature: probrain-menu.png
---

<div class="tiles">
{% for post in site.categories.news %}
  {% include post-grid.html %}
{% endfor %}
</div><!-- /.tiles -->
```
3. _data/navigation.yml에 새로운 카테고리를 연결
```yml
...
- title: News                   # 카테고리 이름
  url: /categories/news/        # 해당 카테고리의 index.md 파일이 있는 경로
  excerpt: "News Excerpt Test"  # 해당 카테고리의 발췌 문구 (아래 사진 참고)
  image:
...
```
![Excerpt Example](./images/excerpt-example.jpg)  
  
4. _posts 폴더에 새로운 카테고리의 게시글을 위한 폴더 생성

## 게시글 추가
1. _posts 폴더에서 추가하고자하는 게시글의 카테고리에 해당하는 폴더에 md 파일 생성
2. 예시 파일들을 참고하여 게시글 작성 (categories 속성은 게시글을 포스팅하고자하는 카테고리로 지정해주어야 함)
```md
---
layout: article
title: "2019 임원진 소개"
categories: news
comments: true
share: false
ads: false
---
- **회장**: 김수연
- **부회장**: 김태준
- **총무**: 서주연
- **서기**: 서보윤
- **관리부장**: 권연우
- **교육부장**: 김기환
- **기술부장**: 김다은
- **홍보부장**: 김연우
- **체육부장**: 김지수
- **예능부장**: 김현아
- **여학우부장**: 인예림
- **환경부장**: 황규진
```