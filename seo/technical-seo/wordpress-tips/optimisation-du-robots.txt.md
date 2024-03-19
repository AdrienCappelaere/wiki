# Optimisation du robots.txt

## Code à intégrer sur un WordPress

Pour les explications, aller plus bas

```
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

## Tips pour une bonne utilisation

### Où intégrer ce robots.txt ?

#### Avec Yoast SEO

![](<../../../.gitbook/assets/image (3).png>)

![](<../../../.gitbook/assets/image (1).png>)

1. Cliquer sur _Outils_ dans l'onglet _SEO_
2. Cliquer sur _Éditeur de fichiers_
3. Coller le robots.txt optimisé dans l'espace dédié, et y ajouter le bon sitemap.xml
4. Enregistrer les changements de robots.txt

#### Avec RankMath SEO

![](<../../../.gitbook/assets/image (2).png>)

1. Entrer dans les réglages généraux
2. Cliquer sur _Modifier le robots.txt_
3. Coller le robots.txt optimisé dans l'espace dédié, et y ajouter le bon sitemap.xml
4. Sauvegarder les modifications
