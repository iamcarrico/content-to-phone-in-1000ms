## First Packet Response

* RFC 6928: 10 packets <!-- .element: class="fragment" -->
* 14.6kb <!-- .element: class="fragment" -->
* <!-- .element: class="fragment" --> [https://iamcarrico.com](https://iamcarrico.com)


Note:
A server will respond with 4 packets (RFC 2581) or 10 packets (RFC 6928), depending on your server's config. If you are using 10 packets (and you should), then that means the first packet response will be 14.6kb. If you can deliver the full render tree in a single response in that time, then you're site will load after the completion of a single HTTP resquest.
