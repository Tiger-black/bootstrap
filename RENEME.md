响应式开发 某个作者2010年提出的 弹性布局，流动布局 宽度不确定 百分比走 它的优化程度有限。响应式网站设计 引入媒体查询 按分辨率割裂 针对不同的设备改变不同的样式。

流动网格、弹性图媒体查询是响应式互联网设计的三大技术成分。 响应式网站是一个设计理念，它是多项技术的综合体。

优点 ： 
一 减少工作量 
	1网站、设计、代码、内容都只需要一份，不用维护多份html、css、js； 
	2多出来的工作量只是js脚本、css样式做一些改动 
二 节省时间 迅速发布 快速迭代 敢于试错 小步快跑成为了互联网企业的基本理念，我们节省一点点时间，提高一点用户体验，使企业离成功更进一步； 

三 面向未来 每个设备都能得到正确的设计 

四 搜索优化 针对不同的设备它的url是相同的 有利于搜索爬虫 

五 更好的用户体验，更利于统计用户来源 

缺点 ： 
一 会加载更多的样式和脚本资源 

二 设计比较难精确定位和控制 

三 对于老版本的浏览器兼容不太好

媒体查询 返回布尔值 @media 
	标识 all（默认 所有设备）／ screen（屏幕）／ print（打印设备）..... ； 
	and（并且符）／or（或）／ not（非） ； ／only（针对老浏览器，只看第一个单词 如果写的media=screen 老的浏览器就认为成立 不管后面的表达式） 
		only最好不要省略 除非你确定不考虑老的浏览器 
	css3主要的媒体属性 视口宽度width height 











	让老的浏览器可以用，让新的浏览器体验更好
1、渐性增强（先构建基本效果 逐渐追加新功能） & 优雅降级 （先来最终状态 根据浏览器兼容的性能针对的剔除功能）；
	优雅降级的设计比较人类。老版浏览器占比低～

2、根据个人习惯和网站性质 自行决定先开发小屏幕还是大屏幕

3、浏览器选择 针对创业公司
	pc: 最新几个版本的 chrome、火狐、ie9+
	M：	UC、QQ、安卓原生浏览器、IOS浏览器
	一般先用一个浏览器开发完成再调试其他浏览器。

响应式网站设计实践原则
	-不管设备大小，应该包含相同的内容还是显示不同的内容 前端不需要关注让产品经理来选 
	-端点的选择 媒体查询的零界点
	   不要针对特定的设备来做选择 应该针对屏幕的大小来进行分割 根据宽度分几个类型
	   比如 （具体实践根据设计师的设计来定）
	   	屏幕小于480像素的为小屏幕
	   	481 - 800像素的为中屏幕
	   	801 - 1400像素的为大屏幕
	   	1400+ 像素的为巨大屏幕

	约定大于配置
	约定代码结构或命名规范来减少代码配置数量










