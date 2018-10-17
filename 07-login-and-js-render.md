# 简单爬虫的困难

需要登录的网站：登录后才能看见网站的内容，直接用爬虫没有登录。

动态渲染的页面：越来越多的网站使用 JavaScript 动态构建页面，最终浏览器看到的页面和请求返回的页面不一样。

# Cookie

网站一般使用 Cookie 来记住登录状态。

当网站设置 Cookie 时，响应会加上 `Set-Cookie` 头。

请求通过加上 `Cookies` 头去告诉网站自己的登录状态。

# 动态渲染

当静态页面没有包含。

Chrome Driver 是自动化的 Chrome 浏览器, 我们可以通过编程的方式控制它访问页面并获得动态渲染后的内容。

Selenium 是自动化网页操作的框架。

结合 Selenium 和 Chrome Driver，我们可以完成动态网页的爬取。