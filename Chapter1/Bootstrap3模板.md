# Bootstrap3模版
* 在head头部中都会插入的meta的几个标签：
	* `<meta charset="utf-8">`  规定 HTML 文档的字符编码
	* `<meta name="renderer" content="webkit">`可以让部分国产浏览器默认采用高速模式渲染页面
	* `<meta http-equiv="X-UA-Compatible" content="IE=edge">`为了让 IE 浏览器运行最新的渲染模式下
	* `<meta name="viewport" content="width=device-width, initial-scale=1">`为了保证在移动端能够正常的显示


* ``[if xxx] ![endif]`这个是IE中的条件注释, 只有在IE浏览器下才会执行以下代码的含义: 如果当前是IE9以下的浏览器, 那么就导入以下的两个JS文件
	* `respond.js`是为了能够在IE8以及IE8以下的浏览器中使用媒体查询(https://cdn.jsdelivr.net/npm/html5shiv@3.7.3/dist/html5shiv.min.js)
	* `html5shiv.js`是为了能够在IE8以及IE8以下的浏览器中使用H5新增的标签(https://cdn.jsdelivr.net/npm/respond.js@1.4.2/dest/respond.min.js)

```
	<!DOCTYPE html>
	<html lang="zh-CN">
	<head>
	    <meta charset="utf-8">
	    <meta name="renderer" content="webkit">
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <meta name="viewport" content="width=device-width, initial-scale=1">
	    <title>自己网页的标题</title>
	    <!-- 导入Bootstrap的CSS文件 -->
	    <link rel="stylesheet" href="css/bootstrap.css">
	
	    <!--[if lt IE 9]>
	        <script src="js/html5shiv.js"></script>
	        <script src="js/respond.js"></script>
	    <![endif]-->
	</head>
	<body>
	<script src="js/jquery-1.12.4.js"></script>
	<script src="js/bootstrap.js"></script>
	</body>
	</html>
```