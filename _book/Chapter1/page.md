# Bootstrap3模版
```
	<!DOCTYPE html>
	<html lang="zh-CN">
	<head>
	    <meta charset="utf-8">
	    <!--可以让部分国产浏览器默认采用高速模式渲染页面-->
	    <meta name="renderer" content="webkit">
	    <!--为了让 IE 浏览器运行最新的渲染模式下-->
	    <meta http-equiv="X-UA-Compatible" content="IE=edge">
	    <!--为了保证在移动端能够正常的显示-->
	    <meta name="viewport" content="width=device-width, initial-scale=1">
	    <title>自己网页的标题</title>
	    <!-- 导入Bootstrap的CSS文件 -->
	    <link rel="stylesheet" href="css/bootstrap.css">
	
	    <!--导入respond.js文件的目的, 是为了能够在IE8以及IE8以下的浏览器中使用媒体查询-->
	    <!--导入html5shiv.js文件的目的, 是为了能够在IE8以及IE8以下的浏览器中使用H5新增的标签-->
	    <!--
	    [if xxx] ![endif]这个是IE中的条件注释, 只有在IE浏览器下才会执行
	    以下代码的含义: 如果当前是IE9以下的浏览器, 那么就导入以下的两个JS文件
	    -->
	    <!--[if lt IE 9]>
	        <script src="js/html5shiv.js"></script>
	        <script src="js/respond.js"></script>
	    <![endif]-->
	</head>
	<body>
	<!-- jQuery (Bootstrap 的所有 JavaScript 插件都依赖 jQuery，所以必须放在前边) -->
	<script src="js/jquery-1.12.4.js"></script>
	<!-- 加载 Bootstrap 的所有 JavaScript 插件。你也可以根据需要只加载单个插件。 -->
	<script src="js/bootstrap.js"></script>
	</body>
	</html>
```