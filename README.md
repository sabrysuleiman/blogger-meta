# blogger-meta
Meta tag for Blogger

```
  <head>
    <title><data:view.title.escaped/></title>
    <link expr:href='data:view.url.canonical' rel='canonical'/>
    <meta expr:content='data:view.description' name='description'/>
    <meta expr:content='data:view.title' itemprop='name'/>
    <b:if cond='data:view.featuredImage'>
      <meta expr:content='data:view.featuredImage' itemprop='image'/>
    </b:if>
    <meta expr:content='data:view.url.canonical' property='og:url'/>
    <b:if cond='data:view.isSingleItem'>
      <meta content='article' property='og:type'/>
    </b:if>
    <meta expr:content='data:view.title' property='og:title'/>
    <b:if cond='data:view.featuredImage'>
      <meta expr:content='data:view.featuredImage' property='og:image'/>
      <meta expr:content='data:view.title' property='og:image:alt'/>
    </b:if>
    <meta expr:content='data:view.description' property='og:description'/>
    <meta expr:content='data:blog.title' property='og:site_name'/>
    <meta expr:content='data:blog.locale' property='og:locale'/>
    <b:if cond='data:view.featuredImage'>
      <meta content='summary_large_image' name='twitter:card'/>
      <meta expr:content='data:view.title' name='twitter:title'/>
      <meta expr:content='data:view.description' name='twitter:description'/>
      <meta expr:content='data:view.featuredImage' name='twitter:image'/>
      <meta expr:content='data:view.url.canonical' name='twitter:url'/>
      <meta content='@rizyskiptra' name='twitter:site'/>
      <b:else/>
      <meta content='summary' name='twitter:card'/>
      <meta expr:content='data:view.title' name='twitter:title'/>
      <meta expr:content='data:view.description' name='twitter:description'/>
      <meta expr:content='data:view.url.canonical' name='twitter:url'/>
      <meta content='@rizyskiptra' name='twitter:site'/>
    </b:if>
    <meta charset='utf-8'/>
    <meta content='width=device-width, initial-scale=1' name='viewport'/>
    <meta content='IE=Edge' http-equiv='X-UA-Compatible'/>
    <meta content='#3ddc84' name='theme-color'/>
    <b:tag cond='data:blog.googleProfileUrl' expr:href='data:blog.googleProfileUrl' name='link' rel='publisher'/>
    <b:tag cond='data:view.featuredImage' expr:href='data:view.featuredImage' name='link' rel='image_src'/>
    <link expr:href='data:blog.blogspotFaviconUrl' rel='icon' type='image/x-icon'/>
  </head>
```
