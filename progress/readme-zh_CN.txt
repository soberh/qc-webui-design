进度条的设计

已测试通过的浏览器:
1) ie6 2010-08-07
2) firefox3.6.8 2010-08-07
3) chrome5.0 2010-08-07
4) safari5.0 2010-08-07

设计说明：
进度条的DOM结构如下
	<div class="progress">
		<div class="percent">50%</div>
		<div class="current"></div>
	</div>
其中progress为进度条的外框架，控制进度条的长度和高度；percent负责显示百分比的文字；current则显示动画进度条；
设计的重点是percent的css控制，须将position设置为absolute的绝对定位方式，否则文字和图片就会上下分离。
通过修改current的背景图片就可以控制界面的显示效果。