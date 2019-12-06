# 01Day--软件测试基础班

### 1天3小节

操作系统分类:操作系统主要作用是管理好硬件设备.

系统软件:
1,桌面操作系统
​	windows系列   用户群体大
​	macOS        适合开发人员
​	linux        应用软件少
2,服务器操作系统
​	linux        安全,稳定,免费 占有率高
​	windows server   付费      占有率低
3,嵌入式操作系统
4,移动设备操作系统
应用软件:qq...

------

### 1天4小节

##### B/S架构  C/S架构

​	B/S架构:浏览器和服务器架构,通过浏览器打开的.包含客户端浏览器,web应用服务器,数据库服务器的软件系统.用户只需要一个浏览器就可以访问服务.系统更新时,只需要更新服务端,不需要更新浏览器(比如淘宝网站,微博网站)
C/S架构:客户机和服务器结构.这种结构与B/S最显著的区别是需要安装客户端,通过客户端程序来访问应用系统.所以更新时,既要更新服务端,也要更新客户端(比如微信,手游等软件)

##### bs和cs优缺点:

1,硬件环境不同:cs使用局域网(局部专用网络)   bs使用广域网
2,安全要求:  cs安全性较高,bs面向所有用户(使用浏览器可以访问),安全性低.
3,系统维护不同: cs表现方式有限,对程序员要求高   bs表现丰富,开发难度低
4,处理问题不同,cs用户固定,安全要求高   bs面向所有用户

------

### 1天7小节

计算机网络---OSI七层模型
​	应用层:所有应用程序的网站在此展开
​	表示层:数据的加密解密
​	会话层:负责建立,维护,拆除会话
​	传输层:负责建立一个可靠的端到端的链接
​	网络层:负责路由寻址和广播
​	数据链路层:负责将上层数据封装成帧
​	物理层:只负责传输01二进制比特流

------

### 1天8小节   IP地址分类

##### TCP/IP协议

​	定义:网络通讯协议
​	应用层:应用程序之间相互沟通的层
​	传输层:提供了数据传送,应用程序之间的通信服务
​	网络互联层:负责提供基本的数据封包传送功能,让每一块数据包都能够到达目的主机
​	网络接口层:接收数据,并进行传输.

##### IP地址分类

​	ipv4:已枯竭,由四段数字组成
​	ipv6:无穷多,由六段数字组成

##### 按照地址类别分类:

​	1,A类地址:第一组数字  1---126
​	2,B类地址:第一组数字  128---191
​	3,C类地址:第一组数字  192---223
​	4,保留IP地址(只能用在局域网中)
​		10开头
​		127开头
​		172.16.0.0---172.31.255.255
​		192.168.*.*

------

### 1天9小节  dos基础操作

- win+r打开运行窗口,输入cmd点击确定,打开命令行窗口.通过输入dos命令,可以操作计算机.
- ipconfig/all    查看电脑的物理地址(mac地址)
- arp -a   查看ip地址和物理地址的对应关系
- ping(空格)网络地址    查看当前计算机和要访问的计算机之间的连通情况
- cls    清屏
- 盘符:(E:)   切换对应的盘符(进入到E盘,记得冒号) 
- cd(空格)文件名    进入到对应的文件夹(目录)
- dir  显示当前文件夹中的文件内容
- cd..    返回上级目录
- cd/     返回根目录(盘符)
- md(空格)名字   建立文件夹
- rd(空格)名字    删除文件夹 但不能删除有内容的文件夹
- copy(空格)想要复制谁(空格)目标路径  复制文件,需要打开盘符,在其中复制路径
- move  移动,使用方法同copy一样
- del(空格)目录名字    删除目录内的所有文件
- del*.*      删除当前目录中的所有文件(不是文件夹)
- del(空格)具体的文件目录和名字    可以单独删除某一文件
- 键盘的左箭头,右箭头可以移动光标的位置   上,下箭头可以快速生成写过的代码
- format千万不能试,否则会清空硬盘数据

------

### 1天10小节 网址 域名

​	网址上线条件:1,网页代码    2,域名      3,服务器
​	域名提供商有:
​	1,www.net.cn
​	2,www.xinnet.com
​	3,www.west263.com
​	把网站内容传到域名下,别人通过搜索域名就可以访问你的网站
​	网站内容最终传到一个空间,或者服务器,或者云存储
​	空间  服务器   云存储

### 1天11小节过一遍

------

# 基础班第2天   软件测试原理

### 2天3小节 测试的目的,定义,原则

##### 一,什么是软件测试

​	在规定条件下对程序进行操作,从而发现问题,对软件质量进行评估的过程.

##### 二,软件测试的目的

​	以最少的人力,物力,时间找到软件中的缺陷并修改,从而回避商业风险.

##### 三,软件测试的定义

​	使用人工和自动手段来运行程序,目的在于检验是否满足了需求.

##### 四,软件测试原则

​	1,所有测试追溯到用户需求
​	2,把尽早和不断的测试,作为座右铭
​	3,测试工作要由专业人员来执行
​	4,80%的错误出现在20%的模块中
​	5,设计测试用例(测什么?怎么测)时,要考虑各种情况
​	6,一定要写缺陷报告
​	7,制定严格的测试计划
​	8,完全测试是不可能的,测试要终止
​	9,注意回归测试(修改了旧代码后,要确认没有引入新的问题)
 	10,妥善保管好测试文档

### 2天4小节  软件质量模型(iso9126)

​		1,功能性(满足明确和隐含要求的功能的能力)
​		2,可靠性(1,尽量不出问题  2,出了问题不能影响主体功能   3,如果影响了主体功能,要能尽快修复)
​		3,易用性(用户体验要好)
​		4,效率(产品性能)
​		5,可维持性(更新)
​		6,可移植性(跨越不同系统平台)

### 2天5小节  软件质量模型保证(SQA)

​		目的:使软件制作的过程对于领导层是可见的.
​		定义:它是一套计划和方法来向领导层保证.
​		5个基本目标:
​			保证有计划地进行
​			保证遵循了步骤和需求
​			及时通知给对应人员
​			高管可以接触到项目内部
​			软件质量需要测试工作来保证
​		qc和qa
​		qc:检验产品的质量
​		qa:审计过程的质量
​		工作关系:qc是进行质量控制,qa是确保qc按照步骤执行

### 2天6小节   软件测试基本流程

​		1,需求分析
​		2,编写测试用例
​		3,评审测试用例
​		4,搭建测试环境
​		5,等待开发提交测试包
​		6,部署测试包
​		7,冒烟测试(对软件主体基本功能进行基本测试)
​		8,执行测试用例
​		9,bug跟踪处理(提交及回归bug)
​		10,n轮之后符合需求
​		11,测试结束,妥善保存一切测试文档

### 2天7小节   登录界面分析

# 3天  HTML基础

##### img图片标签

​	img是一个单标签
​	<img src="图片名字" width="宽度" height="高度" alt="1,图片未加载的提示文字  2,网页阅读器可以读取这里的文字" title="鼠标悬停时的提示文字" />
​	注意:属性名="属性值"后面是一个空格,然后在写下一个属性.  属性设置不分先后

##### 超链接

​	

```
如果想跳转到线上网站,必须添加http://才可以
	<a href="http://www.baidu.com">跳转到百度</a>
	跳转到本地文件,直接写文件名,因为没上线,所以没有http
	<a href="我的订单01">跳转到订单页</a>
	想在新窗口中打开,设置属性 target="_blank"
	<a href="我的订单01" target="_blank">在新窗口打开订单页</a>
	暂时没有目标地址,想做一个空链接的3种方法
	<a href="###">空链接</a>
	<a href="javascript:;">空链接</a>
	<a href="javascript:void(0);">空链接</a>
	这3种空链接的方法都对,只有当写1个,2个,或不写#,才要提bug
	锚点链接,给目标位置写一个id="属性值", a标签的href写#id=""
```



##### form表单

​	<form action="" method="get">
​	action代表数据给哪个后台程序
​	method代表传输过程中使用post或者get形式
​	<input type="text" placeholder="占位文字"/>
​	placeholder属性属于html5最新的属性,它不兼容ie低版本浏览器(6,7,8,9).此效果虽然低版本ie不支持,但不会造成页面混乱,我们认为此属性没有问题.placeholder比value的用户体验好.
​	</form>

# 4天 css第一天

### 2节 单选框

​	举例html中性别案例
​	性别:<input type="radio" name="xb" id="nan" checked="checked" /> <label for="nan">男<label /> <input type="radio" name="xb" id="nv"> <label for="id">女<label />
​	单选框的类型  type="radio" name="必须有值,才可实现单选"
​	如果想点击文字,就能选中当前的单选框,给文字加label for="属性值",对应的单选框加id="属性值"
​	设置默认选中的状态,给指定的单选框加 checked="checked"

### 3节  下拉菜单

​	下拉菜单为select与option的组合
​	如果想设置多组下拉菜单,需要给小类加一个optgroup标签,并设置label属性作为提示文字
​	如果设置默认选中状态,给option添加selected="selected"

### 4节 文本域 textarea

​	<textarea><textarea />
​	textarea 文本域不能设置rows,cols属性,因为浏览器解析的结果不一样.如果想让每个浏览器大小相同,必须设置width,height

### 5节  多选框, 使用方法和单选框

​	爱好:<input type="checkbox" id="tw" checked="checked" /> <label for="tw">跳舞<label /> <input type="checkbox"  id="sf"> <label for="sf">书法<label />

### 6节 按钮类和用户体验细节

##### 按钮类 

​	1,提交按钮 <input type="submit" value="必须设置值"/>  否则浏览器之间有兼容性问题.
​	2,重置按钮<input type="reset" value="必须设置值"/>  否则浏览器之间有兼容性问题.恢复刷新后的默任状态.
​	3,普通按钮,2种方式<input type="button" /> 或者 <button><button />
用户体验细节:刷新后想让第一个输入框默任选中状态,可给其设置属性  autofocus="autofocus"

### 7节  css

​	html属性写法  属性="属性值"
​	css属性写法   属性:属性值;

### 8节 实体化,标签选择器

​	实体化3属性:width, height,background
​	标签选择器 :p, div等直接用标签选择

### 9节 id和class选择器

##### css样式

​	3种css样式比较:
​	1,内嵌式 (style标签放在head中)
​	优点:方便书写.电商网站的首页必须使用这种方式,因为电商首页要求加载速度必须快,内嵌式比外链式快一些.
​	缺点:html和css代码没有实现分离,不方便修改
​	
​	2,外链式(通过link标签把外部的css文件引入到html中)
​	优点:实现了代码分离,方便修改和管理.
​	缺点:运行速度比内嵌稍慢.

​	3,行内样式
​	这种形式一定不要用,它会让代码量变得非常庞大,不方便修改.

##### 基础选择器权重

​	id > class > 标签选择器

# 5天 css第2天

### 2节 后代选择器

后代选择器: 用空格来连接, 代表的意思是找到后代元素.
后代可以是儿子,孙子等
并集选择器:用逗号来连接选择器,代表这些元素同时被选中.

### 3节 指定标签式

格式为标签.类名   类名下的标签为儿子

### 4节  高权重对比

1,引入方式css样式对比:
外链和内嵌权重相同,先写的会被后写的覆盖
内嵌权重最大,如果想要覆盖它,就只能给样式中添加!important来把权重提高.
2,复合选择器权重:
 id >  class > 标签选择器
如果综合起来权重一样,先写的会被后写的覆盖.

### 5节 css常用属性

font-weight:bold;   font-weight:normal;
font-style: italic; 字体倾斜 normal 
text-decoration: none;  没有下划线    text-decoration: underline; 下划线
word-break:break-all;  强制换行
:hover  鼠标悬停

### 6节 行高属性

行高:一行文字的结束到上一行文字结束的间距, line-height: mmpx;

