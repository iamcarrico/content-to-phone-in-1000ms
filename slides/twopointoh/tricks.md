## Tricks 2.0

* Do not use domain sharding <!-- .element: class="fragment" -->
* Concatenation can hurt performance <!-- .element: class="fragment" -->
* Utilize Server.push for important assets <!-- .element: class="fragment" -->

<br>

<div class="drupal fragment">HTTP/2 module is in research</div>

Note:
Many of the tricks we used in HTTP 1.1 can cause issues for HTTP/2, mainly domain sharding and concatination. The former will open more tcp connections are are not needed for HTTP/2, the later will mean entire assets are reloaded when small changes are made to any piece. Finally, where possible, push assets to the user instead of requiring the client to request them.
