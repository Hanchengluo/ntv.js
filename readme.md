# ntv.js
原始框架地址：[点击](https://git.oschina.net/ntv/ntv.js)
ntv.js 博客地址  [点击](https://my.oschina.net/cotonchen/home)


#### 一、源代码目录结构


- css       		    // 包含一些标签默认样式重置、常用class、组件所需的css样式        
- images               // 包含了2张透明图，具体用处后续介绍（可选目录）        
- js                        // 框架核心代码       
   - js/effect       // 框架提供的效果插件，例如滚动div、滑动菜单

#### 二、js文件结构


- 1common.js 

     公共函数类。例如：将document.getElementById(id)封装为 $("#id")函数, $.ajax()等函数。

- 2core.js 

     核心类。包括调试模式、机顶盒平台信息检测。

- 3key.js 
   机顶盒键值处理类。键值的定义、键值触发和系统消息事件的代理函数类和键值控制的  对外接口。

- 4navigation.js
   机顶盒焦点控制类。页面的焦点控制，例如上下左右的焦点移动、焦点边界检测和焦点控制接口。

- 5page.js
  页面的处理类。页面的载入、离开、打开新页面、刷新页面及页面URL的一些处理类。

- 6ngb_h.js
   NGB-H规范接口类。含所有NGB-H规范的接口调用。

- 6ipanel.js 
   iPanel私有规范接口类。含所有iPanel规范的接口调用。

- 6shdv.js 
   SHDV私有规范接口类。含所有SHDV规范的接口调用。

- 6pc.js 
   PC平台模拟接口类。PC平台上的浏览器模拟机顶盒的接口调用（PC调试所用）。

- 7msg.js 
   消息定义类。将接口返回的错误码（CODE）转为可读信息的定义。

- 8stb.js 
   机顶盒的统一接口类。对ipanel.js、shdv.js、ngb_h.js接口的封装，提供统一对外的接口。

- 9util.js 
   常用的工具函数类。例如：字符串的处理、机顶盒相关的字符处理。

- ***10ocn_media_player.js***

   东方有线流媒体播放

- win_js_release.bat 
   win32平台下合并js的批处理，用来将所有js合并为一个ntv.js文件。

- effect
  - effect-scrolldiv.js 

  ​     滚动div插件。用于文章过长时使用上下键阅读内容详细。

  - effect-slidemenu.js 

  ​    滑动菜单插件。横向多图标的滚动插件。
