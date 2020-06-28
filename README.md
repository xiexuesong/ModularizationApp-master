# Android 组件化开发demo
组件化开发可以有效降低代码模块的耦合度，使代码架构更加清晰，同时模块化的编译可以有效减少编译时间，当然总的编译时间是不会减少的，只是App模块化之后开发某个模块时，只需要编译特定模块，可以快速编译调试。

[详情参考](http://www.jianshu.com/p/186fa07fc48a)

![Paste_Image.png](http://upload-images.jianshu.io/upload_images/1407686-2bb840fdef5d9ac2.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/200)![Paste_Image.png](http://upload-images.jianshu.io/upload_images/1407686-eb097c7ce3473583.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/200)![Paste_Image.png](http://upload-images.jianshu.io/upload_images/1407686-74e5145beda0702e.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/200)![Paste_Image.png](http://upload-images.jianshu.io/upload_images/1407686-bb950d3382d8e90b.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/200)![Paste_Image.png](http://upload-images.jianshu.io/upload_images/1407686-a5924d98324b3762.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/200)

### 编译运行

当在gradle.properties中设置IsBuildMudle=true时，可以独立运行每个module，包括app module，单独build module app时，由于没有编译moduleA和moduleB，点击两个模块时不会跳转。每个module可独立运行调试。

当设置IsBuildMudle=false，可以编译运行整个project，注意IsBuildMudle变量设置改变时，要对gradle进行sysn。

有什么奇怪问题，可以clean project再编译……^ - ^

### 感谢

http://kymjs.com/code/2016/10/18/01
https://github.com/mzule/ActivityRouter
https://github.com/liangzhitao/ComponentizationApp

### issue

关于url跳转传参数的一个问题

https://github.com/mzule/ActivityRouter/issues/17
# ModularizationApp-master