### 7节  边框属性

border: mpx solid red;
boeder-left(top,right,bottom)
注意:边框属性只有实线(solid),虚线(dashed)是没有兼容性问题的.   其他方式的线都会有不同程度的兼容问题,如果程序员使用了,一定要报错!

### 8节  css盒模型的组成

盒模型的组成=盒子的宽,高 + 内边距(内容到边框的距离) + 外边距(盒子和盒子之间距离) 

### 9节 html5新标签

header 头部
nav 导航
aside  侧导航
article  文章块
footer  底部
注意:这些html5新标签只能使用在手机网站中,可以提升搜索引擎对网站的优化,不能在pc端,因为ie低版本不识别这些新标签.

### 10节 ps操作

在测量行高时,间距可以有3px左右的误差.

------


 # 2天linux 
#### 1-3小节 ####

​	操作系统:主要作用是管理好硬件设备,并为用户和应用程序提供一个简单的 接口.

​	linux目录:

​		/  表示linux操作系统的根目录,最顶层文件夹

​		/home 表示所有普通用户的家

​		/home/admin 表示admin用户的家

​		/root 表示管理员root用户的家
#### 4节开始linux命令的基本使用 ####

打开命令行方法:   桌面右键------在终端中打开

​				法2  在文件夹下-----右键------在终端中打开

基本命令:

​	cd    	去指定的目录

​	绝对路径      以根目录开头,如 /home/admin

​	相对路径      以当前目录为准,回到上级目录,或者进入下级目录,  如 														         cd admin  表示进入到当前目录下的admin文件夹   cd ..表示返回到当前目录的上一级目录

​	cd .   表示当前目录

​	cd ~   表示进入到当前用户的家目录,即  /home/admin

​       cd-    表示进入到上一个目录,相当于回看

​	pwd    查看当前目录

​	

Ls命令    是list的简写,作用为列出目录的内容.类似于dos下的dir命令

linux中,  . 代表当前目录   .. 代表上一级目录     以 .  开头的文件为隐藏文件,需要用  (空格)-a才能显示.

ls -lah  其中,参数  -a  为显示指定目录下所有子目录与文件,包含隐藏文件.a 为all

​			参数 -l 为以列表方式显示文件的详细信息

​			参数-h为配合 -l ,以人性化的方式显示文件大小.

在linux系统中,同样允许通配符来同时引用多个文件名.特殊字符称为通配符.

*代表文件名中所有字符

ls te*  查找以te开头的文件

ls  *doc   查找结尾为html的文件

?  代表文件名中任意一个字符

ls ?.c  只找第一个字符任意,后缀为.c的文件

ls a.?  只找只有3个字符,前2个字符为a.   最后一个字符任意的文件

[]   这个中括号将字符组括起来,表示可以匹配字符组中的任意一个.  -  用于表示字符范围.

[abc]  匹配a  b  c  中的任意一个

[a-f]  匹配从a到f范围内的任意一个字符

ls [a-f]*   找到从a到f 范围内任意一个字符开头的文件

ls a-f    查找文件名为a-f的文件,当 -  处于方括号外,则失去通配符的作用.

\   如果要使通配符作为普通字符使用,可以在其前面加上转义字符.但 ? 和 * 处于方括号内时,不用使用转义字符就失去通配符的作用.

ls \*a   查找文件名为  *a 的文件.

2,  清屏 clear

clear作用为清除终端上的显示(类似于dos中cls作用),快捷键为ctrl  l   (l为L的小写)

3,切换工作目录  cd

在使用linux中,经常需要更换工作目录.    cd命令可以帮助用户切换工作目录.  linux中所有的目录和文件名大小写敏感.

cd后面可以跟绝对路径,也可以跟相对路径.  

如果省略目录,则默任切换到当前用户的主目录.  cd~

用户登录的时候,默任的目录就是用户的主目录.

 cd~  切换到当前用户的主目录(/home/用户目录)

cd.     切换到当前目录

cd..     切换到上级目录

cd -       进入到上次所在的目录

注意:如果路径是从根路径开始的,则路径的前面需要加上 /  如  /mnt

通常进入某个目录的文件夹,前面不用加   /

4,显示当前路径   pwd

使用pwd命令  可以显示当前的工作目录,该命令直接输入pwd即可.后面不带参数.

5,创建目录 mkdir





9,创建文件   touch

用户可以通过touch来创建一个空的文件.如   touch  hello.txt

说明:1,会在当前路径下创建名字为hello.txt的空文件

2,linux系统没有严格的后缀格式,所以创建文件时可以命名为任意的文件名.



ctrl   shift   +      放大终端窗口的字体显示

ctrl -      缩小终端窗口的字体显示

按上/下箭头可以在曾经使用过的命令之间来回切换

如果想要退出选择,并且不想执行当前选中的命令,按 ctrl  c

------



## 第二阶段  测试理论 01

#### 01 了解测试模型

一,v模型

开发和测试阶段划分比较清晰

需求分析,概要设计,详细设计,编码,单元测试(独立的模块测试),集成测试(模块联调),系统测试(整体流程),验收测试(验证是否满足需求)

优点:包含了底层测试(单元测试)和高层测试(系统测试).  阶段划分清晰,方便工作的整体把控.

缺点:测试阶段比较靠后,之前的问题已经产生,修改不方便,  v模型是瀑布流模型的变种. 如果需求发生变化,必然要发生返工.

二,w模型

开发一个v,测试一个v,开发和测试并行.

1,开发v(需求分析     ,概要设计,     详细设计  ,编码,  集成,   实施,       交付)

2,测试v(系统测试设计,集成测试设计, 单元测试设计, 单元测试, 集成测试,系统测试, 验收测试)

优点: 开发伴随着测试并行,需求和设计一样要进行测试;   尽早的介入测试,会更早的发现问题,降低修复成本;  阶段依然明显,方便整体流程的把控.

缺点: 代码依然在测试之前,不方便代码的测试工作.如果没有文档,根本无法进行w模型,      对于人员要求较高.

#### 三,软件测试分类

##### 按阶段分类

1,单元测试(模块测试)

2,集成测试(组装测试)

3,系统测试(功能,性能, 兼容性)

##### 按是否查看源代码分类

黑盒测试: 不看源代码

功能测试:逻辑,界面,易用性,安装,兼容性

性能测试:一般性能测试,稳定性测试, 负载测试, 压力测试

黑盒测试能发现的错误:

1,功能不对或功能遗漏

2,界面错误

3,数据库访问或者处理错误

4,性能问题

黑盒测试的缺点

1,不能测试程序内部特定部位

2,如果程序未执行的代码无法发现

3,不可能做到穷举测试

##### 按是否运行程序

1,静态测试(看文档,看代码,不运行程序)

2,动态测试(实际运行代码)

##### 是否自动化

人工测试   手工测试

##### 其他分类

1,回归测试  2,冒烟测试           3,随机测试(测试重点模块或者之前出现过问题的模块)

4,验收测试: 内侧版本(alpha),内部人员测试,或者有很少一部分用户.此阶段要解决严重的问题

公测版本(beta),所有用户都可以免费使用,通过用户的反馈修复软件的细节.

准正式版(gamma),跟正式版几乎一样

#### 测试用例

##### 等价类划分法  

 把无法穷举的数据分类书写

步骤: 1,按照需求写出有效等价类    2,根据需求取反,写出一部分无效等价类

3,找到特殊情况的无效等价类(中文,英文,空格,空,符号,小数,是根据需求来选择)

##### 等价类划分小总结

1,长度  2,组合  3,类型   4,是否为空    5,是否区分大小写(根据需求来定,一般大小写会区分)     6,空格问题(程序中  文字的最前和最后的空格,程序员喜欢清除,文字中间的空格会保留)

------



## 测试理论02

##### 边界值的方法和总结

边界值和等价类配合使用.   边界值取比边界值大一点,小一点的值都要测试到位.

##### 因果图制定判定表

##### 场景法

基本流:正确的业务流程

备选流:有问题的业务流程

测试用例的书写:只需要把需求文档的每一条当作一个测试用例即可.

比如一个登陆框,产品经理把每一种情况都列出来,他如果不列,程序员有可能不写.用户体验就不好.产品经理把基本的基本流,备选流就是测试员的测试用例.只要程序员写的和产品经理有冲突,就提bug

每一条场景,就是一条测试用例.

##### 流程法

测试用例必须包含所有的分支条件,每一个分支条件就是一条测试用例.

##### 错误推断法

当时间紧,任务急的时候,测试时间较少,可以考虑使用错误推断法来设计测试用例.根据测试人员以往项目经验来设计.

已经经过了几轮测试后,也可以用推断法进行测试用例的补充.

------



### 测试理论03

##### 正交表

当要**测试的内容,需要排列组合的情况非常多**的时候,我们要考虑使用科学的方法来减少测试用例的个数,这个方法就是正交表.

特点:均匀分散  齐整可比(所有的情况都应该均匀的被测试过一次)

如何查询正交表:

因素:控件的个数

水平:控件里面选项的个数

1,先确定几因素,几水平

2,在"常用正交表"中找到合适的表格

3,复制找到的表格到我们自己的表格中

4,自己再写一个对照表,

5,把复制过来的表格和对照表实现映射关系,就可以得到正交表(测试用例)

注意:如果没有找到合适的正交表,要在表格中找到多一点的表即可,只需把多余的内容删除.

##### 正交软件使用步骤

1,文件---新建工程

2,实验----新建实验

3,设计向导------实验说明,选择正交表,因素与水平都需要填写,类型选择   标准正交表

4,输出  ----保存RTF(word文档)      保存CSV(excel文档)

##### allpairs混合正交工具使用步骤

正常的正交表使用正交设计助手软件或常用正交表  比较方便

混合正交表allpairs可以制作正常正交表,也可以做混合的,但是不方便.

allpairs使用步骤

1,使用excel制作对照表,不要写编号

2,复制表格中的所有所有数据放在一个txt文本中,格式千万别动

3,把此txt文档放在allpairs文件夹中

4,win +r 输入cmd,打开命令行窗口

5,找到工具所在的文件夹

6,输入此行代码即可   allpairs.exe spsx.txt>spsxchenggong.txt      (其中ren.txt是我们复制过来的文本文件,  renchenggong.txt存放的是最终结果,不用事先 建立好))

7,找到最终建立好的txt文件如renchenggong.txt ,打开后,复制第一大段内容到excel表格中,(如果遇到 - - ,代表此选项随意选择,我们根据齐整可比理论,均匀选择即可)

##### 软件缺陷 ---性能问题

首页打开的速度---页面加载速度

网站图片的完美压缩---清楚内存站的小

侧边导航栏分类中的文字--文字多的时候不会换行,影响下一行.

### 测试理论第三天

##### 复习:   软件缺陷的状态

1, 提交      缺陷刚刚提交到系统上

2,打开        此缺陷正在被修改中,等待处理

3,拒绝         程序员认为此问题不修改

4,修复          程序员修改了代码,又提交后的状态,测试员必须进行回归测试

5,关闭             回归测试后,确认没有问题

6,推迟            此问题放在后续版本解决,由经理开会决定

(网站刷新的时候ctrl +  f5,为清除缓存刷新 )

##### 缺陷严重程度划分

1   表面错误 

2  影响独立模块,断断续续的问题,特定条件才发生,与产品要求不一致

3   功能点没有实现,数据丢失

4 5  影响了系统或者出现了严重的计算错误

##### 02节  软件缺陷优先级

1, 最低优先级      只要时间允许才去修复

2,低优先级         不延迟发布,可以在后续来修复

3, 高优先级     影响其他开发或者测试工作的进行,必须在发布之前修复

4    5    根据公司规定不同,最高优先级   严重影响系统

注意: 优先级和严重程度不是绝对的正比关系

