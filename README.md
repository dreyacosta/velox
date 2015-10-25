# Velox

Responsive and minimal theme for Ghost focus on speed, typography and semantic.

![velox 0.3.0](https://raw.githubusercontent.com/dreyacosta/velox/ghost-0.5.0/screenshots/velox-0.3.0-preview.jpg)

## Support

- Author page
- Tag page
- Image post
- Syntax highlighter
- Meta data for SEO
- Disqus comments
- Post read next and previous

## PageSpeed test
Test made with Google Analytics and Prism scripts on a page without images.

![PageSpeed Mobile](https://raw.githubusercontent.com/dreyacosta/velox/ghost-0.5.0/screenshots/pagespeed-mobile.jpg)

![PageSpeed Desktop](https://raw.githubusercontent.com/dreyacosta/velox/ghost-0.5.0/screenshots/pagespeed-desktop.jpg)

## W3C validation

![W3C Home validation](https://raw.githubusercontent.com/dreyacosta/velox/ghost-0.5.0/screenshots/w3c-markup-home.jpg)

![W3C Author validation](https://raw.githubusercontent.com/dreyacosta/velox/ghost-0.5.0/screenshots/w3c-markup-author.jpg)

![W3C Tag validation](https://raw.githubusercontent.com/dreyacosta/velox/ghost-0.5.0/screenshots/w3c-markup-tag.jpg)

## Customize CSS
According [CSS optimization rules of Google](https://developers.google.com/speed/docs/insights/OptimizeCSSDelivery), CSS is deliver inline (default.hbs line 33).

You can customize CSS with [stylus](https://github.com/dreyacosta/velox/assets/stylesheets).

## Optional set up

#### Google Analytics
default.hbs line 48:
```
{{> loaders/load-google-analytics}}
```
partials/loaders/load-google-analytics.hbs line 7:
```
ga('create', 'YOUR-TRACK-ID', 'yourdomain.com');
```

#### Disqus
post.hbs line 65:
```
{{> loaders/load-disqus-comment}}
```
partials/loaders/disqus-comment.hbs line 4:
```
var disqus_shortname = 'YOUR-DISQUS-SHORTNAME';
```

#### Authorship
default.hbs line 24:
```
<link rel="author" href="//plus.google.com/YOUR-ID?rel=author" />
```

#### Fonts
default.hbs line 41:
```
{{> loaders/load-fonts}}
```

#### Prism syntax highlighter
default.hbs line 42:
```
{{> loaders/load-prism}}
```

#### Lazy background cover
default.hbs line 43:
```
{{> loaders/load-lazycover}}
```

## License
This software is free to use under the MIT license.
