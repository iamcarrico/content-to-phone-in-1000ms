## CSS

<ol>
  <li class="fragment">Inline critical CSS (the fold is back!)</li>
  <li class="fragment">Load the rest of CSS asynconously (LoadCSS)</li>
</ol>

<div class="drupal fragment">There is no "out of the box" Drupal solution for this (Yet!)</div>

Note:
Unlike HTML, that can be parsed as it comes down, the CSSOM needs to be parsed as one. Luckily, browsers are REALLY good at doing this. But, we need to get an entire CSSOM to the browser quickly, and this will mean inlining the critical CSS. 