##### 缺陷报告细节

一个缺陷报告只能有一个缺陷的描述

2,缺陷一定要保证可以复现

3,复现缺陷的步骤要写清晰,一个编号写一个步骤(有些不重要的步骤可以整合)

4,描述结果(bug产生的效果)和期望结果(希望程序员要如何改正)

5,避免使用强调符号和俚语,正常描述问题即可.

6,使用术语描述问题,不要使用"似乎""好像"等模糊词

##### 缺陷密度

每千行代码出现的缺陷个数

##### 常用的寻找缺陷的方法

页面大小

​		在b/s结构的软件系统中,当一个页面元素太多,未作精简时,在打开该页面时可能需要较长的加载时间,这对于软件性能是一个不小 的影响,既增加了服务器的压力,又容易引起用户的反感.

比如:

图片未经压缩,格式不正确.

代码冗余,存在太多无用代码

页面元素太多,太过复杂.

容错处理(功能缺陷)

容错处理在软件系统中占据十分重要的地位.容错,就是容忍错误的能力.当用户在使用软件过程中发生错误后,软件应该给出引导信息,指引用户进行正确的操作.

比如     1,用户输入错误,系统无提示,无响应,用户不能清晰知道系统不处理的原因.

​		2,给出信息提示,用户接受后无法继续操作,不给用户"改过自新"的机会

​         	3,用户输入不合法的信息后,系统给出提示,用户确定后,系统仍能处理错误的信息.

​		4,取消功能不能取消.比如删除,系统给出提示,是否确定删除,用户否认后,仍执行了删除.

##### 性能缺陷

这类问题在平常做黑盒测试就能发现

比如  1,打开文档,10s应该完成,却花了3分钟

​	2,启动软件,cpu长时间100%,内存消耗过多

​	3, 5个用户可以正常使用,20个用户使用时系统崩溃

​	4,打开一个登陆页面花了1分钟

​	5,完成一个查询功能,花了2分钟

### SVN简介,<u>从13节往后再过一遍.</u>  

SVN是一个开源的版本管理软件.

------

### 项目实战01天

### 01-08环境搭建过一遍  

##### 09节 项目背景调研

熟悉被测系统,可从3方面: 项目的背景调研    绘制组织架构图  编写测试范围列表

项目背景调研包括项目进展,项目复用程度,项目已有成果物,开发人员

项目进展------a,未开发       b,开发中		c,开发完成

项目复用程度----------a,全新的项目         b,复用部分 代码            c,复用全部代码

项目已有成果物--------A 产品 ----a,需求说明书    b,UI/UE设计图

​			---------B开发-----a,概要设计文档    b,详细设计文档      c,源代码     d,数据库设计文档       e,软件

测试------------a,测试计划    b,测试方案    c,用例       d,缺陷   e,总结报告

##### 10节    绘制组织架构图

绘制组织架构图的目的是从整体理解被测软件

项目-------子系统们-------小模块们 

梳理到模块级别,不用到功能点

##### 11节 编写测试范围列表

目的是弄清楚被测模块的具体功能

统一模板:     功能点的编号       功能点的名称	功能点的测试类型		PATH	优先级

##### 12节 测试计划和方案

测试计划的作用是告诉团队所有的人,是怎么安排测试的.

测试计划编写6要素:

1,为什么要进行这些测试

2,测试哪些方面,不同阶段的工作内容

3,测试不同阶段的起止时间

4,相应文档和缺陷的存放位置

5,项目有关人员组成,安排哪些测试人员进行测试

6,如何去做,使用哪些测试工具以及测试方法进行测试

测试计划的内容:

1,测试目的

2,测试范围

3,测试资源

4,明确测试组织和岗位职权

5,测试轮次确定和时间的安排

6,测试方法简述

7,测试标模板

##### 测试方案

测试方案的作用是指导测试人员进行具体测试规则的技术文档

内容:

1,测试策略

2,测试发布标准

3,测试风险分析  (需求,流程,测试)

4,测试实体标准的制定

##### 测试用例优先级:

P0:冒烟测试用例,一般为保证软件中最主要的功能,最基本的流程能正常运行而设计.

P1: 次要功能,小功能

P2:UI,边界,错误的设置

P3:错误信息,较复杂的场景,不常用的场景

缺陷的严重等级说明:

A:  严重影响系统运行的错误

B:功能方面一般缺陷,影响系统运行

C: 界面布局不美观或轻型错误

D:合理化建议

##### 缺陷状态:

new    新建

open	打开

fixed	修复

rejected	拒绝

assigned	已指派

postponed	延期

reopen   再次打开

------

### 项目实战03天

##### 测试用例设计方法

测试设计方法:   测试需求分析          测试点            测试用例

功能点  :   输入----可见输入------长度,类型,组成规则,是否重复,是否为空

​		处理-----a正常处理----正确数据+正确操作

​				b异常处理----正确数据+错误操作

​							错误数据+正确操作

​							错误数据+错误操作

​							正确数据+正确操作+异常环境

​		输出-----a可见输出---前台,后台

​				b不可见输出---数据库

以后的工作中,测试用例是写在测试管理工具中.自动生成唯一的测试ID

首页:数据校验(商品分类,楼层,楼层数据)

设计数据库表查询

1,	确定功能对应的数据库表

2,编写对应的sql

3,写测试用例

轮播图: 分析实现的细节

测试用例:优先级   测试用例标题   前置条件    操作步骤  测试数据   预期结果    实际结果

------

项目实战03天

bug类型: 代码错误    需求设计	环境部署		性能相关

用户,系统,第三方支付的流程:

1,用户向系统发起支付请求,

2,系统处理请求,生成支付订单

3系统向第三方发起付款请求

4,第三方校验后,向用户生成支付界面

5,用户输入密码,确认支付

6,第三方校验密码无误,进行扣款, 支付成功

7,返回系统,支付成功消息

8,系统向用户生成付款成功页面,并更新订单状态

------

### 项目实战4天

业务场景:深度图,广度图

质量模型: 功能性  		效率	可移植性		可靠性	易用性	可维护性

效率(性能):    a时间维度(响应时间)                        b资源利用率

可靠性(安全性): 数据加密   用户权限    SQL注入

可移植性: 兼容性(适配性)   web系统   移动端app测试

易用性: UI界面和交互 --->

web项目:a浏览器    b,web服务器     c, http协议

http协议的协议: 客户端和服务器通信实现细节

网络模型: a 应用层    http协议

​		b,传输层     TCP协议/UDP协议

​		C,网络层      IP协议

​		d,物理层

### 9节  httpwatch未安装

##### http协议的状态码:

  1**: 信息,客户端继续进行接下来的操作

2**:成功

3**: 重定向

4**: 客户端请求的资源路径错误

5**:服务端错误

##### http请求格式:

请求行,请求头,空行,请求内容,

##### http响应格式:

响应行,响应头,空行,响应内容

##### http1.1版本特性:

保持连接:即http请求和响应,先在客户端和服务端建立tcp连接,不会完成一次http请求响应就关闭,可以在一次tcp连接上完成多次http请求和响应.

##### http的get请求和post请求区别:

get请求:更多向服务器下载资源

​	get参数出现在url,	安全性弱	,参数数据只能是字符串, 参数的数据量小

post请求:更多向服务器提交数据

​	post请求参数出现在请求正文,  安全性好  参数数据可为任意类型    参数数据量大



##### httpwatch包含的内容:

 time :本次请求的响应时间

sent:客户端发送的数据大小

received: 服务端返回的数据大小

result:状态码

type: 资源类型

url:资源地址

### 项目实战05天

##### 002节兼容性问题

###### 移动端APP测试   

平台有ios,     android

操作系统版本  ios:   8,9,10,11                 android:4.4及以上

分辨率:

不同的分辨率,app在页面上展示是有差异的.  测试的时候,市面上常见的分辨率都应该覆盖到.比如720,1280,2k的屏.

厂商: 

 安卓在底层是linux的操作内核,苹果是自己的一套内核.所以安卓的内核是开源的.安卓的厂商会在出厂之前做一些改动.安卓手机的测试会对手机版本做一些覆盖.

网络兼容:

pc端网络较为稳定    移动端会在wifi,弱网情况,4g,    网络的切换  不同的运营商

##### 面试

移动端测试适配哪些机器:?   从 几种机型(5-6种,已经上线的产品,开发人员会进行埋点,即统计当前下载app的用户的手机机型,根据一段时间的统计,分析出排名靠前的用户使用的机型.测试人员在测试的时候尽量覆盖这些机型.如果产品未上线,可通过现有市场占有率的机型),机型分辨率,操作系统版本,厂商..........

### 03节 fiddler安装  未安装

抓包工具:   

httpwatch   兼容性有限

wireshark      功能强大

fiddler    .net平台上,功能强大

charles   mac平台上,功能强大

fiddler的官方网站    www.telerik.com/fiddler

##### 05节  接口介绍

接口分为内部接口,外部接口

内部接口:  软件内部功能,模块调用的实现

外部接口:软件与第三方对接功能. 比如通过登录qq,微信登录来获取校验  通过跳转到支付宝,微信进行支付

##### 柠檬班fiddler讲解  

抓包:将网络传输发送与接收的数据包进行截获,重发,编辑,转存等操作,也用来检查网络安全.抓包也经常被用来进行数据截取等.

fiddler抓包判断是前端还是后端bug:    a,浏览器f12进行简单的调试. b方法,通过fiddler截获的数据包判断,

##### 06节 

fiddler截取浏览器发送给服务器的数据,冒充浏览器发送给服务器;服务器返回的数据,也会被fiddler截获,经fiddler返回给浏览器.是web服务器代理的形式. fiddler默任的ip为本机的 127.0.0.1,端口为8888

##### fiddler移动端抓包 操作一遍

##### 07节  fiddler获取(get/post)请求的过程

1,启动fiddler 	2,确保工作在抓包状态		3,使用浏览器输入访问地址		4,fiddler会话列表中点击需要查看的请求		5,在右侧inspectors面板下点击raw

##### 08节 构造http请求

##### 09节  打断点







### ALM安装

##### 00节    ALM简介

企业中,测试产出物写在工具中,不是excel表中.





### 禅道

##### 00节  禅道简介

禅道主要用于项目管理: a,产品管理  b,项目管理  c,质量管理

开发模型:瀑布和敏捷

瀑布模型,银行用的多: a,文档驱动,即要求每个阶段产生一个明确的文档.

​	b,阶段划分明确,每一个阶段的工作开始必须以前一个阶段的产出为准入.

​	c,适合需求明确且稳定的项目开发

敏捷模型,互联网企业用的多:  a 以人驱动,弱化了文档的需求.

​		b,快速迭代,每次迭代都会产生一个可用的软件产品(2周更新一个版本属于正常)

​	敏捷开发的技术手段: a,xp-->极限编程

​					b, scrum -->禅道思想

​					c,tdd--->测试驱动开发

​					d,ci---->持续集成-->自动化

自动化,持续集成实例: 1,每天开发提交代码,自动进行全项目的编译      2,定时在每天晚上,进行自动打包      3,代码合并后,自动完成单元测试,接口测试,冒烟和回归UI自动化测试脚本     4,自动发送测试报告邮件,发送对应的人员.    备注:jekins工具可完成持续集成

##### 01节 禅道安装,未安装

##### 02节  禅道流程图详解

------

### 第三阶段  python基础

##### day01

pycharm安装需要激活码,python的编译器,电脑需要安装python,

##### python中的变量类型

numbers(数字):   int(有符号整型),	long主要用于8进制,16进制)		float(浮点型)		complex(复数)

string(字符串)

list(列表)

tuple(元祖)

dictionary(字典)

python中,单引号和双引号是不区分的.

##### 标识符

Python标识符的规则:由字母,下划线,数字组成且数字不能开头.,混搭或单一的形式都行,标识符是区分大小写的.

