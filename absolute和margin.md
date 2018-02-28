###Welcome to use MarkDown
absolute定位与margin定位其实是没有什么冲突的，无论absolute元素时候设置了left/top值，其margin属性值都是可以起作用的。
下面展示的是没有left/top值的absolute元素的margin定位。
http://www.zhangxinxu.com/wordpress/2010/01/absolute绝对定位的非绝对定位用法/

2018年1月23号
v
说一下box-sizing的应用场景
盒子模型有两种，ie和w3c的，ie的盒子模型，content包括border和padding；
考虑到盒子的大小设置会比较麻烦，有时设置的width，结果最后大小不是之前设置的大小，所以这时就要box-sizing登场了，
当我们设置box-sizing:border-box以后，如果我们想要一个宽度100的盒子，直接设置width为100，就不用考虑该盒子是否为标准盒子了。
说一下你了解的弹性FLEX布局.
分为两条轴，x轴和y轴，还有一些特殊的属性，支持ie10以上的浏览器，目前应用在移动端比较多的，
Babel应用的就是es6到es5 的一个编译
DOM事件中target和currentTarget的区别
currentTarget(你绑定事件的那个元素), target(触发事件的那个目标) 
JSONP的原理和实现以及cors怎么设置。看一下这篇就足够了。
https://www.cnblogs.com/banning/p/6250677.html

最简单的数组去重

<script type="text/javascript">
	var bb;
	var aa=[1,2,3,1,'a',1,'a']
	  bb=aa.filter(function(ele,index,array){
	  	console.log(ele,index,array)
    return index===array.indexOf(ele)
   })
	  console.log(bb)
</script>

错误的积累：
Uncaught TypeError: Cannot read property 'length' of undefined；报这种length错误的信息，
一般是length前面的那个变量是undefined；

2018年1月26日
对jsp的页面的一些了解，还有对php和.net的比较
https://segmentfault.com/a/1190000012990520

2018年1月27日
localStrorage,sessionStrorage,cookie 都是属于web Storage
sessionStorage 是保存会话数据，localStorage 在客户端长期保存数据
sessionStorage: 该数据实质上是被保存在session对象中，保存用户的临时会话数据，一旦关闭浏览器，所有数据都会消失
localStorage: 该对象可将数据长期保存在客户端中，即使重新打开浏览器也不会丢失
cookie: 将数据保存在用户的客户端，存在于用户硬盘文件上，其缺点事：限制保存数据空间大小，数据保密性差、代码操纵复制等。
 
区别：
1.数据的有效性不同，sessionstorage仅在当前浏览器中有效，关闭浏览器数据消失。localstorage关闭浏览器也有效。cookie只在设置cookie过期时间内有效，无论浏览器是否关闭。
2.作用域不同。sessionStorage不在不同浏览器窗口中共享。localStorage在所有同源窗口中共享。cookie也是所有同源窗口中共享
 
不同浏览器无法共享localStorage或sessionStorage中的信息，相同浏览器的不同页面可以共享相同的localStorage（页面属于相同域名和端口），但是不同页面或标签页间无法共享sessionStorage的信息。
 
总结：localStorage需要在同主域名和端口下才能互相访问 而且是一直保留
sessionStorage只能在单个窗口页面中进行保留
 
允许存储大小：谷歌浏览器5M左右，不同浏览器可存储大小不同
 
cookie 可存储大小4KB

2018年1月28日
7
<script type="text/javascript">
	 判断数组里面的最大值,并显示这个值的name;
	 var aa;
	 var arr=[{a:7},{b:2},{c:0},{d:5},{e:1}];
	 aa=arr.sort(function(item1,item2){
    return item2[Object.keys(item2)[0]]-item1[Object.keys(item1)[0]]
  })[0] 
  console.log(aa,32)
</script>


2018年1月29号；
作者;李星亮；
所谓“健壮”，即最基本的兼容性处理、边界处理，异常处理、用户输入校验。很多时候，需求方不会明确告诉你这些逻辑怎么处理，但并不意味着你不需要处理。
2018年1月30号；
javascript 总结（常用工具类的封装）以下是地址；
https://segmentfault.com/a/1190000013041329
2018年1月31号
addEventListener()js中的监听事件，可以监听好多的点击的动作，然后可以给所需要的东西添加一些内容b
2018年2月2号

学习node.js文档，
 * 学习了node的安装和介绍
    http://www.runoob.com/nodejs/nodejs-tutorial.html
 * node.js EventEmitter 
     node中的许多对象都会分发事件，一个net server对象会在每次有新的连接的时分发一个事件，一个fs.readstream对象会在文件被打开的时候发出一个文件，所有产生这些事件的对像
            都是evenrs.EventEmitter的是列。
 * node.js路	由router 
      自己编写一个router.js文件，然后配置好http的请求，随后在node中跑起来。
  骚气的注释号！                                                                                
     /*
      var foo = "bar";  
      */
             第一种隐藏e
      //*
      var foo = "bar";
      */
             第二种展示;
 *input的轮过；
     outline:0;鼠标点击的时候边框是蓝色，设置上这个属性就好了。
     text-indent：首行缩进；
 *  relative移动后仍占据原来的位置，不会脱离文档，absolute移动后，不会占据原来的位置的，
   10000小时定律；   
 * box-sizing是什么
     设置CSS盒模型为标准模型或IE模型。标准模型的宽度只包括content，二IE模型包括border和padding
     box-sizing属性可以为三个值之一：

	content-box，默认值，只计算内容的宽度，border和padding不计算入width之内
	padding-box，padding计算入宽度内
	border-box，border和padding计算入宽度之内
 
  