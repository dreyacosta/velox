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

## Customize CSS
According [CSS optimization rules of Google](https://developers.google.com/speed/docs/insights/OptimizeCSSDelivery), CSS is deliver inline (default.hbs line 33).

You can customize CSS with [xpressio](https://github.com/dreyacosta/xpressio) framework. You can find the [xpressio Velox theme here](https://github.com/dreyacosta/xpressio/tree/master/source/themes/velox) and [how to compile with Grunt](https://github.com/dreyacosta/xpressio#build-your-theme).

## Optional set up

#### Google Analytics
default.hbs line 42:
```
{{> google-analytics}}
```
google-analytics.hbs line 7:
```
ga('create', 'YOUR-TRACK-ID', 'yourdomain.com');
```

#### Disqus
post.hbs line 68:
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

#### Fonts
default.hbs line 36:
```
{{> load-fonts}}
```

#### Prism syntax highlighter
default.hbs line 37:
```
{{> load-prism}}
```

## License
This software is free to use under the MIT license.