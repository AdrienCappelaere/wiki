# Optimisation du robots.txt

## Code à intégrer sur un WordPress

Pour les explications, aller plus bas

```text
# WordPress Robots.txt
# by Adrien Cappelaere @Digitad
# UTF-8 BOM Tested & Approved

User-agent: Googlebot

# Allow files critical for rendering
Allow: *.js
Allow: *.css

# Allow AJAX - Do Not Remove
Allow: /wp-admin/admin-ajax.php


# Prevent crawl-budget waste on search pages
Disallow: /?s=
Disallow: /search/
# Prevent private admin areas from being crawled
Disallow: /wp-admin
# Prevent duplicate /feed/ pages from being crawled
Disallow: /*/feed/
# Prevent login page crawls etc
Disallow: /wp-login.php
# Prevent register page crawls etc
Disallow: /wp-register.php
# Prevent Trackback Neg SEO
Disallow: /trackback/


User-agent: *

# Allow AJAX - Do Not Remove
Allow: /wp-admin/admin-ajax.php

Disallow: /wp-admin
Disallow: /wp-login.php
Disallow: /trackback/
Disallow: /wp-register.php

# Add all sitemaps
Sitemap: https://urldusitemap.com/
```

