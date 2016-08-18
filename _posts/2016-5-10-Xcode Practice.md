---
layout: post
title: Xcode Practice
author: wood
categories: design
---
因为受[@MengTo](https://twitter.com/mengto)的[design+code](http://sumoing.com/) 的影响，埋了个用Xcode 做demo 和animation的坑（就是学了一半很难受）。MengTo的教程还是比较偏设计啦，Code 的部分经常看着看着就不知所以了，又逢跟客户端技术沟通频繁，沟通过程中学到一些基础知识但是觉得不够用，所以干脆学习了一下简单的swift 语法，跟着Appcoda的[Beginning iOS 9 Programming
with Swift](https://www.appcoda.com/swift/)系列书学习了一下（后面也看了下赠送的intermediate iOS9 reference），语法基本上就是空闲时间看也不记得花了多少时间，demo 练习前后差不多两个月的时间（中间夹杂着去了趟云南什么的），学得有点小激动，记录一下☺️。

1 一开始就是挺长的一个demo，包括滑动，详情页，评价，定位… 因为之前没有想到要记录这回事儿，这时候已经学了些零零碎碎的逻辑，可以运行起来了！画了个图标运行在手机里还是相当鸡冻的呢。
<video width="300" muted controls> <source src="/assets/2016-5-10-FoodPinDemo_3.2.mov" type="video/mp4"> </video><br/>


2 这时候学会增加了选择评价的时候记住结果的功能，还有左滑分享和删除，以及添加。
<video width="300" muted controls> <source src="/assets/2016-5-10-FoodPinDemo_3.7.mov" type="video/mp4"> </video>
<br/>


3 添加数据的一些细节的逻辑，比如空缺提醒和是否到达过的判断。

<video width="300" muted controls> <source src="/assets/2016-5-10-FoodPinDemo_3.3_2.mov" type="video/mp4"> </video>

<br/>

4 这个时候开始往database 里面添加内容，以及搜索，同时对名称、类型和地点的匹配

<video width="300" muted controls> <source src="/assets/2016-5-10-FoodPinDemo_3.7_search.mov" type="video/mp4"> </video>
<br/>


5 Walkthrough嘛，原来直接有控件来解决这个功能~ 
<video width="300" muted controls> <source src="/assets/2016-5-10-FoodPinDemo_3.7_walkthrough.mov" type="video/mp4"> </video>

6添加了Tabbar，看起来像一个真的应用了特别鸡冻again~

<video width="300" muted controls> <source src="/assets/2016-5-10-FoodPinDemo_3.16_Tabbar.mov" type="video/mp4"> </video>

<br/>

7 web页面的3种打开方式：Mobile Safari/UIWebView/SFSafariViewController.
<video width="300" muted controls> <source src="/assets/2016-5-10-FoodPinDemo_3.22_About.mov" type="video/mp4"> </video>
<br/>


8 在网络状况不好的时候的异步加载和缓存的处理 
<video width="300" muted controls> <source src="/assets/2016-5-10-FoodPinDemo_4.10_Discover.mov" type="video/mp4"> </video>
<br/>


9 浮夸的timeline 动画


<video width="300" muted controls> <source src="/assets/2016-5-10-animation_4.11.mov" type="video/mp4"> </video> <br/>

<video width="300" muted controls> <source src="/assets/2016-5-10-animation_4.11_2.mp4" type="video/mp4"> </video>
<br/>

10 上滑菜单栏，原来菜单出现的时候下面的屏幕是截图，涨知识
<video width="300" muted controls> <source src="/assets/2016-5-10-SlideMenu_4.23.mov" type="video/mp4"> </video>
<br/>


11 Carousel样式的卡片demo，挺喜欢这类效果
<video width="300" muted controls> <source src="/assets/2016-5-10-TripCardDemo_4.24.mov" type="video/mp4"> </video>
<br/>


12 因为用CoreData各种报错，于是去appcoda论坛里面问大神，大神说不要用那鬼东西，用realm啊，一脸懵逼地去研究了下好像真的很厉害！于是用realm 练习了下存储，不过这个时候已经离我的学习初衷有点远了…但是有趣啊尝试一下也无妨；
<video width="300" muted controls> <source src="/assets/2016-5-10-RealmDemo_5.4.mov" type="video/mp4"> </video>
<br/>


14 然后开始学习 Json的使用方式，打算拿自己的Pinterest 某个画板作为数据源，优化一下界面设计再来上这个demo，至此Xcode 的学习告一段落。<br/>


----
整体感受是：**首先**，弄清楚某些平常技术GG们念叨来念叨去然而并不是很明白的术语是很开心的，比如他们说什么哈希值也能至少知道是什么领域的事儿了，并且万能的Stack Overflow 用的溜溜的，不会可以查啊！**其二**，用Mengto的 Spring 插件做动画效果和用Xcode 直接写的感觉不太一样，不过学过之后再回去用插件感觉能明白一些原理就爽多啦；**其三**，不用会马上忘哎，整理的时候距离学的时候已经过去一段时间了，现在能记得一些原理，但是再做感觉还是要重新熟悉过，所以遇到技术GG们说这个东西我要撸一遍代码还是需要给足时间啊~ ；**最后**，如果不是真的时间特别有余要求特别高，其实很多工具和方式可以替代用代码直接编写，还是更多花时间在前期的调研和产品功能结构的思考上更重要。
