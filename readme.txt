1. 改变this指向的方式
	以下属于函数的方法
	改变this的指向并且执行调用函数
	.call(),  call(thisScope, arg1, arg2, arg3...)
	.apply(), apply(thisScope, [arg1, arg2, arg3...]);两个参数

	.bind()  bind(thisScope, arg1, arg2, arg3...)改变this的指向，返回的是函数


2. Math对象的方法
	Math.random(); //随机小数0~1之间
	Math.ceil();   // 向上取整
	Math.floor();  // 向下取整
	Math.round();  //四舍五入
	Math.sin();    //三角函数
	Math.PI;       //圆周率
	Math.abs()     //求绝对值
	Math.max();	   //求大数
	Math.max(2,3,1,3,1,3,9,5,6,7)  9
	Math.min();    //求小数

3. 求数组元素的最大值/最小值
	Math.max.apply(null,[1,2,-2]);
	Math.min.apply(null,[1,2,-2])


4. 获取非行间样式
	现代浏览器支持：getComputedStyle(ele) 返回样式对象，只读，不可修改
	如需修改样式，使用element.style.height = '200px'

	IE8以下使用 ele.currentStyle



5. 全局函数
	setInterval()
	setTimeout()
	parseInt()
	getComputedStyle()


6. document整个文档对象
	document.documentElement 页面根元素html
	document.body 页面中的body元素


7.  定位父级，祖先元素有设置position:relative/absolute/fixed之一，没有则为body
	以下属性均为只读
	element.offsetParent 定位父级

	element.offsetLeft  相对定位父级的左偏移值
	element.offsetTop	相对定位父级的上偏移值

	element.offsetWidth 宽度 包括border + padding + width
	element.offsetHeight 高度 包括 border + padding + height

	element.clientWidth 宽度 包括padding + width
	element.clientHeight 高度 包括padding + height
	element.clientTop   元素上边框宽度
	element.clientLeft  元素左边框宽度


8. ele.children 元素ele所有子元素组成的数组【类数组对象】，不能使用真正数组里的方法，如push,pop...