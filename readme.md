已经对原来项目chineseocr进行了删减没用的数据.
模型数据都存在了这里,方便下载.也可以去setup.md里面找百度云链接.
https://v2.fangcloud.com/share/f9fe056b9d78b3b98a548ec68d


pytorch:1.1.0版本!!!!!!!!!


manage.py
用flask来开启服务,就这一个文件够了.


运行python manage.py
请求:
116.196.87.166:5080

pic:  img.jpeg










下一步看这种深度网络模型如何服务模型文件,锁内存中,来提高访问速度?
目前只想到了静态变量来提高速度.
然后看看如何加入文字识别方向,现在是4个方向,感觉至少弄成8个方向才够.

2019-09-12,22点17
好像可以用with 语句来保存模型的内部东西
https://www.jianshu.com/p/43da2553a2fb

https://www.imooc.com/wenda/detail/468056





2019-09-13,11点00
部署细节:
直接把import这种东西都放test.py的函数外面,就始终放内存中了.提高检测速度了.




