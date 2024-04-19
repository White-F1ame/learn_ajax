## 什么是AJAX？

**定义：**
> AJAX是异步的[[JavaScript]]和[[XML]]（**A**synchronous **J**avaScript **A**nd **X**ML）。简单点说，就是==使用XMLHttpRequest对象与服务器通信==。它可以使用JSON，XML，HTML和text文本等格式发送和接受数据。AJAX最吸引人的就是它的“异步”特性，也就是说它可以在不重新刷新页面的情况下与服务器通信，交换数据或更新页面

**概念：** AJAX是浏览器与服务器进行==数据通信==的技术
![[0101.png]]

## 怎么用AJAX？
1. 先使用[[axios]]库，与服务器进行==数据通信== 
	- 基于XMLHttpRequest封装、代码简单、月下载量14亿次
	- ==Vue、React项目中都会用到axios==
2. 再学习XMLHttpRequest对象的使用，了解AJAX底层原理

## axios使用
**语法：**
1. 引入axios.js：
```
		<script src="https://cdn.jsdelivr.net/npm/axios/dist/axios.min.js"></script>
```
1. 使用axios函数
	1. 传入==配置对象==
	2. 再用==.then==回调函数接受结果，并做后续处理
```
		axios({
			url:'目标资源地址'
		}).then((result)=>{
			// 对服务器返回的数据做后续处理
		})
```

需求：请求目标资源地址，拿到省份列表数据，显示到页面
目标资源地址：*https://hmajax.itheima.net/api/province
