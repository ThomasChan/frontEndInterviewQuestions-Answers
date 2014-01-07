[front-end-developer-interview-questions](https://github.com/markyun/Front-end-Developer-Interview-Questions/tree/master/Chinese#%E6%9C%80%E5%88%9D%E7%9A%84%E8%B4%A1%E7%8C%AE%E8%80%85) /  my answers
==================================

一般问题
=======
--------------------------------------------
1. 你用Twitter吗？ （在天朝最好问你用微博吗？）  
**回答：用**
- 如果用，你都关注那些人？  

2. 你用Github吗？  
**回答：用**  
- 如果用，你关注的项目有什么？  
**关注的项目：**  
     - **facebook/tornado**  
     - **frontend-dev-bookmarks**

3. 你关注的博客有那些？  
- [编程随想的博客](http://program-think.blogspot.com/)
- [前端开发](http://www.css88.com/)
- [W3CPlus](http://www.w3cplus.com/)
- [CSS-Tricks](http://css-tricks.com/)
- [我喜欢CSS](http://ilikecss.com/blog/)
- [The CSS Ninja](http://www.thecssninja.com/)
- [Cat in Chinese](http://chinese.catchen.me/)
- [伯乐在线](http://blog.jobbole.com/)
- [Mozilla Hacks](http://hacks.mozilla.org/)
- [Javascript is Sexy](http://javascriptissexy.com/)
- [粉丝日志](http://blog.fens.me/#gsc.tab=0)
- [Flippin' Awesome](http://flippinawesome.org/)
- [进出自由，我的分享](http://zouyesheng.com/)
- [Impressive Webs](http://www.impressivewebs.com/)

4. 你使用那些版本管理系统，比如Git，SVN等？  
**回答： git**

5. 你常用的开发环境是怎样的？比如操作系统，文本编辑器，浏览器，及其他工具等。  
 - **操作系统：WIN 7 64BIT**
 - **文本编辑器：sublime text 3**
 - **浏览器：Chrome,firefox,opera next,safari,ie10**

6. 你能描述一下你制作一个网页的工作流程吗？  
 - **一般情况下：**
     - **考虑网页结构>  
		 写HTML>  
	     写CSS>  
	     调试>  
 	     写javascript>  
	     合并CSS，压缩js**  
 - **使用框架比如angular时：**
     - **考虑网页结构>  
	     考虑可能用到的server，factory，controller并创建文件>  
	     写HTML模板并进行数据绑定>  
	     写CSS并调试>  
	     把需要进行DOM操作的部分写成directive>  
	     进行单元测试>  
	     合并CSS，压缩js**

7. 你能描述一下渐进增强和优雅降级之间的不同吗?  
- 如果提到了特性检测，可以加分。  
**回答：**
		- **渐进增强是向上‘兼容’，一开始只构建站点或产品的最核心特性功能，然后不断针对各浏览器追加功能和优化。**
		- **优雅降级是向下兼容，一开始就构建站点或产品的完整功能，然后针对各浏览器进行优化。**


9. 请解释一下什么是语义化的HTML。  
**回答：**
**语义化的HTML是为了能让人和机器更好的读懂文档。**

10. 你更喜欢在哪个浏览器下进行开发？你使用那些开发人员工具？  
**回答：**
**在Chrome下，chrome的开发者工具**

11. 你如何对网站的文件和资源进行优化？

- 期待的解决方案包括：

	 1.文件合并  
	 2.文件最小化/文件压缩  
	 3.使用CDN托管  
	 4.缓存的使用  
	 5.其他

12. 为什么利用多个域名来存储网站资源会更有效？  
**回答：**  
	- **CDN缓存更方便**
	- **突破浏览器并发限制**
	- **节约cookie带宽**
	- **节约主域名的连接数，优化页面响应速度**
	- **防止不必要的安全问题**

13. 浏览器一次可以从一个域名下做多少资源？  
**回答：**  
	- **(08年的统计)  
	<PRE>Browser					HTTP/1.1	HTTP/1.0
		IE 6,7						2			4
		IE 8						6			6
		Firefox 2					2			8
		Firefox 3					6			6
		Safari 3,4					4			4
		Chrome 1,2					6			?
		Chrome 3					4			4
		Chrome 4+					6			?
		iPhone 2					4			?
		iPhone 3					6			?
		iPhone 4					4			?
		Opera 9.63,10.00alpha		4			4
		Opera 10.51+				8			?</PRE>**
	- **参考链接  
		[roundup-on-parallel-connections](http://www.stevesouders.com/blog/2008/03/20/roundup-on-parallel-connections/)  
		[浏览器允许的并发请求资源数是什么意思？](http://www.zhihu.com/question/20474326)**

14. 请说出三种减低页面加载时间的方法。（加载时间指感知的时间或者实际加载时间）  
**回答：（参考第10个问题）**  
	1. **从2-4个域名提供资源服务增加浏览器并行下载数量（参考上一问）**
	2. **CSS Sprite**
	3. **代码压缩**

15. 如果你接到了一个使用Tab来缩进代码的项目，但是你喜欢空格，你会怎么做？

- 建议这个项目使用像EditorConfig(http://editorconfig.org)之类的规范
为了保持一致性，转换成项目原有的风格
直接使用VIM的retab命令

16. 请写一个简单的幻灯效果页面

- 如果不使用JS来完成，可以加分。  
**无JS超简洁版：** 
	**<pre>
			/**HTML**/
			div.ani
			/**css**/
			.ani{
			  width:480px;
			  height:320px;
			  margin:50px auto;
			  overflow: hidden;
			  box-shadow:0 0 5px rgba(0,0,0,1);
			  background-size: cover;
			  background-position: center;
			  -webkit-animation-name: "loops";
			  -webkit-animation-duration: 20s;
			  -webkit-animation-iteration-count: infinite;
			}
			@-webkit-keyframes "loops" {
				0% {
					background:url(http://d.hiphotos.baidu.com/image/w%3D400/sign=c01e6adca964034f0fcdc3069fc27980/e824b899a9014c08e5e38ca4087b02087af4f4d3.jpg) no-repeat;				
				}
				25% {
					background:url(http://b.hiphotos.baidu.com/image/w%3D400/sign=edee1572e9f81a4c2632edc9e72b6029/30adcbef76094b364d72bceba1cc7cd98c109dd0.jpg) no-repeat;
				}
				50% {
					background:url(http://b.hiphotos.baidu.com/image/w%3D400/sign=937dace2552c11dfded1be2353266255/d8f9d72a6059252d258e7605369b033b5bb5b912.jpg) no-repeat;
				}
				75% {
					background:url(http://g.hiphotos.baidu.com/image/w%3D400/sign=7d37500b8544ebf86d71653fe9f9d736/0df431adcbef76095d61f0972cdda3cc7cd99e4b.jpg) no-repeat;
				}
				100% {
					background:url(http://c.hiphotos.baidu.com/image/w%3D400/sign=cfb239ceb0fb43161a1f7b7a10a54642/3b87e950352ac65ce2e73f76f9f2b21192138ad1.jpg) no-repeat;
				}
			}
	</pre>**
**无JS更好的版本：**  
	<PRE>
			/**HTML**/
			ul.cb-slideshow>li*6
			/**CSS**/
			.cb-slideshow,
			.cb-slideshow:after{
				position:fixed;
				width:100%;
				height:100%;
				top:0;
				left:0;
				z-index:0;
			}
			.cb-slideshow li{
				position:absolute;
				width:100%;
				height:100%;
				top:0;
				left:0;
				color:transparent;
	
				background-size:cover;
				background-position: center;
				background-repeat: none;
				opacity:0;
				z-index:0;
	
				-webkit-backface-visibility: hidden;
				-webkit-animation: loops 36s linear infinite 0s;
			}
			.cb-slideshow li:nth-child(1){
				background-image: url(http://a.hiphotos.baidu.com/image/w%3D2048/sign=bae49cc219d5ad6eaaf963eab5f338db/78310a55b319ebc4dfbad19f8026cffc1f1716f1.jpg);
			}
			.cb-slideshow li:nth-child(2){
				background-image: url(http://e.hiphotos.baidu.com/image/w%3D2048/sign=ccbcc20b249759ee4a5067cb86c34216/5ab5c9ea15ce36d3117f253638f33a87e950b1b9.jpg);
				-webkit-animation-delay: 6s;
			}
			.cb-slideshow li:nth-child(3){
				background-image: url(http://f.hiphotos.baidu.com/image/w%3D2048/sign=856e8c06eb24b899de3c7e385a3e1c95/730e0cf3d7ca7bcba7106129bc096b63f624a849.jpg);
				-webkit-animation-delay: 12s;
			}
			.cb-slideshow li:nth-child(4){
				background-image: url(http://e.hiphotos.baidu.com/image/w%3D2048/sign=b13bc3ec83cb39dbc1c06056e42e0824/b64543a98226cffc72e818b4bb014a90f703eaf2.jpg);
				-webkit-animation-delay: 18s;
			}
			.cb-slideshow li:nth-child(5){
				background-image: url(http://d.hiphotos.baidu.com/image/w%3D2048/sign=8850fe144d4a20a4311e3bc7a46a9922/3b87e950352ac65cdb7ec075f9f2b21193138ab9.jpg);
				-webkit-animation-delay: 24s;
			}
			.cb-slideshow li:nth-child(6){
				background-image: url(http://c.hiphotos.baidu.com/image/w%3D2048/sign=fe5efd301f950a7b753549c43ee963d9/f31fbe096b63f624d9369f058544ebf81a4ca349.jpg);
				-webkit-animation-delay: 30s;
			}
			
			@-webkit-keyframes "loops" {
				0% {
					opacity: 0;
					/*transform:translateY(2000px);
					animation-timing-function:ease-in;*/				
				}
				8% {
					opacity:1;
					/*transform:translateY(-30px);
					animation-timing-function: ease-out;*/
				}
				17% {
					opacity:1;
				}
				25% {
					opacity:0;
					/*transform:translateY(10px);*/
				}
				100% {
					opacity: 0;
					/*transform:translateY(0);*/
				}
			}
	</PRE>
17. 你都使用那些工作来测试代码的性能？

- 例如JSPerf (http://jsperf.com/)
- 例如Dromaeo (http://dromaeo.com/)
- 其它。

18. 如果今年你打算熟练掌握一项新技术，那会是什么？

19. 请谈一下你对网页标准和标准制定机构重要性的理解。

20. 什么是FOUC？你如何来避免FOUC？

HTML相关问题
===========
---
1. 文档类型的作用是什么？你知道多少种文档类型？

2. 浏览器标准模式和怪异模式之间的区别是什么？

3. 使用XHTML的局限有那些？

4. 如果页面使用'application/xhtml+xml'会有什么问题吗？

5. 如果网页内容需要支持多语言，你会怎么做？

6. 在设计和开发多语言网站时，有哪些问题你必须要考虑？

7. 在HTML5的页面中可以使用XHTML的语法吗？

8. 在HTML5中如何使用XML？

9. 'data-'属性的作用是什么？

10. 如果把HTML5看作做一个开放平台，那它的构建模块有那些？

11. 请描述一下cookies，sessionStorage和localStorage的区别？

JS相关问题
=========
---
1. 你使用过那些Javascript库？

2. 你是否研究过你所使用的JS库或者框架的源代码？

3. 什么是哈希表？

4. 'undefined'变量和'undeclared'变量分别指什么？

5. 闭包是什么，如何使用它，为什么要使用它？

6. 你喜欢的使用闭包的模式是什么？

7. 请举出一个匿名函数的典型用例？

8. 请解释什么是Javascript的模块模式，并举出实用实例。

- 如果有提到无污染的命名空间，可以考虑加分。

9. 如果你的模块没有自己的命名空间会怎么样？

10. 你如何组织自己的代码？是使用模块模式，还是使用经典继承的方法？

11. 请指出Javascript宿主对象和内置对象的区别？

12. 指出下列代码的区别：

	Javascript:  
		function Person(){}   
		var person = Person()   
		var person = new Person()

13. '.call'和'.apply'的区别是什么？

14. 请解释'Funciton.prototype.bind'的作用？

15. 你如何优化自己的代码？

16. 你能解释一下JavaScript中的继承是如何工作的吗？

17. 在什么时候你会使用'document.write()'？

18. 大多数生成的广告代码依旧使用'document.write()'，虽然这种用法会让人很不爽。
请指出浏览器特性检测，特性推断和浏览器UA字符串嗅探的区别？

19. 请尽可能详尽的解释AJAX的工作原理。

20. 请解释JSONP的工作原理，以及它为什么不是真正的AJAX。

21. 你使用过JavaScript的模板系统吗？

- 如有使用做，请谈谈你都使用过那些类似库文件。比如Mustache.js,Handlebars等等。

22. 请解释变量声明提升。

23. 请描述下事件冒泡机制。

24. "attribute"和"property"的区别是什么？

25. 为什么扩展JavaScript内置对象是个坏做法？

26. 为什么扩展JavaScript内置对象是个好做法？

27. 请指出document load和document ready的区别。(这是个问题的问题）

28. '=='和'==='有什么不同？

29. 你如何获取浏览器URL中查询字符串中的参数。

30. 请解释一下JavaScript的同源策略。

31. 请解释一下事件代理。

32. 请描述一下JavaScript的继承模式。

33. 如何实现下列代码：

- [1,2,3,4,5].duplicator(); // [1,2,3,4,5,1,2,3,4,5]

34. 描述一种JavaScript memoization(避免重复运算)的策略。

35. 什么是三元条件语句？

36. 函数的参数元是什么？

37. 什么是"use strict"?使用它的好处和坏处分别是什么？

38. JavaScript内存泄漏。

- 什么是内存泄漏？
- JavaScript中哪些原因会导致内存泄漏？
- 有什么样的工具可以检测内存泄漏？
- 应该怎样去避免内存泄漏？

JS代码示例：
----------
---
- ~~3.14  
问题：上面的语句的返回值是什么？  
答案：3

- "i'm a lasagna hog".split("").reverse().join("");  
问题：上面的语句的返回值是什么？  
答案："goh angasal a m'i"

- ( window.foo || ( window.foo = "bar" ) );  
问题：window.foo的值是什么？  
答案："bar" 只有window.foo为假时的才是上面答案，否则就是它本身的值。

- var foo = "Hello";  
(function() {  
	var bar = " World";  
	alert(foo + bar);  
})();  
alert(foo + bar);  
问题：上面两个alert的结果是什么   
答案: "Hello World" & ReferenceError: bar is not defined

- var foo = [];  
foo.push(1);  
foo.push(2);  
问题：foo.length的值是什么？  
答案：'2'

- var foo = {};  
foo.bar = 'hello';  
问题：foo.length的值是什么？   
答案: undefined

- foo = foo||bar  
问题: 这行代码是什么意思?  
答案: if(!foo) foo = bar

- foo>>1  
问题: 这行代码是什么意思?  
答案: Math.floor(foo/2)

- foo|0  
foo+.5|0  
问题: 这行代码是什么意思?  
答案: parseInt(foo) & Math.round(foo)

- function foo(bar1, bar2, bar3){}  
问题: 如何获取参数的个数?  
答案: foo.length //this example is 3

jQuery-Specific Questions:
==========================
jQuery相关问题
=============
---
1. 解释"chaining"。

2. 解释"deferreds"。

3. 你知道那些针对jQuery的优化方法。

4. 请解释'.end()'的用途。

5. 你如何给一个事件处理函数命名空间，为什么要这样做？

6. 请说出你可以传递到jQuery方法的四种不同值。

- 选择器（字符串），HTML（字符串），回调函数，HTML元素，对象，数组，元素数组，jQuery对象等。

7. 什么是效果队列？

8. 请指出'.get()','[]','eq()',的区别。

9. 请指出'.bing()','.live()'和'.delegate()'的区别。

10. 请指出'$'和'$.fn'的区别？或者说出'$.fn'的用途。

11. 请优化下列选择器：

- $(".foo div#bar:eq(0)")

12. 'delegate()'和'live()'有什么区别?

CSS相关问题
==========
---
1. 描述css reset的作用和用途。

2. 描述下浮动和它的工作原理。

3. 清除浮动的方法有那些，分别适用于什么情形。

4. 解释css sprites,如何使用。

5. 你最喜欢的图片替换方法是什么，你如何选择使用。

6. 讨论CSS hacks，条件引用或者其他。

7. 如何为有功能限制的浏览器提供网页。

- 你会使用那些技术和处理方法。

8. 如何视觉隐藏网页内容，只让它们在屏幕阅读器中可用。

9. 你使用过网格系统吗？如果使用过，你最喜欢哪种？

10. 你使用过meidia queries（媒体查询）吗，或者移动网站相关的CSS布局。

11. 你熟悉SVG样式的书写吗？

12. 如何优化网页的打印样式。

13. 在书写高效CSS文件时会有哪些问题需要考虑。

14. 你使用CSS预处理器吗？(SASS,Compass,Stylus,LESS)

- 如果使用，描述你的喜好。

15. 你是否接触过使用非标准字体的设计？

- 字体服务，Google Webfonts, Typekit,等等。

16. 请解释浏览器是如何根据CSS选择器选择对应元素的。

可选的有趣问题
============
---
- 你编写过的最酷的代码是什么？其中你最自豪的是什么？

- 你知道HTML5的帮派标志吗？

- 你是否正在或曾经在一艘船上。(不懂这个幽默）

- 你使用的开发工具中，你最喜欢的部分是什么？

- 你有什么业余项目吗？是那种类型的？

- 解释cornify的重要性？(本题完全摸不到头脑）

- 在一张纸上，垂直写下ABCDE，然后不用任何代码，将他们到序排列。
 + 静静的看他们是否将纸反转。

- 海盗还是忍者？

 + 如果是两者的合体，并有恰当理由，可以加分。如果是僵尸猴子海盗加忍者加两分。(注，此题文化差异过大）

- 如果没有在Web开发，你会做什么？

- 卡门圣迭哥的隐藏处在哪里？

 + 提示：本题的答案永远是错的。

- 你最爱的IE特性是什么？

- 完句填空： Brendan Eich和Doug Crockford是JavaScript的________。

- 讨论：jQuery是牛逼的库还是最牛逼的库。
