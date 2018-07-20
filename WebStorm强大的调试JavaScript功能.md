<font size=4>

# webstorm 调试javascript

## 一、JavaScript的调试

目前火狐和Chrome都具备调试JavaScript的功能，而且还是相当的强大。如果纯粹是用浏览器来进行js调试的话，我比较喜欢用火狐。火狐可以安装各种插件，真的是非常适合开发者。不过今天的主角并不是火狐，也不是Chrome，而是号称最智能的JavaScript IDE：WebStorm。
> WebStorm 是jetbrains公司旗下一款JavaScript 开发工具。被广大中国JS开发者誉为“Web前端开发神器”、“最强大的HTML5编辑器”、“最智能的JavaScript IDE”等。与IntelliJ IDEA同源，继承了IntelliJ IDEA强大的JS部分的功能。

其实WebStorm之所以支持调试JavaSccript，其实也是借助了Chrome，只要Chrome安装JetBrains IDE Support插件，就可以直接在WebStorm里面进行调试了，效果那是非常的强大。

## 二、相关软件安装和配置
###  安装WebStorm 
- WebStorm官网：( https://www.jetbrains.com/webstorm/ )  

###  安装Chrome和JetBrains IDE Support   
1. JetBrains IDE Support的地址是：   
https://chrome.google.com/webstore/detail/hmhgeddbohgjknpmjagkdomcpobmllji   
2. 不过一般都是被墙了，所以得翻墙去安装插件了。   
(不懂的人可以直接安装蓝灯软件，很方便翻墙。)
![](http://img.blog.csdn.net/20170106195952925?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvc3VqdW4xMA==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
3. 配置端口(不是必须的) 
如果你的端口刚好被占用，那么记得修改相应的端口Chrome和WebStorm都要修改   
浏览器--更多工具--扩展程序--找到JetBrains IDE Support--选项
![](http://img.blog.csdn.net/20170106200130988?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvc3VqdW4xMA==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
WebStorm对应修改的地方： 
![](http://img.blog.csdn.net/20170106200155057?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvc3VqdW4xMA==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

## 三、WebStorm调试JavaScript

1. WebStorm增加JavaScript调试选项 
增加个TestJS的项目工程，直接选择Empty Project类型即可 
然后自己增加相应的html和js文件 
在工程的右上角那里，点那个下尖符号，弹出 Edit Configurations 

![](http://img.blog.csdn.net/20170106201552247?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvc3VqdW4xMA==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

点绿色的+号，然后选择JavaScript Debug 

![](http://img.blog.csdn.net/20170106201752542?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvc3VqdW4xMA==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

配置好相关路径就可以了 

  ![](http://img.blog.csdn.net/20170106201924106?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvc3VqdW4xMA==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

2. 运行调试效果 
点击那个绿色的甲虫，就可以看到实际的调试效果了。这个时候Chrome会有下面的提示 

  ![](http://img.blog.csdn.net/20170106202219904?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvc3VqdW4xMA==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
会自动切换回WebStorm的调试界面 

  ![](http://img.blog.csdn.net/20170106202348884?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvc3VqdW4xMA==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
如果仅仅是这样，那么跟其他浏览器的调试区别还是不是非常大，唯一的好处就是方便了，不用去切换。 
下面的效果我觉得才是更加的调试效果，因为他可以直接把一些参数类型、数值结果直接显示在代码上面。 
注意那个绿色的字体效果： 
  ![](http://img.blog.csdn.net/20170106202705171?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvc3VqdW4xMA==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)
  ![](http://img.blog.csdn.net/20170106202715577?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQvc3VqdW4xMA==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/SouthEast)

## 补充
- webstorm必须2017版本及以上
- 加断点之后触发webpack编译才能生效
- webpack配置启用source map（devtool:"cheap-eval-source-map"）

哦了



</font>