3种常见的命名规则:1,小驼峰命名  2,大驼峰命名  3,下划线

##### 格式化输出

```python
my_age = 20
my_name = '小明'
print('名字是: %s' % my_name)
print('小明今年%d岁' % my_age)
my_height = 160.12
print('小明身高:%.2f' % my_height)
# 格式化输出bool类型,法1. %s 把布尔看成字符串类型   法2 %d 把布尔类型看成数字类型
is_boy = True
print('是男孩吗:%s' % is_boy)
# 换行符  \n
```



##### 换行符 \n

```python
print('hello\npython')
```

\n前后不带空格,类似于空格键的效果

\t 制表符   类似于tab键的作用

##### 输入

python2版本, input输入,你输入的是什么类型的值,输出的就是什么类型.  raw_input不论输入什么,输出的都是字符串.

python3版本中,只有input输入,用法同raw_input

##### 运算符

取整除 //   9//2  为4

取余 %    9%2 为1

指数 **   10 **2为100

##### 数据类型转换

int(x)  将x转换成一个整数

float(x)  将x转换成一个浮点数

str(x)   将x转换成一个字符串

一般能复制就不要手敲,以防敲错.

python中,对缩进要求很严格

------

##### day02 

##### If 语句

1,满足某些条件,才能做某件事情.条件不满足,则不能做

2,if语句的代码块指和if语句有缩进的部分.代码的缩进为1个tab键

2,if 语句只说明了分支结构的一种情况

比较运算符就是对比2个数的大小关系.比较运算符和if搭配,如果条件为true,则可以进入if条件语句中,如果条件为false,则不能进入.

##### elif

1,elif必须和if 一起使用

2,else 一般用在最后,即所有条件都不满足时使用

3,python中只能用elif,不能用 else if

##### if语句的嵌套

if语句的嵌套,和分析的逻辑一样写,注意逻辑层次的划分.

##### while循环

1,定义一个变量,记录循环次数

2,while判断条件,如果条件满足,则执行代码

3,对变量的值进行修改,之后再次进行循环

注意:

1,while循环中,如果不对变量进行操作,容易死循环.死循环太浪费设备性能.

2,一般情况下,需要多次重复执行的代码,都可以用循环的方式来完成

3,为了提高代码的重复使用率,开发者都会采用循环

4,while循环内部的代码需要进行缩进,

##### while 嵌套

1,while循环嵌套:外面的循环执行一次,内部循环会执行n次,一直到执行完毕,再执行外部的循环.

2,无论是内部的while循环还是外部的while循环,都需要定义一个变量,作为循环次数的记录

3,内部while和外部while都需要对变量进行累加操作,以保证循环次数的减少.

注意:不换行在python3版本是end=''     在python2版本是在首行添加  ,    就行.

```python
print('bu'),
print('huanhang')
```

结国就是 buhuanhang

##### day3 

注意:本文件夹从第5节字符串开始,前面的几节有时间看一遍

##### 5节字符串的介绍

字符串的形式: 第一种 '字符串内容'   第二种  "字符串内容"

第三种,多行注释的写法,  '''字符串内容''',  此法能够保留换行,空格及空行.单双引号都行.

##### 6节字符串输出,输入

输出 print(字符串名)

输入  input()  如  input('姓名: %s' % name)

查看字符串类型 type()

查看字符串长度  len()

##### 7jie字符串的下标和切片

```python
字符串的下标索引,从左往右:0,1,2,3.....  从右往左:-1,-2,-3,.....
```

切片写法   变量名[起始位索引:结束位索引(不包含):步长],  左边闭合,右边开(结束的索引不包括).字符串是不可变的,切片只是截取字符串的一部分.

下标是获取字符串的一个字符.  切片是获取字符串的一部分

字符串无论怎么切,原字符串都不改变,只是复制出来新的字符串

字符串切片可以从左侧也可以从右侧进行,相应的索引值不同:

从左侧进行,索引值为0,1,2,3

从右侧进行,索引值为-1,-2,-3....从右侧进行切片的时候,需要注意步长也为负数.



```python
range = 'abcdefg'
#下标
print(range[-1])
#切片abc
ret0 = range[0:3]
print(ret0)
#切片ace
ret1 = range[0:5:2]
print(ret1)
```

##### 10jie 字符串的常见操作

```python
names = 'lili lucy nancy'
ret2 = names.find('lu')
print(ret2)
#输出的是lu的第一个字符l的索引
```

find()方法,index()方法相似,都是查目标的索引,区别是find()方法中,要查找的字符串不存在,输出会返回-1,而index()方法直接报错.

##### 15节 列表

列表的格式  列表名 = [元素1, 元素2,....]

空列表的定义: my_list = []    或  my_list = list()

列表是一个容器,能够容纳各种数据类型,

列表索引从左往右为0,1,2,3.....  从右往左为-1, -2, -3....

列表的相关操作,增删改查

A: 添加元素append  extend,insert

列表名.append(元素)  此法添加的元素为任意类型,最终的列表为原封不动的在后边添加.

列表名.extend(元素)    此法添加的元素为可遍历的,字符串,列表.添加到列表中为遍历的.

列表名.insert(要插的索引,元素)

B:修改元素 列表名[要修改的索引] = 目标元素

修改元素只需先获取,后赋值修改

根据下标索引来获取元素

C:查找

查找2种方法,in,not in    另一种count和index结合

D:删除

del,pop,clear

------

##### day4元祖,字典,函数

##### 2节 列表的排序

升序:  列表名.sort()                        降序:   列表名.reverse()

列表嵌套:列表里包含列表

##### 元祖

元祖名 = (元素1,元素2....)    元祖里面的元素是不能修改的

##### 字典

my_dict = {key1: value1, key2: value2.....}

字典和列表一样,也能存储多个数据,且数据类型没有要求

字典中找某个元素时,是根据'名字'(就是冒号前面的那个值,也叫键)

字典中的每个元素由2部分组成,  键:值

一般情况下,字典里的键是不能重复

##### 字典的常见操作

字典和列表是可变的.    字符串和元祖是不可修改的

只有字典是按照键查找元素.    字符串,列表,元祖都是根据索引来找元素

##### 10节 公共方法的总结

1)开闭区间的总结

随机数:

import random

random.randint(1, 10)    取值范围[1, 10]

range范围:

range(1, 10)   取值范围[1, 10)

切片

a = 'itcast'

a[起点:终点(不包含):步长]

##### 函数

所有面向对象的语言都有3个特征:封装,继承,多态

函数的出现解决了多次重复某一部分代码的问题

函数往往是某个功能的集合

函数就是个代码块

函数的定义:  函数代码块以def开头,后接函数名和():                  函数内容必须要缩进

函数的调用:          函数名()

##### 函数的文档说明

给函数加注释,说明当前函数的主要功能,参数作用,返回值情况

------

##### day5 

##### 函数的返回值

```python
#下面是个递归函数
def deep(num):
    print(num)
    if num == 20:
        return
    num += 1
    return deep(num)
deep(2)
```

```
return:
return 数据m  代表返回数据m
return       代表结束函数
```

函数可以有返回值,也可以没有

程序读取到return关键字后,就会退出当前的函数体,即return之后的代码将不会执行

return后面有内容,则返回return后面的内容,如果单独写一个return,则返回none,函数不在往下执行.

有时候,我们会把return当成跳出当前函数的方式来使用,而不是用它来返回内容.

下面这个情况,return都会被调用到:

```python
def scoreLevel(score):
    if score >= 90:
        return('优')
    elif score >= 80:
        return ('良')
    else:
        return('中')
print(scoreLevel(93))
```

```python
def fun22(a, b):
    ret = a + b
    return(a, b, ret)
ret2 = fun22(20, 50)
print(ret2)
```

##### 4种类型的函数

```python
#1,无参数,无返回值
def print_func():
    print('*********')
print_func()
#2,无参数,有返回值
def pi():
    return 3.14
yuan = pi()
print('祖冲之发现的圆周率为:%.2f' %yuan)
#3,有参数,无返回值
def fun3(name):
    print('你的名字:%s' %name)
fun3('lucy')
#有参数,有返回值
def sumTo(num):
    sum = 0
    for i in range(num):
        i += 1
        sum += i
    print(sum)
sumTo(100)
def sum2(num):
    i = 1
    sum = 0
    while i <= num:
        sum += i
        i += 1
    print(sum)
sum2(100)
```

##### 函数的嵌套

调用某个函数,此函数必须写在调用之前.

一个函数中可以嵌套无数个函数

函数可以连着进行嵌套

```python
def getNo():
    index = input('请您输入编号:')
    #根据编号,获取家长姓名
    name = getName(index)
    #根据家长姓名,获取学生姓名
    cName = childName(name)
    #根据学生姓名,获取学生成绩
    score = childScore(cName)
    #查等级
    scoreClass(score)
def scoreClass(score):
    if score >= 90:
        print('excel')
    elif score >= 80:
        print('liang')
    elif score >= 70:
        print('normal')
    elif score >= 60:
        print('cha')
    else:
        return 'bujige'
def childScore(cName):
    if cName == '小王':
        return 90
    elif cName == '小孙':
        return 80
    elif cName == '小马':
        return 70
    elif cName == '小朱':
        return 80
def childName(name):
    if name == '老王':
        return '小王'
    elif name == '老孙':
        return '小孙'
    elif name == '老马':
        return '小马'
    elif name == '老朱':
        return '小朱'
def getName(index):
    if index == 301:
        return '老王'
    elif index == 302:
        return '老孙'
    elif index == 303:
        return '老马'
    elif index == 304:
        return '老朱'
    else:
        print('输入的编号错误')
getNo()
```

##### 函数参数

位置函数:形参,实参一一对应

关键字赋值: 

```python
def fun1(a, b):
    result = a - b
    print(result)
fun1(b = 20, a = 10)
#运算为10-20
```

缺省参数

```python
缺省参数,缺省参数只能放在最后一位参数
def class_1(name, no, sex='女'):
    my_name = '姓名是%s' % name
    a = my_name.decode('utf-8')
    my_no = '学号是%d' % no
    b = my_no.decode('utf-8')
    my_sex = '性别是%s' % sex
    c = my_sex.decode('utf-8')
    print(a, b, c)
class_1('lucy', 301,)
class_1('nancy', 302,)
class_1('mike', 303, '男')
```

##### 拆包

拆包:直接获取里面数据的过程

对元祖,列表,字典等都可以拆包,拆包获取的是value值,但字典获取的是key值

拆包时,需要拆的数据的个数要与变量的个数相同,否则程序会异常

```python
#交换a,b两个数的值
a = 1
b = 2
a, b = b, a
```

##### 函数的局部变量

局部变量:定义在函数内部的变量(变量在def函数名:    下面,并且有缩进)

局部变量的作用范围是这个函数内部,即只能在这个函数中使用,在函数外部是不能使用

不同的函数可以定义相同名字的局部变量

局部变量的作用是为了临时保存数据,需要再函数中定义变量来进行存储

当函数调用时,局部变量被创建,当函数调用完之后这个变量就不能够使用

##### 函数的全局变量

全局变量:变量在一个函数中使用,也能在其他的函数中使用

在函数外边定义的变量叫全局变量

全局变量在所有函数中都能被调用

##### 匿名函数

匿名函数:用lambda关键词创建小型的匿名函数.

简单的函数用匿名函数

写法为 lambda参数名:函数体

 调用方法    函数名 = lambda参数名:函数体    调用时 函数名(实参)

------

##### day6

前两节回顾有时间看一下

##### 3,列表推导式

列表推导式,指的是轻量级循环创建列表

```python
list1 = [item for item in 循环体]

my_list = [x*2 for x in range(10)]
print(my_list)
list2 = [x for x in 'hello' if x != ' ' and x != 'l']
```

