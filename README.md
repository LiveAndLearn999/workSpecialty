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
#### css动画插件
  *  https://www.cnblogs.com/sunny0120/p/6669688.html
  * 2018 15个css/javascript库 推荐 https://baijiahao.baidu.com/s?id=1595516973359211872&wfr=spider&for=pc

##  css-Preprocessor
####   Sass
####   Less
####   Stylus

##  JS
####   javascript
1. 菜鸟教程 http://www.runoob.com/js/js-tutorial.html
2. HTML CSS JAVASCRIPT三者之间的关系
 * HTML 定义了网页的内容
 * CSS  描述了网页的布局
 * JAVASCRIPT 网页的行为
3. javascript组成部分
  * ECMAScript
  * DOM
  * BOM
4. 字面量的定义---------（变量是一个名称。字面量是一个值。）
  * 在编程语言中，一般固定值称为字面量
    1. 数字（Number）字面量 可以是整数或者是小数，或者是科学计数(e)。 如：3.14  1001 123e5 
    2. 字符串（String）字面量 可以使用单引号或双引号:    如; "John Doe"
    3. 表达式字面量 用于计算：              如：5 + 6  5*6
    4. 数组（Array）字面量 定义一个数组：   如：[40, 100, 1, 5, 25, 10] 
    5. 对象（Object）字面量 定义一个对象：  如：{firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"} 
    6. 函数（Function）字面量 定义一个函数：如：function myFunction(a, b) { return a * b;} 
  * 变量是一个名称。字面量是一个值。
5. 判断该对象是否为数组
  * 使用 isArray 方法 if (Array.isArray) {if(Array.isArray(cars)) {document.write("该对象是一个数组。") ;}}、
  * 使用 instanceof 操作符 if (cars instanceof Array) {document.write("该对象是一个数组。") ;}
6.  undefined 和 null 都是小写，并且。
  * var x,y;if(x == null){document.write(x);}          //undefined
  * if(y == undefined){document.write(y);}             //undefined
7. javascript 作用域
  * 作用域为可访问变量，对象，函数的集合（JavaScript 函数作用域: 作用域在函数内修改。）
8. javascript变量生命周期
  * JavaScript 变量生命周期在它声明时初始化
  * 局部变量在函数执行完毕后销毁
  * 全局变量在页面关闭后销毁
9. javascript 字符串对象
  * 菜鸟 http://www.runoob.com/jsref/jsref-obj-string.html
10. javascript 执行上下文
  https://juejin.im/post/5af9933bf265da0ba063490e
  https://www.jianshu.com/p/8f19e45fd1f1
  * 执行环境
    * 执行环境的分类
      * 1.全局执行环境
        * 是JS代码开始运行时的默认环境（浏览器中为window对象）。全局执行环境的变量，对象始终都是作用域链中的最后一个对象
      * 2.函数执行环境
        * 当某个函数被调用时，会先创建一个执行环境及相应的作用域链。然后使用arguments和其他命名参数的值来初始化执行环境的变量对象。
      * 3.使用eval()执行代码
    * 执行上下文（执行环境）的组成
      * 执行环境（execution context，EC）或称之为执行上下文，是JS中一个极为重要的概念。当JavaScript代码执行时，会进入不同的执行上下文，而每个执行上下文的组成
        * 变量对象（Variable object，VO）: 变量对象，即包含变量的对象，除了我们无法访问它外，和普通对象没什么区别
        * [Scope]]属性:数组。作用域链是一个由变量对象组成的带头结点的单向链表，其主要作用就是用来进行变量查找。而[[Scope]]属性是一个指向这个链表头节点的指针。
        * this: 指向一个环境对象，注意是一个对象，而且是一个普通对象，而不是一个执行环境。
    * 执行上下文栈
      * 若干执行上下文会构成一个执行上下文栈（Execution context stack，ECS） 
    * 产生执行上下文的两个阶段
      * 创建阶段 （当函数被调用，但是开始执行函数内部代码之前）
        * 创建变量对象VO
        * 设置[[Scope]]属性的值
        * 设置this的值
        * 激活/代码执行阶段
      * 初始化变量对象，即设置变量的值、函数的引用，然后解释/执行代码。
    * 创建变量对象VO过程
      * 1.根据函数的参数，创建并初始化arguments object
      * 2.扫描函数内部代码，查找函数声明（function declaration）
        * 对于所有找到的函数声明，将函数名和函数引用存入VO中
        * 如果VO中已经有同名函数，那么就进行覆盖
      * 3.扫描函数内部代码，查找变量声明（Variable declaration）
        * 对于所有找到的变量声明(通过var声明)，将变量名存入VO中，并初始化为undefined
        * 如果变量名跟已经声明的形参或函数相同，则什么也不做
        * 注：步骤2和3也称为声明提升（declaration hoisting）
