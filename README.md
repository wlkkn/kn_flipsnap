kn_flipsnap
===========

flipsnap.js是一个手机屏幕水平滑动框架

1、基本调用方法 Flipsnap(HTMLElement)
；

2、参数设定

    Flipsnap(HTMLElement,{
	    distance:602,//每次移动的距离
	    maxPoint:7,//最大移动次数
	    transitionDuration:1000,//过度时间
	    disableTouch:true,//是否触摸
	    disable3d:true//是否3d
	});

3、可绑定的事件fspointmove、fstouchstart、fstouchmove、fstouchend，绑定方式

    flipsnap.element.addEventListener('fspointmove',function(){})
	或者通过jquery
	$(flipsnap.element).bind('fspointmove', function() {
    	// do something
	}, false);

4、可使用的方法

    
	  flipsnap.refresh();//刷新当前页面
	  flipsnap.hasNext();
	  flipsnap.hasPrev();
	  flipsnap.toNext([transitionDuration]);
	  flipsnap.toPrev([transitionDuration]);
	  flipsnap.moveToPoint(point,[transitionDuration]);