##### 文件的操作

##### 4节 文件的写入, 读取

```python
f = open('day6_1.txt', 'w', encoding='utf-8')
str = '''既然你问了,
那我就告诉你,
为了防止世界被破坏!!!!
为了守护世界和平~~~~
'''
f.write(str)
#关闭文件
f.close()
```

w权限:如果文件不存在,那么创建.  

如果存在,那么就先清空,然后写入数据

读取文件:

```
#读取文件
f1 = open('day6_1.txt', encoding='utf-8' )
content = f1.read()
print(content)
f1.close
```

```python
#readline为读取一行数据
f = open('day6_1.txt', 'r')
content = f.readline()
print('1:%s' % content)
content = f.readline()
print('2:%s' % content)
f.close()
```

readlines按照行的方式把整个文件中的内容进行一次性读取,并且返回的是一个列表,每一行的数据为一个元素.

```python
f = open('day6_1.txt')
content = f.readlines()
i = 1
for temp in content:
    print('%d%s' % (i, temp))
    i += 1
f.close()
```

```python
#coding=utf-8
old = open('file_old.txt', 'w')
str = '''我如果爱你
绝不像攀援的凌霄花
借你的高枝炫耀自己
'''
old.write(str)
old = open('file_old.txt')
result = old.read()
new = open('file_new.txt', 'w')
new.write(result)
old.close()
new.close()
```

##### 文件   文件夹的相关操作

对文件进行重命名,删除等一些操作,导入python的os模块

```python
import os
#重命名文件
os.rename('day61.txt', 'day611.txt')
#删除文件
os.remove('day611.txt')
#创建文件夹
os.mkdir('day7')
#删除文件夹
os.rmdir('day7')
#获取当前文件(即你正在操作的文件)所在的目录地址,绝对路径
path = os.getcwd()
print(path)
#改变当前文件的默任路径
os.chdir('../')
path = os.getcwd
print(path)
#获取目录列表
os.chdir('day7')
list = os.listdir('./')
print(list)

```

##### 面向对象基础

面向对象有2个重要概念:类,对象

类是创建对象的模板

类由3部分构成:类名,属性,方法(行为)

```python
class Person(object):
    # 定义方法
    def move(self):
        print('running')
    def attack(self):
        print('hitting')
#         在类里边通过self获取对象的属性
        print(self.name, self.home, self.height)
# 创建对象 对象名1 = 类名()
lucy = Person()
# 给对象添加属性,以及对应的属性值
lucy.name = 'lucy'
lucy.home = 'hangzhou'
lucy.height = 170
lucy.look = 'pretty'
# 通过.成员选择运算符,获取对象的属性值
# lucy.home,  lucy.height,  lucy.look
print('人物 %s 的家在 %s' % (lucy.name, lucy.home))
print('人物 %s 的身高是 %d' % (lucy.name, lucy.height))
print('人物 %s 的外表是 %s' % (lucy.name, lucy.look))
# 通过.成员选择运算符,获取对象的方法
lucy.move()

```

##### 魔法方法之__init__()

innit方法前后都有__    在python中,以__开头,__结尾的方法,称为魔法方法

innit方法,在创建一个对象时默任被调用,不需要手动调用

innit中的self参数,不需要开发者传递,python解释器会自动把当前的对象引用传递过去.

python可以通过这些魔法方法监听我们创建对象的进度

```python
class ShuCai(object):
    # init用来做变量初始化或赋值操作,在类实例化对象时会被自动调用
    def __init__(self, new_name, new_color, new_shape):
        self.name = new_name
        self.color = new_color
        self.shape = new_shape
        print('%s 的颜色是 %s' % (self.name, self.color))
        print('%s 的形状是 %s' % (self.name, self.shape))
        # 普通实例方法
    def move(self):
        print('风吹叶子会动')
luobo = ShuCai('luobo', 'yellow', 20)
baicai = ShuCai('baicai', 'green', 40)
luobo.move()
baicai.move()
```

通过一个类,可以创建多个对象,就好比通过一个模具,创建多个实体一样

init中,默任有1个参数名字为self,如果在创建对象时传递了2个实参,那么init中除了self第一个形参外,还需要2个形参,如__init__(self, x, y)

在类内部获取属性和  实例方法,通过self获取

在类外部获取属性和   实例方法,通过对象名获取

如果在一个类中有多个对象,每个对象的属性是各自保存,都有各自独立的地址

但是实例方法是所有对象共享的.  类会通过self来判断哪个对象调用了实例方法

##### 魔法方法str

```python
class ShuCai(object):
    def __init__(self, name, color, shape):
        self.name = name
        self.color = color
        self.shape = shape

    def __str__(self):
        return '%s %s %s' % (self.name, self.color, self.shape)
fanqie = ShuCai('fanqie', 'hongse', 10)
print(fanqie)
```



> str魔法方法,没有参数,只有1个返回值,而且这个返回值必须是一个字符串
>
> ------
>
> ##### day7

##### del魔法方法

```python
class Hero(object):
    def __init__(self, name, age, sex):
        self.name = name
        self.age = age
        self.sex = sex
    def __del__(self):
        print('干掉对象,我才会被输出')
libai = Hero('libai', 30, 'man')
del libai
```

当有变量保存了一个对象的引用时,此对象的引用计数就会加1

当使用del删除变量指向的对象时,则会减少对象的引用计数.如果对象的引用计数不为1,那么会让这个对象的引用计数减1,  当对象的引用计数为0的时候,则对象会被真正删除.

##### 单继承和多继承

```python
class Master(object):
    def __init__(self):
        self.peifang = '古法制作的煎饼'
    def make(self):
        print('这是古法制作的程序')
class Tudi(Master):
    pass
DaMao = Tudi()
print(DaMao.peifang)
DaMao.make()
```

子类在继承的时候,在定义类时,小括号()中为父类的名字

父类的属性,方法,会被继承给子类

##### 多继承

```python
class Master(object):
    def __init__(self):
        self.peifang = '古法制作的煎饼'
    def make(self):
        print('这是古法制作的程序')
    def chouyan(self):
        print('老师傅爱抽烟')
class Modern(object):
    def __init__(self):
        self.peifang = '现代配方'
    def make(self):
        print('这是%s制作程序' % self.peifang )
class Tudi(Master, Modern):
    pass
DaMao = Tudi()
print(DaMao.peifang)
DaMao.make()
DaMao.chouyan()
```

多继承是继承多个父类,也继承了所有父类的属性和方法

如果多个父类中有同名的属性和方法,则默任使用第一个父类的属性和方法.

多个父类中,不重名的属性和方法,不会有任何影响

##### super

调用父类方法:

```python
def old_make(self):
    #第1种写法
    Master.make(self)
    #第2种写法
    super(Tudi, self).make()
    #第3种写法
    super().make()
```

super()在python2.3之后才有,用于通常单继承的多层继承.

子类继承了多个父类,如果父类名改了,那么子类也要涉及多次修改.而且调用也需修改,显得代码臃肿.

使用super()可以逐一调用所有的父类方法,并且只执行一次.

如果继承了多个父类,且父类都有同名方法,则默任只执行第一个父类.同名方法只执行一次.即不支持多个父类的同名方法

##### 多态

python的多态,就是弱化  类型,   重点在于对象参数是否有指定的属性和方法,如果有就认定合适,不关心对象的类型是否正确

```python
class Person(object):
    def __init__(self, name, age):
        self.name = name
        self.age = age
    def eat(self):
        print('吃饭....')
class Dog(object):
    def __init__(self, name, age):
        self.name = name
        self.age = age
    def eat(self):
        print('eating....')
lucy = Person('lucy', 15)
wangwang = Dog('wangwang', 2)
# 多态
def print_fun(object):
    print(object.name, object.age)
    object.eat()
print_fun(lucy)
print_fun(wangwang)
```

##### 类属性

```python
class Person(object):
    # 这个banji为类属性
    banji = '一年级'
    def __init__(self, name, sex):
        self.name = name
        self.sex = sex
xiaoli =  Person('xiaoli', 'boy')
# 通过2种方法访问类属性
# 法1,对象名访问
print(xiaoli.banji)
# 法2,类名访问
print(Person.banji)
# 修改类属性只能通过改类名.类属性名 = 新值
Person.banji = '二年级'
```

##### 类属性

```python
class Person(object):
    # 这个banji为类属性
    banji = '一年级'
    def __init__(self, name, sex):
        self.name = name
        self.sex = sex
xiaoli =  Person('xiaoli', 'boy')
# 通过2种方法访问类属性
# 法1,对象名访问
print(xiaoli.banji)
# 法2,类名访问
print(Person.banji)
# 修改类属性只能通过改类名.类属性名 = 新值
Person.banji = '二年级'
```

##### 类方法

```python
class Person(object):
    # 实例方法
    def move(self):
        print('正在走路中...')
    # 类方法
    @classmethod
    def run(self):
        print('跑步....')
# 类,对象均可调用类方法
# 法1
Person.run()
# 法2
lucy = Person()
lucy.run()
```

##### 类私有

```python
class Person(object):
    # 私有类属性
    __money = 100
    @classmethod
    def get_money(cls):
        return cls.__money
    @classmethod
    def set_money(cls, new_money):
        cls.__money = new_money
lily = Person()
lily.set_money(500)
print(lily.get_money())
```

```
def foo(x, *args,**kwargs):
    print(x)
    print(args)
    print(kwargs)
foo(1, 2, 3, 4, a = 1, b = 2, c = 3)
# 结果为
# 1
# (2, 3, 4)
# {'a': 1, 'c': 3, 'b': 2}
```

##### 单例模式

设计模式是为了可重用代码

单例模式目的是让  类  创建出的对象,  在系统中,只有  唯一一个实例

每一次执行   类名()  返回的对象,内存地址都是相同的,

##### 异常

```python
try:
    num = 12
    print(num)
except:
    print('发生错误...')
else:
    print('没有捕获到异常')
```

```python
try:
    num = 100
    print(num)
    try:
        print(num2)
    except:
        print('嵌套里边的异常捕获到了')
except:
    print('嵌套外围的异常捕获到了')
# 结果 100  嵌套里边的异常捕获到了
```



### 第四阶段 web自动化

火狐浏览器安装路径  C:\Program Files (x86)\Mozilla Firefox 

修改不了E:\testProgram\Mozilla Firefox

##### selenium特点

1,开源软件,源代码开放,可以根据需求来增加工具的某些功能

2,跨平台:linux,mac,windows

3,核心功能:在多个浏览器上进行自动化测试

4,多语言:java,python,js....

5,成熟稳定

6,功能强大:能够实现类似商业工具的大部分功能.因为开源性,可实现定制化功能

##### selenium IDE

selenium IDE 是一个火狐插件,用于记录和播放用户与浏览器的交互(录制web操作脚本)

selenium IDE安装:

1,必须是在火狐浏览器上,版本是35

2,selenium IDE是2.9,法一:可把这个压缩包(web相关软件文件夹中),直接拖至火狐浏览器中.即 E:\TestVideo\【赠】软件测试相搭配的所有工具安装包\web自动化相关软件\selenium_ide-2.9.1-fx.xpi

法二: 在selenium IDE官网直接找2.9的版本

法三:在火狐浏览器菜单栏----工具---附加组件 中搜索selenium IDE

##### firebug

firebug插件是火狐浏览器的一款插件,能调试所有网站语言.但对于测试,最主要的功能是快速定位html页面中的元素.

在线安装firebug:1,在火狐浏览器,v35版本

​				2,附加组件------搜素FireBug

##### 总结:

selenium IDE主要作用:1,录制脚本   2,转换成指定语言?????????

selenium IDE录制时,点击浏览器右上方小图标se,即为打开selenium IDE.在弹出的对话框中,1,在新项目中记录新测试  2,打开现有项目  3,创建新项目  4,关闭selenium ID