11. javascript 预解析
  * JavaScript 中，函数及变量的声明都将被提升到函数的最顶部。 
  * 遇到 script 标签的话 js 就进行预解析，将变量 var 和 function 声明提升，但不会执行 function，然后就进入上下文执行，上下文执行还是执行预解析同样操作，直到没有 var 和 function，就开始执行上下文。需要注意都是函数声明提升直接把整个函数提到执行环境的最顶端。
  * 使用匿名函数的方式不存在函数提升，因为函数名称使用变量表示的，只存在变量提升 var getName=function(){console.log(2);}  function getName(){console.log(1);} getName();//结果为2
12. JavaScript中浮点数的运算
  * 所有的编程语言，包括 JavaScript，对浮点型数据的精确度都很难确定：
  * JavaScript 中的所有数据都是以 64 位浮点型数据(float) 来存储。
  * 为解决以上问题，可以用整数的乘除法来解决：var z = (x * 10 + y * 10) / 10;
13. javascript:void(0) 含义 
  * javascript:void(0) 中最关键的是 void 关键字， void 是 JavaScript 中非常重要的关键字，该操作符指定要计算一个表达式但是不返回值。 
14. 闭包
  * 闭包是可访问上一层函数作用域里变量的函数，即便上一层函数已经关闭




####   ES6
 1. react react-native es6 https://github.com/reactnativecn/react-native-guide

####   ES7
####   JSX
####   TYPESCRIPT
##  JS-library
####   jquery
####   Prototype
####   zepto
####   常用JS库整理 https://www.jianshu.com/p/dccad48bed89 11个实用的JavaScript库 https://blog.csdn.net/moyouyou123/article/details/80797684 JS常用库收集 http://www.cnblogs.com/Aaxuan/p/9424430.html

#### layui https://www.layui.com/doc/modules/layer.html

#### bootstrap

##  JS-frame 
####   vue
    1. https://cn.vuejs.org/v2/guide/
    2. vue响应式原理
      * 当你把一个普通的 JavaScript 对象传给 Vue 实例的 data 选项，Vue 将遍历此对象所有的属性，并使用 Object.defineProperty 把这些属性全部转为 getter/setter。Object.defineProperty 是 ES5 中一个无法 shim 的特性，这也就是为什么 Vue 不支持 IE8 以及更低版本浏览器。
      * 这些 getter/setter 对用户来说是不可见的，但是在内部它们让 Vue 追踪依赖，在属性被访问和修改时通知变化。这里需要注意的问题是浏览器控制台在打印数据对象时 getter/setter 的格式化并不同，所以你可能需要安装 vue-devtools 来获取更加友好的检查接口。
      * 每个组件实例都有相应的 watcher 实例对象，它会在组件渲染的过程中把属性记录为依赖，之后当依赖项的 setter 被调用时，会通知 watcher 重新计算，从而致使它关联的组件得以更新。
      * 每个组件实例都有相应的 watcher 实例对象，它会在组件渲染的过程中把属性记录为依赖，之后当依赖项的 setter 被调用时，会通知 watcher 重新计算，从而致使它关联的组件得以更新。
      *  检测变化的注意事项
        *  受现代 JavaScript 的限制 (而且 Object.observe 也已经被废弃)，Vue 不能检测到对象属性的添加或删除。由于 Vue 会在初始化实例时对属性执行 getter/setter 转化过程，所以属性必须在 data 对象上存在才能让 Vue 转换它，这样才能让它是响应的。
        *  Vue 不允许在已经创建的实例上动态添加新的根级响应式属性 (root-level reactive property)。然而它可以使用 Vue.set(object, key, value) 方法将响应属性添加到嵌套的对象上：
      *  异步更新队列
        * 可能你还没有注意到，Vue 异步执行 DOM 更新 只要观察到数据变化，Vue 将开启一个队列，并缓冲在同一事件循环中发生的所有数据改变。
        如果同一个 watcher 被多次触发，只会被推入到队列中一次。这种在缓冲时去除重复数据对于避免不必要的计算 和 DOM 操作上非常重要。
        然后，在下一个的事件循环“tick”中，Vue 刷新队列并执行实际 (已去重的) 工作。Vue 在内部尝试对异步队列使用原生的 Promise.then 和 
        MessageChannel，如果执行环境不支持，会采用 setTimeout(fn, 0) 代替。

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

