# 从URL输入到页面展现的过程


总体来说分为以下几个过程:


1. ### DNS解析
    把您输入的网址翻译成IP地址。
    查找顺序为：浏览器缓存、系统缓存、路由器缓存、ISP DNS 缓存、递归搜索。
    
    
2. ### 建立TCP连接
    三次握手。


3. ### 发送HTTP请求
    构建HTTP请求报文并通过TCP协议中发送到服务器指定端口(HTTP协议80/8080, HTTPS协议443)。
    HTTP请求报文是由三部分组成: 请求行、请求报头和请求正文。
    
    
4. ### 服务器响应请求并返回HTTP报文
    常见的Web服务器有Apache、Nginx、lls、Lighttpd等。
    网站处理流程：MVC模型(model)-视图(view)-控制器(controller)。
    
    
5. ### 浏览器解析渲染页面
   1. HTML字符串被浏览器接受后被一句句读取解析。
   
   2. 解析到 link 标签后重新发送请求获取css。
   
   3. 解析到 script 标签后发送请求获取 js，并执行代码。
   
   4. 解析到 img 标签后发送请求获取图片资源。
   
   5. 浏览器根据 HTML 和 CSS 计算得到渲染树，绘制到屏幕上js 会被执行。
   
   
6. ### 连接结束


参考：

- https://segmentfault.com/a/1190000006879700

- http://www.cnblogs.com/strick/p/5494869.html

以后会继续修改整理。
