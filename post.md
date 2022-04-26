---

title:  "github.io 블로그  첫 글"

excerpt: "github.io 블로그 첫 글 작성해봅니다."

categories:

  - Blog

tags:

  - Blog

last_modified_at: 2019-04-13T08:06:00-05:00

---

글작성하기 위해 마크다운을 공부해서 
좋은 글들을 작성해 보자.

이 글의 제목은 {{ page.title }}이고

마지막 수정 시간은 {{ page.last_modified_at }}이다.

<header class="header-page">
  <h1 class="page-title">{{page.title}}</h1>
  {% if page.last_modified_at %}
    <div class="page-date"><span>{{page.last_modified_at | date: '%Y, %b %d'}}&nbsp;&nbsp;&nbsp;&nbsp;</span></div>
  {% else %}
    <div class="page-date"><span>{{page.date | date: '%Y, %b %d'}}&nbsp;&nbsp;&nbsp;&nbsp;</span></div>
  {% endif %}
</header>
