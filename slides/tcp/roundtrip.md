## A Roundtrip

<div class="roundtrip clearfix">
  <div class="column">
    <div class="row fragment" data-fragment-index="1">&nbsp;</div>
    <div class="row fragment" data-fragment-index="1">DNS Lookup</div>
    <div class="row fragment" data-fragment-index="2">TCP Connection</div>
    <div class="row fragment" data-fragment-index="3">TLS Handshake</div>
    <div class="row fragment" data-fragment-index="4">HTTP Request</div>
    <div class="row fragment" data-fragment-index="5">Total</div>
  </div>
  <div class="column">
    <div class="row fragment" data-fragment-index="1">Google Fiber</div>
    <div class="row fragment" data-fragment-index="1">40ms</div>
    <div class="row fragment" data-fragment-index="2">60ms</div>
    <div class="row fragment" data-fragment-index="3">60-120ms</div>
    <div class="row fragment" data-fragment-index="4">60ms</div>
    <div class="row fragment" data-fragment-index="5">220-280ms</div>
  </div>
  <div class="column fragment" data-fragment-index="6">
    <div class="row ">LTE</div>
    <div class="row ">100ms</div>
    <div class="row ">100ms</div>
    <div class="row ">100-200ms</div>
    <div class="row ">100ms</div>
    <div class="row ">400-500ms</div>
  </div>
  <div class="column fragment" data-fragment-index="7">
    <div class="row">3G</div>
    <div class="row">200ms</div>
    <div class="row">200ms</div>
    <div class="row">200-400ms</div>
    <div class="row">200ms</div>
    <div class="row">800-1000ms</div>
  </div>
</div>


Note:
What happens we we request a URL in our browser that we have not been to before? The browser will do a DNS lookup, then create a TCP connection, then (maybe) a TLS handshake for SSL, then we can finally make our first HTTP request. For fiber connections, that isn't so bad, but what about LTE or 3G connections. We quickly deplete our 1000ms budget to almost nothing.
