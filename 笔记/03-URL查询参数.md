# URL查询参数
**定义：** 浏览器提供给服务器的==额外信息==，让服务器返回浏览器想要的数据
**语法：** 
![[AJAX/笔记/img/0301.png]]
![[0302.png]]

## axios-查询参数
**语法：** 使用axios提供的==params==选项
**注意：** axios在运行时会把参数名和值拼接到url==?参数名=值== 
**城市列表：** https://hmajax.itheima.net/api/city?pname=福建省

```
axios({
	url:'目标资源地址'
	params:{
		参数名:值
	}
}).then(result=>{
	// 对服务器返回的数据做后续处理
})
```
**示例：**
```
axios({
	url:' https://hmajax.itheima.net/api/city'
	params:{
		pname:'福建省'
	}
}).then(result=>{
	// 对服务器返回的数据做后续处理
})
```


#axios
上一篇：[[02-认识URL]]
下一篇：[[04-常用请求方法和数据提交]]