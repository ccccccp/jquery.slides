# jquery.slides
一款基于jQuery无缝轮播图插件,支持图内元素动画，可以自定义动画类型

初始化插件

$(".slideInner").slide({

	slideContainer: $('.slideInner a'),
	
	effect: 'easeOutCirc',//动画类型
	
	autoRunTime: 5000,//自动轮播时间
	
	slideSpeed: 1000,//速度
	
	nav: true,//是否显示左右导航
	
	autoRun: true,//是否自动滚动
	
	prevBtn: $('a.prev'),//左按钮
	
	nextBtn: $('a.next')//右按钮
	
	});

兼容性：
ie8+、google、firefox、360、QQ、欧朋、safi

html实例讲解：


<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
	<head>
		<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
		<title>智我首页</title>
		<meta name="Resource-type" content="Document" />
		<meta name=renderer content=webkit>
		<meta http-equiv=x-ua-compatible content=ie=edge>
		<meta http-equiv=x-ua-compatible content=ie=edge,chrome=1>
		<!--[if lte IE 6]>
		<script type="text/javascript" src="js/image.js"></script>
		<script type="text/javascript" src="js/png.js"></script>
		<script type="text/javascript">
		DD_belatedPNG.fix('div, ul, img, li, input , a,span');
		</script>
		<![endif]-->
		<link rel="stylesheet" type="text/css" href="css/slide.css"/>
		<script src="js/jquery.min.js"></script>
		<script src="js/slide.js" type="text/javascript" charset="utf-8"></script>
		<script type="text/javascript">
			$(document).ready(function() {
				$(".slideInner").slide({
					slideContainer: $('.slideInner a'),
					effect: 'easeOutCirc',
					autoRunTime: 5000,
					slideSpeed: 1000,
					nav: true,
					autoRun: true,
					prevBtn: $('a.prev'),
					nextBtn: $('a.next')
				});
			});
		</script>
	</head>
	<body>
		<div class="slides">
			<div class="slideInner">
				<a href="#" style="background: url(img/slide1.jpg) no-repeat;">
					<div class="moveElem img1" rel="0,easeInOutExpo">
						<img src="img/slide1p1.png" />
					</div>
					<div class="moveElem img2" rel="150,easeInOutExpo">
						<img src="img/slide1p2.png" />
					</div>
				</a>
				<a href="#" style="background: url(img/slide2.jpg) no-repeat">
					<div class="moveElem img1" rel="0,easeInOutExpo">
						<img src="img/slide2p1.png" />
					</div>
				</a>
				<a href="#" class="slide3" style="background: url(img/slide3.jpg) no-repeat;">
					<div class="moveElem img1" rel="0,easeInOutExpo">
						<img src="img/slide3p1.png" />
					</div>
					<div class="moveElem img2" rel="150,easeInOutExpo">
						<img src="img/slide3p2.png" />
					</div>
					<div class="moveElem img3" rel="300,easeInOutExpo">
						<img src="img/slide3p3.png" />
					</div>
				</a>
				<a href="#" style="background: rgb(113, 209, 231);">
					<div class="moveElem img1" rel="0,easeInOutExpo">
						<img src="img/slide1p1.png" />
					</div>
					<div class="moveElem img2" rel="150,easeInOutExpo">
						<img src="img/slide1p2.png" />
					</div>
				</a>
				<a href="#" style="background: rgb(178, 44, 44);">
					<div class="moveElem img1" rel="0,easeInOutExpo">
						<img src="img/slide1p1.png" />
					</div>
					<div class="moveElem img2" rel="150,easeInOutExpo">
						<img src="img/slide1p2.png" />
					</div>
				</a>
				
			</div>
			<div class="nav">
				<a class="prev" href="#"></a>
				<a class="next" href="#"></a>
			</div>
		</div>
	</body>

</html>
