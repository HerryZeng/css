## 直接上代码

```html
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>Document</title>
	<style type="text/css">
#box{ 
          width:500px; 

          background:#000; 

          height:500px;
          /*overflow: hidden;*/
          border: 3px solid black;

 } 

#content { 

          float:left; 

          width:600px; 

          height:600px; 

          background:red;

 } 
	</style>
</head>
<body>

	<div id="box">
		<div id="content"></div>
	</div>
	
</body>
</html>
```
如下图：
![](../images/chapter02/024.png)

给`box`这个`div`加了一个`overflow:hidden`这个属性解决了这个问题。我们知道`overflow:hidden`这个属性的作用是隐藏溢出，给`box`加上这个属性后，我们的`content` 的宽高自动的被隐藏掉了。

```html
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>Document</title>
	<style type="text/css">
#box{ 
          width:500px; 

          background:#000; 

          height:500px;
          overflow: hidden;
          border: 3px solid black;

 } 

#content { 

          float:left; 

          width:600px; 

          height:600px; 

          background:red;

 } 
	</style>
</head>
<body>

	<div id="box">
		<div id="content"></div>
	</div>
	
</body>
</html>
```
![](../images/chapter02/025.png)

另外，我们再做一个试验，将box这个div的高度值删除后，我们发现，box的高度自动的被content 这个div的高度值给撑开了。

```html
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>Document</title>
	<style type="text/css">
#box{ 
          width:500px; 

          background:#000; 

          /*height:500px;*/
          overflow: hidden;
          border: 3px solid black;

 } 

#content { 

          float:left; 

          width:600px; 

          height:600px; 

          background:red;

 } 
	</style>
</head>
<body>

	<div id="box">
		<div id="content"></div>
	</div>
	
</body>
</html>
```
![](../images/chapter02/026.png)

