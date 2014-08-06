## sudo bundle install

<h1 class="fragment">DO NOT DO THIS</h1>
<h2 class="fragment">... seriously</h1>
<h3 class="fragment">... ever</h3>

Note: Running bundle install as sudo will have unexpected consequences, as bundler needs to put some files into your user profile. If you are tempted to do so, then just install all gems into the .vendor folder instead.
