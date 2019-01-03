[nuxt官网，自定义html模板](https://zh.nuxtjs.org/guide/views/)
[相关链接](https://juejin.im/post/5af17417518825670c45e34a)
通过自定义HTML模板，修改访问网址的浏览器高级程度由上到下，如果直接写content="edge"，并且用户使用的是IE浏览器，他将默认使用IE7进行访问，页面将出现混乱
```
<!DOCTYPE html>
<html {{HTML_ATTRS}}>
    <head>
        <meta http-equiv="X-UA-Compatible" content="IE=edge;IE=11;IE=10;IE=9;">
        <meta http-equiv="Cache-Control" content="no-siteapp">
        <meta name="renderer" content="webkit">
        {{HEAD}}
    </head>
    <body {{BODY_ATTRS}}>
        {{APP}}
    </body>
</html>
```
