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
