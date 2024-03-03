---
list_title: Latest Posts
layout: default
---

<article class= "top">
  <div class="wrapper">
    <div class="box box1">
      <img src="https://kadetat.github.io/Laton-Company/images/latonlogo.PNG" alt="Profile Pic">
    </div>
  </div>
  <h1 class="OutlineText"> Janae Talbott - Rural Revitalizer, Innovator, Creator </h1>
  <h2>My Blog</h2>

  <div class="row" style="background-color: #F9F9F9; padding-inline: 2%; padding-top: 2%; padding-bottom: 1%;  border-radius: 25px; margin-left: 25%; margin-right: 25%;">
      <div class="col-sm-3">
        <img src="https://kadetat.github.io/Laton-Company/images/profilepic.PNG" alt="Profile Pic" width="125" height="125" style="float:right">
      </div>
      <div class="col-md-9" style="text-align:left;">
        <p> ************************description*************************** </p>
        <p> ************************description*************************** </p>
        <p> ************************description*************************** </p>
      </div>
  </div>
</article>

{%- if posts.size > 0 -%}
    {%- if page.list_title -%}
      <h2 class="post-list-heading">{{ page.list_title }}</h2>
    {%- endif -%}
    <ul class="post-list">
      {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
      {%- for post in posts -%}
      <li>
        <span class="post-meta">{{ post.date | date: date_format }}</span>
        <h3>
          <a class="post-link" href="{{ post.url | relative_url }}">
            {{ post.title | escape }}
          </a>
        </h3>
        {%- if site.show_excerpts -%}
          {{ post.excerpt }}
        {%- endif -%}
      </li>
      {%- endfor -%}
    </ul>
  {%- endif -%}
