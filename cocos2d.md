#2015 Unique Studio Android Team Stay Up Examination

##第一题

####用cocos2d实现地图动态加载：

* 地图为类似天天酷跑横向移动，有背景和地面两层；
* 镜头会以一定速度前进，**你需要预先把前方的地图加载出来**；
* 背景图循环出现，首尾相接；
* 地面是按x坐标分块的，可随意做出阶梯或高低高低的形状等，循环出现；
* 注意：图片资源自选；**当后方地图移动至屏幕外后要移除**；还有把显示帧率开启；
* 提交源码（不限c++，js，lua）和apk文件；

##第二题

####用cocos2d自定义场景切换效果：

 * 你需要实现两个游戏场景切换的幕布状效果；
 * 幕布为一张图片，**从上方落下盖住场景1**，停顿少许，**然后收起露出场景2**；
 * 场景1和场景2只要放两张不同的图片就可以了；
 * **最好写成一个方法**，可通过sence1->myReplaceScene(sence2)使用；
 * 提示：如果遇到困难可用layer代替sence；
 * 提交源码（不限c++，js，lua）；

##第三题

 ####用cocos2d-x创建一个Action类:

 * 构造一个Actions类继承于*ActionInterval*，实现正**五角星运动**。
 * create函数传入的参数包括**运动时间**，**起始坐标**，**五角星边长**。
 * 运动轨迹从五角星顶上顺时针运动，不限C++,Lua,Js。
 * 附加题：优雅地实现可定义**五角星角度**与**顺逆时针方向**。

##第四题

####用cocos2d-x实现双摇杆，需求如下：

 * 左右两个摇杆一样，**不触摸时隐藏**。
 * 触摸左半屏幕左摇杆出现，摇杆出现在手指触摸的位置，右同理，**两边同时触摸时，两个摇杆同时出现**。
 * 某个手指离开屏幕后，那个手指所在的**摇杆消失**。
 * 预留摇杆**触发事件**接口。
 * 完成后上交源码（不限C++,Lua,Js）和可安装APK文件。
 * 每个摇杆的效果如下图，小圆不得超出大圆外，资源图片随意。
 ![](http://bosseveryday.qiniudn.com/www.yxkfw.com-8375.gif)
