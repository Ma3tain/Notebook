### 函数path()
四个参数：必需两个(route(),view()),kwargs,name
<mark class="hltr-blue">route：</mark> 用于匹配相应的url地址，从urlpatterns的第一项开始顺序查找，这些准则不会匹配 GET 和 POST 参数或域名。例如，URLconf 在处理请求 `https://www.example.com/myapp/` 时，它会尝试匹配 `myapp/` 。处理请求 `https://www.example.com/myapp/?page=3` 时，也只会尝试匹配 `myapp/`
<mark class="hltr-blue">view</mark> ：当route匹配到一个存在的准则的时候，调用该函数的视图函数，传入一个httprequest对象作为第一个参数，
<mark class="hltr-blue">name：</mark> 为你的 URL 取名能使你在 Django 的任意地方唯一地引用它，尤其是在模板中。这个有用的特性允许你只改一个文件就能全局地修改某个 URL 模式。
