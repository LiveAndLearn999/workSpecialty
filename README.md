# WORK-SPECIALTY
## 最近几年前端发展趋势
1. 从框架层面开始：backbone -> angular -> react
2. 工具生态：grunt -> gulp -> webpack
3. 语言：JavaScript 1.3 -> ECMA 5 -> ECMA 2015，CSS2.1 -> CSS3.0，XHTML -> HTML4.0 -> HTML5.0
4. Firefox OS （虽然它挂了）
5. 桌面应用：NW.js -> Electron
6. 出现了Node.js和Mongodb
7. 服务端框架：Express -> koa
8. 移动应用：PhoneGap -> Cordova | ionic -> React Native | weex
9. 语法检查：jslint -> eslint
10. 模块化：AMD | CMD -> Commonjs -> import export
11. 语法增强：CoffeeScript -> Dart -> TypeScrip

##  html
1. 菜鸟教程：http://www.runoob.com/（HTML事件：http://www.runoob.com/tags/ref-eventattributes.html）
##  css
1. 菜鸟教程：http://www.runoob.com/ (伪类：http://www.runoob.com/css/css-pseudo-classes.html 伪元素 http://www.runoob.com/css/css-pseudo-elements.html)
* 1 伪类PK伪元素
  1. 伪类选择元素基于的是当前元素处于的状态，或者说元素当前所具有的特性，而不是元素的id、class、属性等静态的标志。由于状态是动态变化的，所以一个元素达到一个特定状态时，它可能得到一个伪类的样式；当状态改变时，它又会失去这个样式。由此可以看出，它的功能和class有些类似，但它是基于文档之外的抽象，所以叫伪类。
  2. 与伪类针对特殊状态的元素不同的是，伪元素是对元素中的特定内容进行操作，它所操作的层次比伪类更深了一层，也因此它的动态性比伪类要低得多。实际上，设计伪元素的目的就是去选取诸如元素内容第一个字（母）、第一行，选取某些内容前面或后面这种普通的选择器无法完成的工作。它控制的内容实际上和元素是相同的，但是它本身只是基于元素的抽象，并不存在于文档中，所以叫伪元素。
* 2 CSS 属性选择器 *=, |=, ^=, $=, *= 的区别  
  1. attribute 属性中包含 value:　
      [attribute~=value] 属性中包含独立的单词为 value，例如：
      [title~=flower]  -->  /*<img src="/i/eg_tulip.jpg" title="tulip flower" />*/
      [attribute*=value] 属性中做字符串拆分，只要能拆出来 value 这个词就行，例如：
      [title~=flower]   -->  /*<img src="/i/eg_tulip.jpg" title="ffffflowerrrrrr" />*/
  2. .attribute 属性以 value 开头:
      [attribute|=value] 属性中必须是完整且唯一的单词，或者以 - 分隔开：，例如：
      [lang|=en]     -->  /*<p lang="en">  <p lang="en-us">*/
  3. attribute 属性以 value 结尾:
      [attribute$=value] 属性的后几个字母是 value 就可以，例如：
      a[src$=".pdf"]
* css 弹性盒子属性
  1. display             指定 HTML 元素盒子类型。
  2. flex-direction      指定了弹性容器中子元素的排列方式
  3. justify-content     设置弹性盒子元素在主轴（横轴）方向上的对齐方式。
  4. align-items         设置弹性盒子元素在侧轴（纵轴）方向上的对齐方式。
  5. flex-wrap           设置弹性盒子的子元素超出父容器时是否换行。
  6. align-content       修改 flex-wrap 属性的行为，类似 align-items, 但不是设置子元素对齐，而是设置行对齐
  7. flex-flow           flex-direction 和 flex-wrap 的简写
  8. order               设置弹性盒子的子元素排列顺序。
  9. align-self          在弹性子元素上使用。覆盖容器的 align-items 属性。
  10. flex               设置弹性盒子的子元素如何分配空间。
    
##  css-library
####   30个免费css库（http://www.html580.com/6412）
##  css-Preprocessor
####   Sass
####   Less
####   Stylus
##  JS
####   javascript
####   ES6
##  S-library
####   jquery
####   Prototype
####   zepto
####   常用JS库整理 https://www.jianshu.com/p/dccad48bed89 11个实用的JavaScript库 https://blog.csdn.net/moyouyou123/article/details/80797684 JS常用库收集 http://www.cnblogs.com/Aaxuan/p/9424430.html
##  JS-frame 
####   vue
####   react
####   angular
## Hybrid App
####   PhoneGap / Cordova（https://www.cnblogs.com/oc-bowen/p/6742511.html）
####   IONIC 
####   WeX5
####   APICloud
####   Appcelerator
####   NativeScript
####   Kinvey
####   ExMobi （https://blog.csdn.net/dj0379/article/details/50518486）
##  web-native
####   react-native
####   Weex
####   Flutter
##  web-automation
####   webpack
####   gulp
####   Grunt （https://blog.csdn.net/qq_42606051/article/details/81041825）


