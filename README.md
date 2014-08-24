# Velox

Responsive and minimal theme for Ghost focus on speed, typography and semantic.

![velox 0.2.0](https://raw.githubusercontent.com/dreyacosta/velox/ghost-0.5.0/screenshots/velox-0.2.0-preview.jpg)

## PageSpeed test
Test made with Google Analytics and Prism scripts on a page without images.

![PageSpeed Mobile](https://raw.githubusercontent.com/dreyacosta/velox/ghost-0.5.0/screenshots/pagespeed-mobile.jpg)

![PageSpeed Desktop](https://raw.githubusercontent.com/dreyacosta/velox/ghost-0.5.0/screenshots/pagespeed-desktop.jpg)

## W3C validation

![W3C Home validation](https://raw.githubusercontent.com/dreyacosta/velox/ghost-0.5.0/screenshots/w3c-markup-home.jpg)

![W3C Author validation](https://raw.githubusercontent.com/dreyacosta/velox/ghost-0.5.0/screenshots/w3c-markup-author.jpg)

![W3C Tag validation](https://raw.githubusercontent.com/dreyacosta/velox/ghost-0.5.0/screenshots/w3c-markup-tag.jpg)

## Optional set up

#### Google Analytics
default.hbs line 54:
```
{{> google-analytics}}
```
google-analytics.hbs line 7:
```
ga('create', 'YOUR-TRACK-ID', 'yourdomain.com');
```

#### Disqus
post.hbs line 42:
```
{{> disqus-comment}}
```
partials/disqus-comment.hbs line 4:
```
var disqus_shortname = 'YOUR-DISQUS-SHORTNAME';
```

#### Authorship
default.hbs line 19:
```
<link rel="author" href="//plus.google.com/YOUR-ID?rel=author" />
```

#### Twitter cards
default.hbs line 28:
```
<meta name="twitter:creator" content="@yourTwitterUsername">
```

#### Fonts
default.hbs line 48:
```
{{> load-fonts}}
```

#### Prism syntax highlighter
default.hbs line 49:
```
{{> load-prism}}
```