## 协议相关
#### 四层模型
  https://zhuanlan.zhihu.com/p/53409989
  1. 数据从网络中一个终端上的应用程序传送到另外一个终端的应用程序，中间需要经历很多过程，有多方参与对数据进行层层封装、转发。我们把这个流程在逻辑上进行分成层，每一层根据本层的规章制度(协议)各司其职。TCP/IP协议族可以分为四层：应用层、传输层、网络层、数据链路层。
  2. 为了权责分明，我们对上面的几种角色的职能起草几个规范文档：皇室成员写信规范、通政司业务流程规范、驿站工作流程规范、信使职能规范。其实皇室成员代表计算机上的各种应用，不同的皇室成员写信使用不同的规矩和规范。与之对应的是不同的应用使用不同的应用层协议，如HTTP协议、FTP协议、POP3协议等。通政司代表传输层协议的实现，通政司的规矩规范代表传输层协议，如TCP、UDP等。驿站的职能规范代表网络层协议，如IP协议。信使等职能规范代表数据链路层协议，如以太网协议。
  3. 这里的协议，我们可以理解为规范、规矩、规则、约定。比如作为学生想发表论文必须遵守论文的规范（包含摘要、背景、实现、文献），否则老师不认可。 想发表专利必须遵守专利的书写规范，否则专利局不收。协议不是一个软件，不要把HTTP当成一个软件或者一段程序代码。
  4. 这里面的层，我们可以理解为管理层，每个管理层有自己的职能。围绕当前职能会起草多个规章协议（比如通政司会有针对皇室信件安全但繁复的书信投送流程，也有针对皇宫普通宫女的简单书信投送流程）。这些规章协议会有对应的实施者贯彻实施。每一层只需关心自己职能范围的事即可，不用操心其它层级能否完成任务以及具体如何实施。
  5. 应用层协议
      * 与网络相关的程序通过网络与其他程序通信使用的数据格式规范。比如浏览器向服务器发请求获取网页数据，此时发送的请求报文（皇室信件）就需要遵循HTTP协议（按HTTP协议的要求填写字段）。常见的应用层协议有：
      * 1.HTTP（80端口），主要用于普通浏览。
      * 2.HTTPS（443端口），HTTP协议的安全版本。
      * 3.FTP（20和21端口），用于文件传输。
      * 4.POP3（110端口），收邮件用。
      * 5.SMTP（25端口），用来发送电子邮件。
      * 5.SSH（22端口），用于加密安全登陆用。
      * 6.DHCP（67端口，动态主机配置协议），动态配置IP地址。
      * 7.DNS，用于完成地址查找，邮件转发等工作（运行在TCP和UDP协议上）。
      * 8.SNMP，用于网络信息的收集和网络管理。
      * 9.ARP，用于动态解析以太网硬件的地址。
  6. 传输层协议
      * 解决诸如端到端可靠性（数据是否已经到达目的地）和保证数据按照正确的顺序到达这样的问题。TCP、UDP都是传输层协议
  7. 网络层协议
      * 解决在一个单一网络上传输数据包的问题。IP协议是网络层协议。
  8. 数据链路层协议
      * 它是数据包从一个设备的网络层传输到另外一个设备的网络层遵循的规范。比如以太网协议、Wi-Fi协议。
      
## 深入JavaScript

