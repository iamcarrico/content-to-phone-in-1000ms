## What is it?

* Multiplexed streams <!-- .element: class="fragment" -->
* Request prioritization <!-- .element: class="fragment" -->
* Server push <!-- .element: class="fragment" -->
* Removal of redundant headers <!-- .element: class="fragment" -->
* Compressed headers <!-- .element: class="fragment" -->


Note:
SPDY has a lot of optimizations and performance benefits. It has been setup to allow a drop in solution for apache and nginx. The biggest benefit SPDY gives off the back is the use of multiplexed streams, allowing for multiples files to use a single TCP connection. This removes the need for multiple TCP handshakes, each of which could cost 100's of milliseconds. With that also comes the need to prioritize requests, which the client can prioritize high-importance items over others. The server can also push resources to the client, instead of the client needing to make individual requests for everything. Finally, they will remove redundant headers, and compress any that are needed. 
