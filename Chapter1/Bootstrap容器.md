## Bootstrap容器

     在Bootstrap中容器是响应式布局的基础, Bootstrap推荐将所有内容都定义在容器之中
     并且容器是启用Bootstrap栅格系统必不可少的前置条件


* Bootstrap中提供了两个容器: `container/container-fluid`
    * `container容器(固定容器)`:
    只要给标签添加了container类名, 这个标签就变成了Bootstrap的container容器
    只要这个标签变成了Bootstrap的container容器, 在不同视口大小下就会有不同的固定宽度
    * `container-fluid(自适应宽度容器)`
    只要给标签添加了container-fluid类名, 这个标签就变成了Bootstrap的container-fluid容器
    只要这个标签变成了Bootstrap的container-fluid容器, 那么容器的宽度永远都是100%自适应


* Bootstrap对视口划分

	Bootstrap4将视口划分为了5种：
     - 超小屏幕(xs): <576px
     - 小屏幕(sm): >=576px
     - 中等屏幕(md):>=768px
     - 大屏幕(lg): >=992px
     - 超大屏幕(xl): >= 1200px
 
 
* 容器实现
```
	<!doctype html>
	<html>
	<head>
	    <meta charset="utf-8">
	    <title>05-Bootstrap容器实现</title>
	    <style>
	        *{
	            margin: 0;
	            padding: 0;
	        }
	        .container {
	            width: 100%;
	            padding-right: 15px;
	            padding-left: 15px;
	            margin-right: auto;
	            margin-left: auto;
	        }
	
	        @media (min-width: 576px) {
	            .container {
	                max-width: 540px;
	            }
	        }
	
	        @media (min-width: 768px) {
	            .container {
	                max-width: 720px;
	            }
	        }
	
	        @media (min-width: 992px) {
	            .container {
	                max-width: 960px;
	            }
	        }
	
	        @media (min-width: 1200px) {
	            .container {
	                max-width: 1140px;
	            }
	        }
	        div{
	            height: 100px;
	            background: red;
	        }
	    </style>
	</head>
	<body>
	<div class="container"></div>
	</body>
	</html>
```