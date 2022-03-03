---
layout: default
---
<article class="post">

  <header class="post-header">
    <h1 class="post-title">{{ page.title | escape }}</h1>
  </header>

  <div class="post-content">

<p align="center">

  <img src="{{page.image}}" alt="{{page.name}}" height="200px">
  
</p>
    {{ content }}
  </div>

</article>


