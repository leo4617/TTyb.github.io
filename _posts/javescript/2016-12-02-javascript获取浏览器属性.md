---
layout: post
categories: [javascript]
title: javascript获取浏览器属性
date: 2016-12-02
author: TTyb
desc: "javascript获取浏览器属性"
---

### 直接上代码

```
navigator.appName：浏览器名称；
navigator.appVersion：浏览器版本；
navigator.language：浏览器设置的语言；
navigator.platform：操作系统类型；
navigator.userAgent：浏览器设定的User-Agent字符串。
```


```
'use strict';
alert('appName = ' + navigator.appName + '\n' +
      'appVersion = ' + navigator.appVersion + '\n' +
      'language = ' + navigator.language + '\n' +
      'platform = ' + navigator.platform + '\n' +
      'userAgent = ' + navigator.userAgent);
```

![](http://images2015.cnblogs.com/blog/996148/201612/996148-20161202110902693-762272230.png)


```
screen.width：屏幕宽度，以像素为单位；
screen.height：屏幕高度，以像素为单位；
screen.colorDepth：返回颜色位数，如8、16、24。
```


```
'use strict';
alert('Screen size = ' + screen.width + ' x ' + screen.height);
```

![](http://images2015.cnblogs.com/blog/996148/201612/996148-20161202110927756-2075154505.png)

>http://www.example.com:8080/path/index.html?a=1&b=2#TOP


```
location.protocol; // 'http'
location.host; // 'www.example.com'
location.port; // '8080'
location.pathname; // '/path/index.html'
location.search; // '?a=1&b=2'
location.hash; // 'TOP'
```


```
'use strict';
if (confirm('重新加载当前页' + location.href + '?')) {
    location.reload();
} else {
    location.assign('/discuss'); // 设置一个新的URL地址
}
```


![](http://images2015.cnblogs.com/blog/996148/201612/996148-20161202111153037-22700067.png)


```
'use strict';
// 获取当前浏览器title
alert(document.title)
// 更改title
document.title = '百哥么么哒';
```


![](http://images2015.cnblogs.com/blog/996148/201612/996148-20161202111100349-925986790.png)


```
// 获取cookie
alert(document.cookie)
```

![](http://images2015.cnblogs.com/blog/996148/201612/996148-20161202111116865-458313086.png)

