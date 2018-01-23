###Welcome to use MarkDown
absolute定位与margin定位其实是没有什么冲突的，无论absolute元素时候设置了left/top值，其margin属性值都是可以起作用的。
下面展示的是没有left/top值的absolute元素的margin定位。
http://www.zhangxinxu.com/wordpress/2010/01/absolute绝对定位的非绝对定位用法/

2018年1月23号

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
