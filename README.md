# jquery.slides
一款基于jQuery无缝轮播图插件,支持图内元素动画，可以自定义动画类型

初始化插件
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