https://juejin.im/post/5965943ff265da6c30653879
#### javascript正则
  1. 正则表达式是匹配模式，要么匹配字符，要么匹配位置
  2. 两种模糊匹配
  
    *  横向模糊匹配
      *  横向模糊指的是，一个正则可匹配的字符串的长度不是固定的，可以是多种情况的。
      *  其实现的方式是使用量词。譬如{m,n}，表示连续出现最少m次，最多n次
    *  纵向模糊匹配
      *  纵向模糊指的是，一个正则匹配的字符串，具体到某一位字符时，它可以不是某个确定的字符，可以有多种可能
      *  其实现的方式是使用字符组。譬如[abc]，表示该字符是可以字符“a”、“b”、“c”中的任何一个。
  3. 字符组
  
    * 需要强调的是，虽叫字符组（字符类），但只是其中一个字符。例如[abc]，表示匹配一个字符，它可以是“a”、“b”、“c”之一。
    * 如果字符组里的字符特别多的话，怎么办？可以使用范围表示法。
      *  比如[123456abcdefGHIJKLM]，可以写成[1-6a-fG-M]。用连字符-来省略和简写。
      *  因为连字符有特殊用途，那么要匹配“a”、“-”、“z”这三者中任意一个字符，该怎么做呢？不能写成[a-z]，因为其表示小写字符中的任何一个字符。可以写成如下的方式：[-az]或[az-]或[a\-z]
    *  纵向模糊匹配，还有一种情形就是，某位字符可以是任何东西，但就不能是"a"、"b"、"c"。
      *  此时就是排除字符组（反义字符组）的概念。例如[^abc]，表示是一个除"a"、"b"、"c"之外的任意一个字符。字符组的第一位放^（脱字符），表示求反的概念。
    *  常见的简写形式
      *  \d就是[0-9]。表示是一位数字。记忆方式：其英文是digit（数字）。
      *  \D就是[^0-9]。表示除数字外的任意字符。
      *  \w就是[0-9a-zA-Z_]。表示数字、大小写字母和下划线。记忆方式：w是word的简写，也称单词字符。
      *  \W是[^0-9a-zA-Z_]。非单词字符。
      *  \s是[ \t\v\n\r\f]。表示空白符，包括空格、水平制表符、垂直制表符、换行符、回车符、换页符。记忆方式：s是space character的首字母。
      *  \S是[^ \t\v\n\r\f]。 非空白符。
      *  .就是[^\n\r\u2028\u2029]。通配符，表示几乎任意字符。换行符、回车符、行分隔符和段分隔符除外。记忆方式：想想省略号...中的每个点，都可以理解成占位符，表示任何类似的东西。
 4. 简写形式
      *  {m,} 表示至少出现m次。
      *  等价于{m,m}，表示出现m次。
      *  ? 等价于{0,1}，表示出现或者不出现。记忆方式：问号的意思表示，有吗？
      *  + 等价于{1,}，表示出现至少一次。记忆方式：加号是追加的意思，得先有一个，然后才考虑追加。
      *  * 等价于{0,}，表示出现任意次，有可能不出现。记忆方式：看看天上的星星，可能一颗没有，可能零散有几颗，可能数也数不过来。
   *  贪婪匹配和惰性匹配
      *  其中正则/\d{2,5}/，表示数字连续出现2到5次。会匹配2位、3位、4位、5位连续数字。
      *  其中/\d{2,5}?/表示，虽然2到5次都行，当2个就够的时候，就不在往下尝试了。
      *  通过在量词后面加个问号就能实现惰性匹配，因此所有惰性匹配情形如下：  {m,n}?  {m,}?  ??  +? *?
 5. 多选分支
      *  一个模式可以实现横向和纵向模糊匹配。而多选分支可以支持多个子模式任选其一
      *  具体形式如下：(p1|p2|p3)，其中p1、p2和p3是子模式，用|（管道符）分隔，表示其中任何之一。
      
  6.  正则表达式位置匹配攻略
   * 位置
       *  位置是相邻字符之间的位置
   * 匹配位置
       *  在ES5中，共有6个锚字符：  ^ $ \b \B (?=p) (?!p)
       *  ^（脱字符）匹配开头，在多行匹配中匹配行开头。
       *  $（美元符号）匹配结尾，在多行匹配中匹配行结尾。
       *  比如我们把字符串的开头和结尾用"#"替换（位置可以替换成字符的！） var result = "hello".replace(/^|$/g, '#');console.log(result); // => "#hello#"
       *  多行匹配模式时，二者是行的概念，这个需要我们的注意： var result = "I\nlove\njavascript".replace(/^|$/gm, '#');console.log(result);/*#I# #love# #javascript# */
       *  \b是单词边界，具体就是\w和\W之间的位置，也包括\w和^之间的位置，也包括\w和$之间的位置。var result = "[JS] Lesson_01.mp4".replace(\b/g, '#');console.log(result); // => "[#JS#] #Lesson_01#.#mp4#"
       *  \B就是\b的反面的意思，非单词边界。例如在字符串中所有位置中，扣掉\b，剩下的都是\B的。具体说来就是\w与\w、\W与\W、^与\W，\W与$之间的位置。
       *  (?=p)，其中p是一个子模式，即p前面的位置。var result = "hello".replace(/(?=l)/g, '#');console.log(result); // => "he#l#lo"
       *  (?!p)就是(?=p)的反面意思，var result = "hello".replace(/(?!l)/g, '#');console.log(result); // => "#h#ell#o#"
   * 位置的特性
       *  于位置的理解，我们可以理解成空字符""。  比如"hello"字符串等价于如下的形式： "hello" == "" + "h" + "" + "e" + "" + "l" + "" + "l" + "o" + ""; 也等价于： "hello" == "" + "" + "hello"
       *  因此，把/^hello$/写成/^^hello$$$/，是没有任何问题的：
       *  字符之间的位置，可以写成多个    （把位置理解空字符，是对位置非常有效的理解方式。）








      
  
  https://www.zhihu.com/question/22855484/answer/22875761
