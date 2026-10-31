---
layout: default
---
<article class="post">

  <header class="post-header">
    <h1 class="post-title">{{ page.title | escape }} <a href="https://github.com/tactmaster/tactmaster.github.io/edit/main/{{ page.path }}" title="Edit this recipe on GitHub" style="font-size: 0.5em; text-decoration: none; vertical-align: middle;">✏️</a></h1>
  </header>

  <div class="post-content">

<p align="center">

  <img src="{{page.image}}" alt="{{page.name}}" height="200px">
  
</p>
    {{ content }}
  </div>

</article>

<style>
  .ingredient-list { position: relative; font: inherit; color: inherit; background: none; border: 0; border-bottom: 2px dotted #c9a227; padding: 0; cursor: help; }
  .ingredient-list-popup { display: none; position: absolute; left: 0; top: 100%; z-index: 10; width: max-content; max-width: min(18em, 80vw); margin-top: 4px; padding: 0.4em 0.7em; background: #fff8e1; border: 1px solid #e0c97f; border-radius: 6px; box-shadow: 0 2px 6px rgba(0, 0, 0, 0.15); font-size: 0.9em; text-align: left; white-space: normal; }
  .ingredient-list.open .ingredient-list-popup,
  .ingredient-list:focus-visible .ingredient-list-popup { display: block; }
  @media (hover: hover) {
    .ingredient-list:hover .ingredient-list-popup { display: block; }
  }
</style>
<script>
  // Tap (or click) a dotted phrase to show its ingredients; tap anywhere else to hide.
  document.addEventListener('click', function (event) {
    var clicked = event.target.closest('.ingredient-list');
    document.querySelectorAll('.ingredient-list.open').forEach(function (el) {
      if (el !== clicked) el.classList.remove('open');
    });
    if (clicked) {
      clicked.classList.toggle('open');
      keepOnScreen(clicked);
    }
  });
  document.addEventListener('mouseover', function (event) {
    var hovered = event.target.closest('.ingredient-list');
    if (hovered) keepOnScreen(hovered);
  });

  // Shift the popup left if it would go off the right edge of the screen.
  function keepOnScreen(button) {
    var popup = button.querySelector('.ingredient-list-popup');
    popup.style.left = '0';
    var overflow = popup.getBoundingClientRect().right - (document.documentElement.clientWidth - 8);
    if (overflow > 0) popup.style.left = -overflow + 'px';
  }
</script>


