## Reduce redirects

# REMOVE Redirects <!-- .element: class="fragment" -->


Note:
Every redirect you do adds on extra (unneeded) round trip. This includes redirecting one domain to another, or even redirecting from http to https. There are many ways of removing redirects. Sharing direct links to content.
If you are using https only, you can add the 'strict-transport-security' headers to your site, so that all subsequent loads always use https. There is also the ability of adding your site to Google/Mozillas HSTS list.
