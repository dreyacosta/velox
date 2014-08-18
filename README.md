# Velox

Responsive and minimal theme for Ghost focus on speed, typography and semantic.

First velox 0.2.0 preview

![velox 0.2.0](https://raw.githubusercontent.com/dreyacosta/velox/ghost-0.5.0/velox-0.2.0-preview.jpg)

## Optional set up

### Nav menu

**index.hbs**, **page.hbs** and **post.hbs**: customize your nav menu
```
{{!
  Here, you can add your nav menu.
  Also go to partials/nav-menu.hbs to set your links.
}}
{{> nav-menu}}
```

### Google Analytics

**default.hbs**: uncomment `{{!> google-analytics}}` to `{{> google-analytics}}`
```
{{!
  Here, you can add Google Analytics.
  Also go to partials/google-analytics.hbs to set your ID and DOMAIN.
}}
{{> google-analytics}}
```

**partials/google-analytics.hbs**: set your `TRACK-ID` and `DOMAIN.com`
```
<script>
  (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
    (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
    m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
  })(window,document,'script','//www.google-analytics.com/analytics.js','ga');

  ga('create', 'YOUR-TRACK-ID', 'yourdomain.com');
  ga('send', 'pageview');
</script>
```

### Disqus comments

**page.hbs** and **post.hbs**: uncomment `{{!> disqus-comment}}` to `{{> disqus-comment}}`
```
{{!
  Here, you can add disqus comment.
  Also go to partials/disqus-comment to set your SHORTNAME.
}}
{{!> disqus-comment}}
```

**partials/disqus-comment.hbs**: set your `disqus_shortname`
```
<div id="disqus_thread" class="margin_top_big"></div>
<script type="text/javascript">
  /* * * CONFIGURATION VARIABLES: EDIT BEFORE PASTING INTO YOUR WEBPAGE * * */
  var disqus_shortname = 'YOUR-DISQUS-SHORTNAME'; // required: replace example with your forum shortname

  /* * * DON'T EDIT BELOW THIS LINE * * */
  (function() {
    var dsq = document.createElement('script'); dsq.type = 'text/javascript'; dsq.async = true;
    dsq.src = '//' + disqus_shortname + '.disqus.com/embed.js';
    (document.getElementsByTagName('head')[0] || document.getElementsByTagName('body')[0]).appendChild(dsq);
  })();
</script>
```