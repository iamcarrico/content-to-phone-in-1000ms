## iamcarrico.com

* Utilizes SPDY <!-- .element: class="fragment" -->
* Has a custom CDN <!-- .element: class="fragment" -->
  * Moved DNS to AWS Route 53  <!-- .element: class="fragment" -->
* Inlines critical CSS on first page load <!-- .element: class="fragment" -->
* Loads rest of CSS asynchronously <!-- .element: class="fragment" -->

Note:
My personal blog I did some fun testing with to find how I can make it as fast as possible. It uses SPDY (nginx -> varnish -> nginx) for all connections. Since I had custom edge side includes code, I had to create my own CDN (NYC, Amsterdam, Singapore). On first page load, the CSS will be inlined, while following page loads will utilize the browser cache.
