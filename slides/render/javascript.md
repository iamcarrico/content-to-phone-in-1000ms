## JavaScript

<ol>
  <li class="fragment">Move JavaScript to the footer</li>
  <li class="fragment">Utilize async / defer</li>
  <li class="fragment">Inline critical JS</li>
</ol>

<div class="drupal fragment">Use the Magic Module</div>

Note:
JavaScript in the header will block the rendering of the page. To prevent this, we can move most of our JavaScript to the footer, or load it asynchronously. Within Drupal, the easiest way to do this is my enabling the Magic module. 
