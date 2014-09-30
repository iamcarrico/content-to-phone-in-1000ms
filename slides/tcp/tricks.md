## HTTP 1.1 Tricks

* Domain sharding <!-- .element: class="fragment" -->
* Concatenation <!-- .element: class="fragment" -->
* Spriting <!-- .element: class="fragment" -->
* Inlining of assets <!-- .element: class="fragment" -->

The fastest request you will ever make, is the one you don't. <!-- .element: class="fragment" -->

Note:
Most modern browsers will open ~6 tcp connections per domain to download more assets. Thus enters domain sharding, where we create separate subdomains for a set of 6 assets, thus being able to load them. We can also concatenate assets to have fewer requests. This is great, except for when assets change often, which will cause large re-downloads for minor changes. Spriting images also allows for less requests to be made. Finally, inlining of assets removes entire requests.
