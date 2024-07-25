-  首先访问https://search.google.com/search-console/welcome
- 建议使用网址前缀方案
<img width="763" alt="image" src="https://github.com/user-attachments/assets/37af19b3-15a1-4091-87fc-882d1b7f14f3">
- 随后添加自己的blog地址
- html标记的方式最为方便，直接在config.jso添加字符即可 
<img width="646" alt="image" src="https://github.com/user-attachments/assets/75012edd-64bf-46e5-b000-fbb06db3cde2">

- 在allhead 字段直接添加对应字符即可

```python
"allHead":"<script src='https://blog.meekdai.com/Gmeek/plugins/GmeekBSZ.js'></script> <script src='https://blog.meekdai.com/Gmeek/plugins/GmeekVercount.js'></script> <meta name='google-site-verification' content='1VMjcA03zLI8aKEYQ3WOXgkTtOBe--5NNn6YKpeAxzQ' />",
```

- 随后返回google验证即可

- 后续在作者大大的帮助下，js也可以很好的把blog喂给google了。可以[参考](https://github.com/Meekdai/Gmeek/issues/87#issuecomment-2249763145)

```
"allHead":"<script src='https://blog.meekdai.com/Gmeek/plugins/GmeekBSZ.js'></script> <script src='https://blog.meekdai.com/Gmeek/plugins/GmeekVercount.js'></script> <meta name='google-site-verification' content='1VMjcA03zLI8aKEYQ3WOXgkTtOBe--5NNn6YKpeAxzQ' /> <script async src='https://www.googletagmanager.com/gtag/js?id=G-xxxxxx'></script><script>window.dataLayer = window.dataLayer || [];function gtag(){dataLayer.push(arguments);}gtag('js', new Date());gtag('config', 'G-xxxxx');</script>",
```