#### javascript命名空间
  1. 命名空间namespace（某些语言中叫package），是一个在静态语言中常见的概念。它可以帮助我们更好地整理代码，并可避免命名冲突https://www.jianshu.com/p/554454d951d9
  2. 核心知识点 https://www.cnblogs.com/digdeep/p/4175969.html
     *  利用了 window 这个特殊引用的不可覆盖性，不可修改；
     *  命名空间其实是对象链条来模拟的
     *  理解引用的含义：引用是个在stack上的变量，可以修改它指向不同的对象，要访问或者说修改他指向的对象，必须使用 “.” 点操作符，比如 o.index ={}; 而单纯的修改 o ，比如 o = {}; 并不会修改他指向的对象，因为 没有访问到他指向的对象，怎么能修改到他指向的对象呢？
#### javascript变量污染
    https://blog.csdn.net/qq_39480597/article/details/79655997
    1. 变量污染  变量被后定义的覆盖了
    2. javaScript 可以随意定义保存所有应用资源的全局变量。但全局变量可以削弱程序灵活性，增大了模块之间的耦合性。在多人协作时，如果定义过多的全局变量 有可能造成全局变量冲突，也就是全局变量污染问题,以下是两种解决办法
      * 定义全局变量命名空间   只创建一个全局变量，并定义该变量为当前应用容器，把其他全局变量追加在该命名空间下
      * 利用匿名函数将脚本包裹起来
 #### JavaScript变量提升和函数声明提升
 https://www.cnblogs.com/Gary-Guoweihan/p/6251870.html
    1. Js代码分为两个阶段：编译阶段和执行阶段
      * Js代码的编译阶段会找到所有的声明，并用合适的作用域将它们关联起来，这是词法作用域的核心内容包括变量声明(var a)和函数声明(function a(){})在内的所有声明都会在代码被执行前的编译阶段首先被处理
      * 过程就好像变量声明和函数声明从他们代码中出现的位置被移动到执行环境的顶部，这个过程就叫做提升只有声明操作会被提升，赋值和逻辑操作会被留在原地等待执行
      * 变量声明
        * Js编译器会把变量声明看成两个部分分别是声明操作(var a)和赋值操作(a=2)
        * 声明操作在编译阶段进行，声明操作会被提升到执行环境的顶部，值是undefined(表示未初始化) 赋值操作会被留在原地等待执行阶段
      * 函数声明
        * 定义函数有两种方式：函数声明和函数表达式
        * 函数声明提升会在编译阶段把声明和函数体整体都提前到执行环境顶部，所以我们可以在函数声明之前调用这个函数
        * 函数表达式，其实就是变量声明的一种，声明操作会被提升到执行环境顶部，并赋值undefined。赋值操作被留在原地等到执行。
      * 控制语句
        * Js中使用函数级作用域，不存在块级作用域。所有普通块中的声明都会被提升到顶部，所以控制语句对声明的控制就显得完全没有效果
      * 函数优先
        * 提升操作会优先进行函数的声明
        * 函数会首先被提升然后才是变量，重复的变量声明会被忽略，只剩下赋值操作，多个函数声明可以进行覆盖声明的顺序是这样的：
          * 1.找到所有的函数声明，初始化函数体，如有同名的函数则会进行覆盖
          2 2.查找变量声明，初始化为undefined，如果已经存在同名的变量，就什么也不做直接略过
    

## ServerSide
#### node
#### php 
#### python
#### java