点击rec,为开始录制你在浏览器上的操作.

手动输入命令行完成录制:

如果自己写命令行,则不要点击rec,把速度调成slow.  直接先点击一下空白行,然后在下面写command,target,value,有些命令只需command.

open  pause    goBack    refresh

type(元素的定位表达式, 要输入的值)  如command 填 type  ,target填 id=kw  value填  周杰伦,即为在搜索框中写周杰伦.这个命令下面常跟点击按钮,为跳转页面到周杰伦.下行命令为command填click  , target填id=su,  

### webDriver

webDriver是什么:1,测试web项目的自动化测试工具     2,一套友好的API	3,不依赖任何测试框架,只需要浏览器驱动

API:应用编程接口说明(webDriver类库内封装非常多的方法,要使用这些方法,就需要有好的调用命名规则)

webDriver支持的浏览器:1,firefox 2,ie  3,opera  4,chrome  5,safari  6,htmlUnit

firefox,chrome  :对元素定位和操作有良好的支持,对js支持也非常好

ie: 只能在windows平台运行,是所有浏览器中运行速度最慢

htmlUnit:无界面运行,运行速度最快

webdriver就是找元素,操作元素

为什么要搭建环境?  1,工具包  2,解释器

##### python环境安装

1,windows系统     2,python3.5(以上版本  软件安装地址   E:\TestVideo\【赠】软件测试相搭配的所有工具安装包\接口相关软件)	  https://baijiahao.baidu.com/s?id=1606573927720991570&wfr=spider&for=pc	3,安装selenium包   4,浏览器			5安装pycharm

安装selenium:   pip install selenium==2.48.0(等号前后无空格)如果没有==2.48.0,会默任为最新版本

查看   pip show selenium

火狐浏览器推荐:

1,firefox 48 以上版本:

selenium 3.x + firefox 驱动(geckodriver)

2,firefox 48 以下版本:

selenium 2.x内置驱动



下了个Firefox39.0.2版本就好了。后附上下载地址：

https://archive.mozilla.org/pub/firefox/releases/39.0b2/win64/zh-CN/

在火狐扩展中心里，firebug这个插件的描述是：
适用：Firefox 30.0a1 - 52.0

，火狐在推出了新版本的浏览器55之后，火狐录制回放的小插件Selenium IDE就无法再使用了。

------

### 第二天  webDriver元素定位方式

##### -1节   webDriver定位方式分类

1)id,name,class_name  为元素属性定位

2)tag_name 为元素标签名称

3)link_text  partial_link_text:  超链接(a)定位

4) Xpath  元素路径定位

5)Css 为css选择器定位

sleep按ctrl+alt+空格,可自动导包from time import sleep

##### id定位

id定位操作步骤:1,导入需要的包   2,实例化浏览器   3,打开项目地址  4,定位元素    5,操作元素   6,暂停  7,关闭

id定位,元素必须   id='id的值'

```python
#coding=utf-8
#用id定位用户名,输入值,定位密码,输入值,等待3秒,关闭窗口
#导包
from selenium import webdriver
#这个sleep为自动导包,即下面敲sleep后,按ctrl+alt+空格,这个包就自动导好.
from time import sleep
# 实例化浏览器
driver=webdriver.Firefox
# 打开地址
driver.get('E:\\pycharmWorkSpace\\day01\\seleniumziliao\\注册A.html')
# 定位用户名文本框
element=driver.find_element_by_id('userA')
# 给文本框传值
element.send_keys('admin')
# 密码框同理
pwd=driver.find_element_by_id('passwordA')
pwd.send_keys('123456')
# 暂停3秒
sleep(3)
# 关闭浏览器
driver.quit()
```

第3步中,打开项目地址,有3种写法:

法1,转义符法,在每个反斜杠\后加一个\  'E:\\\pycharmWorkSpace\\\day01\\\seleniumziliao\\\注册A.html'

法2,r修饰,即被r修饰的字符串,字符串中的转义符不做转义使用

r'E:\pycharmWorkSpace\day01\seleniumziliao'

法3,打开地址,进入浏览器页面,复制地址栏中的地址

'file:///E:/pycharmWorkSpace/day01/seleniumziliao/%E6%B3%A8%E5%86%8CA.html'

##### name定位

name定位像人名,在当前文档中可以不是唯一的.name定位的前提是元素必须有name属性, 即 name='name的值'

##### class_name定位

class_name定位,元素必须  class='class的值'

此法定位元素 find_element_by_class_name()

##### tag_name定位

此法是通过标签名称来定位.find_element_by_tag_name('标签')返回的是符合条件的第一个标签.

##### link_text定位

此法主要针对a标签,需要传入a标签的全部文本

```python
driver.find_element_by_link_text('访问 新浪 网站').click()
```

##### partial_link_text定位

partial_link_text为模糊匹配,需要传入a标签局部文本---能表达唯一性..是对link_text的补充.

##### find_elements_by_xxx

1,查找定位所有符合条件的元素   

2,返回的定位元素格式为数组(列表)格式,列表数据格式的读取需要指定下标,下标从0开始

##### Xpath, css 定位策略

学习Xpath, css 定位的原因:1,实际项目中标签没有id,name, class属性   2,id,name, class属性值为动态获取,随着刷新加载而变化

Xpath是xml path 的简称,用来确定xml文档中某部分位置的语言.

html可以看做是xml的一种实现,所以selenium用户可以使用这种强大的语言在web应用中定位元素.

xml为一种标记语言,用于数据的存储和传递,后缀为.xml

Xpath为强大的语言,是因为它有非常灵活的定位策略

Xpath定位方法  driver.find_element_by_xpath()

##### xpath策略按优先级排列:

1,路径   2,属性  3,层级与属性(层级:父子标签)   4,属性与逻辑  

##### 绝对路径,相对路径

绝对路径:从最外层元素到指定元素之间所有经过元素层级路径,如/html/body/form/div/fieldset/p[1]   但我只要写[],就爆红?????????????

绝对路径以单斜杠/  开始.  使用firebug可以快速生成,元素xpath绝对路径.

寻找元素绝对路径,页面中查看元素----定位元素-----在HTML这栏(控制台后边),对标蓝的代码右键,选择复制xpath,即可得到此元素的绝对路径.

如果对蓝标的代码右键,选择复制最简xpath,即为相对路径.



相对路径:以双斜杠//开始,后边必须跟*或者标签名称.如//input[@id='userA']

能指定标签名称,绝不用*,做性能测试很关键.

使用firebug的扩展插件firepath可快速生成:点击firepath-----定位元素---此时xpath就出现此元素的相对路径.

##### 利用元素属性

快速定位元素,利用的是元素唯一属性,如  //input[@id='userA']

XPath中,使用属性,一定先写@

##### 层级与属性结合,

要找的元素没有属性,但是它的父级有

如//*[@id='p1']/input

##### 属性与逻辑结合

解决元素之间相同属性重名问题,比如定位A元素,它的一个属性和B的相同,一个属性和C的相同,a不能通过一个属性定住.     通过and逻辑,把A元素的定位卡死,如 //*[@id='userA'  and  @class='cA']

##### xpath延伸

//*[text()="文本内容"]    文本内容为全部的文本的元素,多用于a,h标签

//*[starts-with(@属性名, '属性值')]  如一个元素的属性name='password'  

*可写成 //*[starts-with(@name, 'pas')] 

但必须保证以pas开头的属性值为这一个.

//*[contains(@属性名, 'xxx')]   属性中含有xxx的元素



##### css常用定位

1,selenium中极力推荐css定位,因为它比xpath定位速度要快

2,css选择器语法强大

##### css定位方法  

driver.find_element_by_css_selector()

##### css定位常用的策略(方式)

1, id选择器  2,class选择器   3,元素选择器  4,属性选择器  5, 层级选择器

id,class是属性,但因为用的特别多,所以把它俩单独列出来.

##### id选择器

根据元素id属性来选择   格式: #id值,

css定位首先确保firepath下的路径为css, xpath定位确保firepath下的路径为xpath

```python
from selenium import webdriver
from time import sleep
driver=webdriver.Firefox()
url=r"E:\pycharmWorkSpace\day01\seleniumziliao\注册A.html"
driver.get(url)
#id选择器
driver.find_element_by_css_selector('#userA').send_keys('admin')
driver.find_element_by_css_selector('#passwordA').send_keys('123456')
#class选择器
driver.find_element_by_css_selector('.telA').send_keys('15091481234')
#元素选择器,一般是此元素只有1个,或者elements返回列表使用
driver.find_element_by_css_selector('button').click()
#属性选择器
driver.find_element_by_css_selector('[placeholder="文本1"]').send_keys('文本1的内容')

sleep(3)
driver.quit()
```

##### class选择器

根据元素class属性来选择   格式: .class值,

用法同id选择器一样

##### 元素选择器

直接根据元素的标签进行旋选择

##### 属性选择器

根据元素的属性名和值来选择,格式为  [属性名='值']

如[placeholder='输入密码']选择所有placeholder属性值为 输入密码的值

##### 层级选择器

根据元素的父子关系来选择   element>element  其中>也可用空格代替

如p #passwordA

##### css延伸

用input作为例子

1, input[type^='pa']  说明:input标签中,选择type属性中以pa开头的元素

2, input[placeholder$='母']  说明:input标签中,选择placeholder属性中以母结束的元素

3,input[class*='w']   input中,class属性中有w字母的元素

上述中,元素标签名称可以不用,直接[]写内容

------

##### day3

##### 2小节  元素操作方法, 浏览器操作方法

学习操作元素的方法原因:1,需要让脚本模拟用户给浏览器指定元素输入值     2,需要让脚本模拟人为删除元素的内容   3,需要让脚本模拟点击按钮

常用的元素操作方法 :  1,send_keys()  模拟输入    2,clear()   清除文本    3,click() 单击元素

##### 3小节 浏览器常用方法

通过webdriver操作浏览器的常用方法

```python
#coding=utf-8
# webdriver常用操作
from time import sleep
from selenium import webdriver
driver=webdriver.Firefox()
url=r'E:\pycharmWorkSpace\day01\seleniumziliao\注册实例.html'
driver.get(url)
# 浏览器打开页面是全屏
driver.maximize_window()
sleep(3)
driver.refresh()
driver.find_element_by_link_text('注册A网页').click()
sleep(3)
# 一个窗口打开2个网站,先后退,然后才能前进
driver.back()
sleep(3)
driver.forward()
sleep(3)
# 关闭,close,quit区别  close()关闭当前主窗口 ,quit()关闭由webdriver启动的所有窗口
driver.close()
# 不常用的浏览器操作
# driver.set_window_size(100, 100)  设置浏览器大小
# driver.set_window_position(100, 200)  设置浏览器位置

```

##### webdriver其他常用的操作方法

