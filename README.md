# 网易前端微专业大作业
## 1.1	关闭顶部通知条
	点击顶部通知条中的“X 不再提醒”后，刷新页面不再出现此通知条（使用本地cookie实现）。
## 1.2	关注“网易教育产品部”/登录
	点击关注按钮：首先判断登录的cookie是否已设置（loginSuc）
	如果未设置登录cookie，则弹出登录框，使用给定的用户名和密码（需要表单验证）调用服务器Ajax登录，成功后设置登录cookie
	登录成功后，调用关注API，并设置关注成功的cookie（followSuc）
	登录后“关注”按钮变成不可点的“已关注”状态。按钮的hover效果见视觉稿
## 1.3	顶部右侧导航及内容区各产品的“了解更多”
	点击导航中的“网易公开课”，“网易云课堂”，“中国大学MOOC”，新窗口打开对目的页面，对应的跳转链接如下，点击项的hover效果见视觉稿。点击“了解更多>”的跳转链接及打开方式相同。
	网易公开课：http://open.163.com/
	网易云课堂：http://study.163.com/
	中国大学MOOC：http://www.icourse163.org/
## 1.4	轮播图
	三张轮播图轮播效果：实现每5s切换图片，图片循环播放；鼠标悬停某张图片，则暂停切换；切换效果使用入场图片500ms淡入的方式。点击后新开窗口打开目的页面，对应的跳转链接如下，
	banner1：http://open.163.com/
	banner2：http://study.163.com/
	banner3：http://www.icourse163.org/
## 1.5	左侧内容区tab切换
	点击“产品设计”或“编程语言”tab，实现下方课程内容的更换。tab项的hover及选中效果见视觉稿，tab项对应的课程卡片数据见本文档的数据接口列表
## 1.6	查看课程详情
	鼠标悬停“产品设计”或“编程语言”tab下的任意课程卡片，出现浮层显示该课程的课程详情；鼠标离开课程详情浮层，则浮层关闭。课程卡片即详情浮层的效果见视觉稿，课程卡片及详情数据见本文档的数据接口列表
## 1.7	右侧“机构介绍”中的视频介绍
	点击“机构介绍”中的整块图片区域，调用浮层播放介绍视频。图片的hover效果见视觉稿，浮层中调用的播放器（不做浏览器兼容,可用html5）及视频内容接口见本文档的数据接口列表
## 1.8	右侧“热门推荐”
	实现每次进入或刷新本页面，“热门推荐”模块中，接口返回20门课程数据，默认展示前10门课程，隔5秒更新一门课程，实现滚动更新热门课程的效果。课程数据接口见本文档的数据接口列表
## 1.9	页面布局动态适应
	根据浏览器窗口宽度，适应两种视觉布局尺寸。窗口宽度<1205时，使用小屏视觉布局；窗口宽度>=1205时，使用大屏视觉布局。布局示意图见视觉效果