1,size 获取元素大小   2,text 获取元素的文本   3,title   获取页面title   4,current_url 获取当前页面url    5,get_attribute('xxx')  ,如 get_attribute(''type')    6,is_display() 判断元素是否可见   7,  is_enabled()  判断元素是否可用

size,text,title,current_url为属性,调用时无括号

title, current_url使用时浏览器实例化对象,直接调用.如driver.title

*****分析时候先分清哪些需要查找元素,哪些不需要查找元素

```python
#coding=utf-8
# webdriver其他操作
from time import sleep
from selenium import webdriver
driver=webdriver.Firefox()
url=r'E:\pycharmWorkSpace\day01\seleniumziliao\注册实例.html'
driver.get(url)
title=driver.title
print('此页面的title为 ',title)
current_url=driver.current_url
print('当前页面url为 %s' %current_url)
print('------------------------------')
is_display=driver.find_element_by_css_selector('p #passwordA').is_display()
print('"p #passwordA"这个元素是否存在: ',is_display)
is_enabled=driver.find_element_by_css_selector('input').is_enabled()
print('判断input标签是否可用: ',is_enabled)
print('**************')
size=driver.find_element_by_css_selector('#userA').size
print('id为userA的元素大小为: ',size)
text=driver.find_element_by_link_text('访问 新浪 网站').text
print('a标签链接文本值为: ',text)
get_attribute=driver.find_element_by_link_text('访问 新浪 网站').get_attribute('id')
print('get_attribute获取的值为: ',get_attribute)
```

text在实际工作中,通过获取元素的文本作为实际结果,和预期结果相比较.

title,  current_url也是和预期结果相比较.

get_attribute获取到属性对应的标签,然后给标签传送内容等,如get_attribute('id')得到'telA',我们就知道是电话号码,然后我们传送1个电话号码.

##### webdriver鼠标,键盘操作

webdriver将鼠标操作的方法封装在ActionChains类中.鼠标操作有右键 context_click,   双击 double_click  拖拽drag_and_drop   悬停 move_to_element

```python
#coding=utf-8
# 将鼠标悬停在 用户注册A 按钮,会显示加入会员A的提示
#鼠标悬停 move_to_element
from time import sleep
from selenium.webdriver.common.action_chains import ActionChains
from selenium import webdriver
driver=webdriver.Firefox()
driver.get(r'E:\pycharmWorkSpace\day01\seleniumziliao\注册实例.html')
element=driver.find_element_by_css_selector('button')
ActionChains(driver).move_to_element(element).perform()
sleep(3)
driver.quit()
```

##### 键盘操作

模拟键盘的一些操作,如ctrl+c,ctrl+v   webdriver中对键盘的操作封装在keys类中.

导包  from selenium.webdriver.common.keys import keys

常用的键盘操作:

1, send_keys(Keys.CONTROL, 'a') 全选

2, send_keys(Keys.CONTROL, 'x') 剪贴

3,   send_keys(Keys.ENTER)   回车键

4,    send_keys(Keys.ESCAPE)   回退键

5   send_keys(Keys.BACK_SPACE)   删除键   调用1次,删除1个字母或汉字

.......

```python
#coding=utf-8
# 输入用户名admin1,暂停3秒,删除1
# 全选用户名, 暂停3秒,
# 复制用户名admin, 暂停3秒
# 粘贴至密码框,暂停3秒
# 关闭浏览器
from selenium.webdriver.common.keys import Keys
from selenium import webdriver
from time import sleep
driver=webdriver.Firefox()
driver.get(r'E:\pycharmWorkSpace\day01\seleniumziliao\注册实例.html')
element=driver.find_element_by_css_selector('#user')
element.send_keys('admin1')
sleep(3)
element.send_keys(Keys.BACKSPACE)
sleep(3)
element.send_keys(Keys.CONTROL, 'a')
sleep(3)
element.send_keys(Keys.CONTROL, 'c')
sleep(3)
element1=driver.find_element_by_css_selector('#password')
element1.send_keys(Keys.CONTROL, 'v')
sleep(3)
driver.quit()
```

##### 设置元素等等

了解元素显示等待   掌握元素隐式等待

元素等待:webdriver定位页面元素时,如果未找到,会在指定时间内一直等待的过程.

设置元素等待的原因:

1,由于网络速度的原因

客户端向服务端发请求,服务器接收到请求后会给出一个响应,浏览器接收到响应的数据会解析这些数据的代码,最后展现给我们.有可能接收到数据的时候,浏览器没有解析完成,但元素定位已经开始找元素,造成没有找到,直接抛出异常.但是代码没有问题.在外网状态下很常见.所以元素等待是必须要设置的.

2,电脑配置原因

3,服务器处理请求原因

##### 显示等待

使webdriver等待指定元素条件成立时继续执行,否则在达到最大时长时抛出超时异常(TimeoutException)

需要引入2个包:

1,在webdriver中把显示等待的相关方法封装在WebDriverWait类中

2,等待是判定条件成立时,把相关的判断方法封装在expected_conditions类中

```python
#coding=utf-8
# 如果用户名文本框存在,就输入admin
from selenium.webdriver.common.keys import Keys
from selenium import webdriver
from time import sleep
from selenium.webdriver.common.by import By
from selenium.webdriver.support.wait import WebDriverWait
from selenium.webdriver.support. import expected_conditions as EC
# EC为简写
driver=webdriver.Firefox()
driver.get(r'E:\pycharmWorkSpace\day01\seleniumziliao\注册实例.html')
sleep(3)
element=(By.CSS_SELECTOR,'#user')
# 实例化WebDriverWait
WebDriverWait(driver, 10).until(EC.presence_of_element_located(element)).send_keys('admin')
sleep(3)
driver.quit()
```

##### 隐式等待

隐式等待:等待元素加载指定的时长,超出抛出   NoSuchElementException异常,在实际工作中,一般都使用隐式等待.

显示与隐式区别:

1,作用域:显示等待为  单个元素   有效,  隐式等待为   全局元素

2,方法: 显示等待方法封装在 WebDriverWait类中,而隐式等待   直接通过浏览器实例化对象  调用.

如果定位元素在第一次就定位到,则不会触发隐式等待时长.  

如果定位某一元素定位失败,那么就会触发隐式等待有效时长.  如果在指定时间内加载完毕,则继续执行.否则会抛出NoSuchElementException

------

##### day4

##### 3小节 下拉选择框

下拉框是html中的select元素

需求:城市选项下拉框,暂停3秒选上海,暂停3秒选重庆,暂停3秒选广州

法1,通过css定位option中的属性value='xx',操作元素

```python
from time import sleep
from selenium.webdriver.common.keys import Keys
from selenium import webdriver
driver=webdriver.Firefox()
driver.get(r'E:\pycharmWorkSpace\day01\seleniumziliao\注册实例.html')
driver.find_element_by_css_selector('[value="sh"]').click()
sleep(3)
driver.find_element_by_css_selector('[value="gz"]').click()
sleep(3)
driver.find_element_by_css_selector('[value="cq"]').click()
sleep(3)
driver.quit()
```

法2,select类

select类是webdriver为解决select标签定位诞生的,此类定位的是select标签.

select方法有3种:  根据option索引来定位,从0开始    select_by_index()       根据option属性value来定位    select_by_value()        根据option显示文本来定位  select_by_visible_text()



步骤:  导包   from selenium.webdriver.support.select import Select

​            实例化Select类   WebElement=定位的select元素      select=Select(WebElement) 

​	    调用方法         select.select_by_index(n)

```python
from time import sleep
from selenium import webdriver
from selenium.webdriver.support.select import Select
driver=webdriver.Firefox()
driver.get(r'E:\pycharmWorkSpace\day01\seleniumziliao\注册实例.html')
webelement=driver.find_element_by_css_selector('selector')
select1=Select(webelement)
# 用索引
select1.select_by_index(1)
sleep(3)
# value
select1.select_by_value("cq")
sleep(3)
# 用显示文本
select1.select_by_visible_text('广州')
driver.quit()
```

##### 警告框

html中,常用的弹出对话框有3种,处理方法都一样:1,alert  2,confirm  3,prompt

警告框的处理:1,获取警告框  alert=driver.switch_to.alert

2,调用警告框,有3种方法 1,alert.text  返回对话框中的文本信息 2,alert.accept()  接受对话框选项   3,alert.dismiss()取消对话框

```python
from time import sleep
from selenium import webdriver
driver=webdriver.Firefox()
driver.get(r'E:\pycharmWorkSpace\day01\seleniumziliao\注册实例.html')
driver.find_element_by_css_selector('[value="alert"]').click()
# 处理弹出的对话框
alert=driver.switch_to.alert
alert.accept()
driver.find_element_by_css_selector('#user').send_keys('admin')
sleep(3)
driver.quit()
```

##### 滚动条的操作



webdriver类库中并没有直接提供对滚动条进行操作方法,但它提供了可调用javascript脚本的方法,所以可以通过javascript脚本来达到操作滚动条的目的.

学习滚动条操作的原因:

1,页面的注册同意条款,需要滚动条到最底部,才能点击同意

2,html页面中,页面元素为动态显示,元素根据滚动条的下拉而被加载

需求实现分析:1,设置javascript脚本控制滚动条 ,让滚动条垂直向下移动m像素    js='window.scrollTo(0, m)'  

2,webdriver调用js脚本方法    driver.execute_script(js)

```python
#coding=utf-8
# 滚动条向下拉到1000,然后在回到(0,0)位置
from time import sleep
from selenium import webdriver
driver=webdriver.Firefox()
driver.get(r'E:\pycharmWorkSpace\day01\seleniumziliao\注册实例.html')
js1='window.scrollTo(0, 1000)'
driver.execute_script(js1)
sleep(3)
js2='window.scrollTo(0, 0)'
driver.execute_script(js1)
sleep(3)
driver.quit()
```

##### frame表单切换

frame:主要作用是在当前页面的指定区域显示另一页面元素

在html中,frame  ,  iframe 标签为表单框架

切换表单方法：  driver.switch_to.frame("frame标签的name属性值")

进行第3个表单切换时，需要先恢复到默任页面，因为第二个页面没有要切换的frame的name属性值。恢复方法是 driver.switch_to.default_content



##### 多窗口切换

在webdriver中,封装了获取当前窗口句柄方法和获取所有窗口句柄方法以及切换指定句柄窗口的方法.

句柄: handle   是窗口的唯一识别码

方法:

1,  driver.current_window_handle   获取当前窗口句柄

2,  driver.window_handles  获取所有窗口句柄

3, driver.switch_to.window(handle)  切换指定句柄窗口

##### 窗口截图

把当前操作页面,截图保存在指定位置

窗口截图的原因:自动化脚本是由程序去执行,因此有时候打印的错误信息并不明确.如果在执行出错的时候对当前窗口截图保存,那么通过图片就直观看到出错原因.

webdriver类库中,可以调用此方法

driver.get_screenshot_as_file('图片保存的路径')

```python
#coding=utf-8
#注册实例页面中,点击注册A网页,跳转到新的页面,然后再次操作元素.
from time import sleep
from selenium import webdriver
driver=webdriver.Firefox()
driver.get(r'E:\pycharmWorkSpace\day01\seleniumziliao\注册实例.html')
# 获取当前窗口句柄
current=driver.current_window_handle
driver.find_element_by_link('注册A网页').click()
# 获取所有窗口句柄
handles=driver.window_handles
# 遍历及切换
for handle in handles:
    if handle != current:
        # 执行切换窗口
        driver.switch_to.window(handle)
        #填写注册A信息
        driver.find_element_by_css_selector('#userA').send_keys('admin1')
        #截屏保存      driver.get_screenshot_as_file('../images/img1.jpg')
sleep(3)
driver.quit()
```

##### 验证码

一种随机生成的信息(图片.数字,字母,汉字等).目的是为了防止恶意的请求行为,增加软件应用的安全性.

学习验证码的原因:在web应用中,大部分系统在用户登录的时候都要输验证码,所以我们在设计自动化脚本时,就需要面临验证码的问题.

验证码的几种处理方式:

1,去掉验证码(把验证码注释掉,在测试环境下采用)

2,设置万能验证码(比如123123,是在生产环境,项目上线了,有用户使用,采用)

3,验证码识别技术(识别图片类型的验证码,识别率很难达到100%)

4,记录cookie(通过记录cookie进行登录,是比较推荐的方法)

##### cookie

作用:绕过验证码登录

记录:登录后的用户名,密码,把加密的用户名和密码信息一起发送给服务器

提示:记得要刷新

方法: add_cookie(字典)

```python
#coding=utf-8
from selenium import webdriver
import time 
driver=webdriver.Firefox()
driver.get('http://www.baidu.com')
driver.add_cookie({'name':'BAIDUID','value':'根据实际的情况填写'})
driver.add_cookie({'name':'BDUSS','value':'根据实际的情况填写'})
time.sleep(3)
driver.refresh()
time.sleep(3)
driver.quit()
```

##### cookie工作步骤还是不熟

------

day5

##### UnitTest框架

框架:主要为了解决一类事情的功能集合

UnitTest框架是专门用来进行执行代码测试的框架.

使用UnitTest框架原因:1,能够组织多个用例去执行   2,提供丰富的断言方法     3,提供丰富的日志与测试结果

UnitTest核心要素:TestCase,      TestSuit,     TextTestRunner,    Fixture

#####TestCase

```python
#导包
import unittest
#新建测试类,继承unittest.TestCase
class Test01(unittest.TestCase):
    #必须是test开头
    def test01(self):
        print('test01被执行')
    def test02(self):
        print('test02被执行')
# 方法只要以test开头就行,不需要实例化对象及方法
#方法在main中运行,快捷键为main cterl+alt+空格
if __name__ =='__main__':
    unittest.main()
#main语句的作用是本文件中的文件只在本文件中运行,导包到其他文件中,在本文件中就不执行了.在单个模块测试中要用
```

##### TestSuite

TestSuite:多条测试用例集合在一起

使用:

1,实例化   suite=unittest.TestSuite()

2,添加用例  suite.addTest(类名('方法名'))

3,添加扩展   suite.addTest(unittest.makeSuite(ClassName))

搜索指定ClassName内以test开头的方法并添加到测试套件中

```python
import unittest
#导入需要测试的用例
from unit_test.Case.test02 import Test02
from unit_test.Case.test03 import Test03
from unit_test.Case.test04 import Test04
if __name__ == '__main__':
    #实例化 suite
    suite=unittest.TestSuite
    #调用 法1添加用例方法
    suite.addTest(Test02('test001'))
    suite.addTest(Test03('test001'))
    #调用 法2添加扩展法
    suite.addTest(unittest.makeSuite(Test04))
    #TestSuite需要配合TextTestRunner才能被执行
    runner=unittest.TextTestRunner()
    runner.run(suite)
```

##### Fixture

Fixture是一个概述,对一个测试用例环境的搭建和销毁就是一个Fixture

1,初始化(搭建)   def setUp(self)    setUp:此方法继承于unittest.TestCase 首先被执行

2,结束(销毁)   def tearDown(self)    tearDowm此方法继承于unittest.TestCase    最后被执行

注意:

1,必须继承unittest.TestCase类,,setUp,tearDown才是一个Fixture

2,setUp一般做初始化工作,比如:实例化浏览器, 浏览器最大化,  隐式等待等

3, tearDown一般做结束工作,比如关闭浏览器,退出登录等

4,如果一个测试类有多个test开头的方法,则每个方法执行之前都会运行setUp, 结束时运行 tearDown

```python
import unittest
class Test01(unittest.TestCase):
    def test001(self):
        print('001被执行')
    def setUp(self):
        print('suetUp被执行')
    def tearDown(self):
        print('tearDown被执行')
    def test002(self):
        print('002被执行')
 if __name__ == '__main__':
        unittest.main()
```

##### 案例 iweb登录

使用unittest框架对iweb项目进行正向登录测试

步骤分析:

1,导包  import unittest

2,新建测试类并继承unittest.TestCase

3,新建一个Fixture(setUp, tearDown)

4,新建登录方法

5,if __name__ == '__main__':

​	unittest.main()

```python
#百度登录
import unittest
from time import sleep
from selenium import webdriver
class Iweb_login(unittest.TestCase):
    def setUp(self):
        #实例化浏览器
        self.driver=webdriver.Firefox()
        #打开项目网站
        self.driver.get('https://www.baidu.com/')
        #最大化浏览器
        self.driver.maximize_window()
        #设置隐式等待
        self.driver.implicitly_wait(30)

    def test_login(self):
        #登录
        driver=self.driver
        driver.find_element_by_link_text('登录').click()
        driver.find_element_by_css('#TANGRAM__PSP_10__userName').send_keys('15091489951')
        driver.find_element_by_css('#TANGRAM__PSP_10__password').send_keys('youyou123')
        driver.find_element_by_css('[value="登录"]').click()
        sleep(3)
        #退出
        driver.find_element_by_css('#TANGRAM__PSP_10__submit').click()
        driver.find_element_by_css('[onclick="return false;"]').click()
        sleep(3)
    def tearDown(self):
        #关闭浏览器
        self.driver.quit()
```

##### defaultTestLoader

使用defaultTestLoader()类,通过该类下面的discover()方法自动搜索指定目录下,指定开头的.py文件,并将查找到的测试用例组装到测试套件.

discover = unittest.defaultTestLoader.discover('指定的目录', pattern='此目录下查找的.py文件的格式')。搜索指定的目录，指定的py文件，并返回所有搜索文内以test开头的方法，返回的形式以测试套件的形式返回。

运行为:

runner=unittest.TextTestRunner()

runner.run(discover)

```python
#需求:批量运行本文件夹下test01.py---test10.py
import unittest
if __name__ == '__main__':
    #定义测试套件
    discover=unittest.defaultTestLoader.discover('./',pattern='test*.py')
    #指定测试套件
    unittest.TextTestRunner().run(discover)
```

defaultTestLoader与TestSuite区别:

1,TestSuite可以添加TestCase中所有test开头的方法以及添加指定的test开头方法

2, defaultTestLoader搜索指定目录下指定开头的.py文件,并添加TestCase中所有test开头的方法,不能指定添加方法

defaultTestLoade属于TestSuite另一种实现方式.

##### 断言

断言:让程序代替人为判断程序执行结果是否符合预期结果的过程

```python
import unittest
class Test001(unittest.TestCase):
    def test_1(self):
        self.assertIn('admin', '你adimin好')
        str=False
        self.assertTrue(str)
```

assertEqual(arg1, arg2), 验证arg1, arg2是否相等,不等则fail

assertIn(arg1, arg2)    验证arg1是arg2的子串,不是则fail

##### html报告生成

测试报告生成的步骤:

1,复制HTMLTestRunner.py文件到项目文件夹,此文件在E:\TestVideo\第四阶段-web自动化+白盒测试\web自动化Day05\02_其他资料

1. 2,导入HTMLTestRunner, UnitTest包


3,discover加载要执行的用例

discover=unittest.defaultTestLoader.discover(test_dir, pattern='test.py')

4,设置报告生成路径和文件名

file_name=file_dir + nowtime +'report.html'

5,打开报告

with open(file_name,'wb') as f:

6,实例化HTMLRunner对象

runner=HTMLTestRunner(stream=f)

7,执行

runner.run(discover)

```python
import unittest,time
from unit_test.Case.tools.HTMLTestRunner import HTMLTestRunner
#添加测试套件
unittest.defaultTestLoader.discover('./',pattern='test*.py')
if __name__ == '__main__':
    dir_path='../report/'
    nowtime=time.strftime('%Y_%m_%d %H_%M_%S')
    file_name=dir_path+nowtime+'report.html'
    with open(file_name,'wb') as f:
        HTMLTestRunner(stream=f,).run(discover)
```

------

##### 白盒测试day1

##### 单元测试

1, 语句:非分支  非判断  的代码

语句覆盖率=被覆盖语句 / 总语句

2, 分支:判断语句的分支,如if判断有N个分支

分支覆盖率 = 覆盖分支 / 总分支数

3, 条件:结果为true或false

注意:条件之间使用逻辑 and连接时,如果第一个条件失败,则不会判断第2个条件.  如果使用or,第一个条件成功,则不会判断第二个条件.第一个条件失败,才会判断第二个条件.

4, 路径:从开始到结束的过程

路径的分子永远为1

5,分支-条件覆盖率

分支覆盖率的分子+条件覆盖率的分子 /  分支覆盖率的分母+条件覆盖率的分母

##### 测试策略

1,自上到下   2,自下到上   3,孤立策略

打桩:模拟被调用的函数名(pass或者 return 结果(如一个数10等)

------

##### 白盒测试day2

##### 参数化

参数化:根据需求动态获取数据并进行赋值的过程

参数化方式:1,XML格式    2,CSV格式    3,JSON串   4,TXT文本

##### txt

导包中,从文件夹一层层找到指定文件里的类名,老出错!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

```python
#在unittest框架中,所以导unittest.检测三角形,所以导三角形的判定文件,还要txt读取
import unittest
from day01.baiheces2.codes.sjx import Sjx
from day01.baiheces2.ReadData.read_txt import Read_Txt
#实例化三角形
sjxClass=Sjx()
#实例化txt
readTxtClass=Read_Txt()
class Test_Txt(unittest.TestCase):
    #测试三角形程序
    def test001(self):
        #调用三角形方法
        for i in range(len(readTxtClass.Read_Txt())):
            result=sjxClass.sjx(int(sjxClass.sjx(readTxtClass.Read_Txt()[i][0]),
                        int(sjxClass.sjx(readTxtClass.Read_Txt()[i][1]),
                        int(sjxClass.sjx(readTxtClass.Read_Txt()[i][2]))
            #调用断言,判定程序执行后的结果是否与预期相符
            self.assertEqual(result, readTxtClass.Read_Txt()[i][3])
            print(sjxClass.sjx(readTxtClass.Read_Txt()[i][0],
                               readTxtClass.Read_Txt()[i][1],
                               readTxtClass.Read_Txt()[i][2],
                               readTxtClass.Read_Txt()[i][3])

if __name__ == '__main__':
    unittest.main()
```



------

##### day1 接口测试 

接口:数据交互的入口和出口,是一套规范,一套标准.

分类:

硬件:USB接口  电源接口  网线接口

软件:前后端共同遵守的一套数据交互的规范

不使用接口的缺点:

1,研发标准不统一,团队磨合难度高  2,增加了研发周期   3,可扩展性差(需要频繁沟通)

使用接口的好处:

1,统一了设计标准  2,前后端开发相对独立  3,扩展性灵活   4,前后端都可以使用自己熟悉的技术

高效,灵活:前端和后端不用频繁沟通,看相关文档就行

##### 接口的环境搭建:

1. 安装python环境  推荐python3.5以上版本

2. 安装依赖模块：pip install -r requirements.txt -i https://pypi.douban.com/simple (复制粘贴到dos命令行,但我粘贴了,需要升级,没安装好)
   若安装速度慢，指定国内源,需再加上: -i https://pypi.douban.com/simple    

3. 如果须使用mysql，那么需要将studentManagementSystem/studentManagementSystem/settings.py的第78行的配置更改一下，注释掉sqllite3，解注释mysql的配置

4. 执行studentManagementSystem.sql文件，生成数据库

5. 启动命令：python run_server.py

6. 默认端口是8000，地址本机ip

   ##### SQLiteStudio安装

   E:\TestVideo\【赠】软件测试相搭配的所有工具安装包\接口相关软件\SQLiteStudio\SQLiteStudio.exe

   安装成功后的图标是个银白色圆筒,然后可以把数据如db.sqlite3拖到SQLiteStudio左边部分,  在tables中,选择classes--Generate....-----select---在右部分就打开了-----点击运行

   ##### 接口测试用的插件

   火狐浏览器------RESTClient      我安装的时候对火狐浏览器要求是48版本,35版本安装不上啊

   谷歌浏览器------POSTman

   谷歌浏览器安装包位置:E:\TestVideo\【赠】软件测试相搭配的所有工具安装包\接口相关软件\谷歌

   ​

   java实现的测试工具------Jmeter(重点)

   ##### 接口测试风格:RESTful

   RESTful风格:开发测试时,大家习惯遵守的一些默任的规范. RESTful风格中规范了URL的实现方式,提交数据的实现方式,响应数据的实现方式.........

   RESTful风格是为了程序的易读性和易维护性