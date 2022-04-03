# html-css-code-
heima程序员的


HTML

    # java学科的学习阶段
    1. javase
    	standard edition : 标准版 (java基础语法)
    	enterprice edition : 企业版 (企业级应用)
    	micro edtion : 微型版 
    	
    2. javaweb (website : 网站)
    	 目的: 做一个简易的网站
    	
    3. 框架
    	 SSM框架: javase + javaweb 整合 
    	 
    4. 项目
    	



    # web阶段  : 做网站
    1. 数据库(重点)
    2. 前端 
    3. 后端(重点)
    
    # 前端
    0. 网页 : 跟用户打交道 (移动端)
    1. 基础
        a. html : 网页结构
        b. css : 美化网页
        c. javascript : 交互效果
    2. 框架
        a. vue 
        b. elementUI
    
    # 开发环境
    1. 开发工具 : HBuilder(改自eclipse),DreamWeaver,VScode
    		IDEA
    2. 运行环境
    		浏览器(chrome : google浏览器)



---

    # 今日目标
    
    1. 会使用页面中的文字,超链接,图片,列表,特殊符号
    2. 会使用表格完成页面布局
    3. 掌握HTML表单控件



一 HTML概述

超文本标记语言（HyperText Markup Language）

作用：搭建基础网页

超文本：超出文本的范畴, 不仅具有普通文本的特性，同时还可以加入图片、视频、超链接等等。

标记：即标签，定义好的标签有不同的功能和效果；例如：<img/>   

语言：人与计算机沟通桥梁



HTML 的语法规范是 由 W3C(World Wide Web Consortium 万维网联盟) 制定的。

html : HyperText Markup Language

XML: extensible markup language 可扩展的标记语言

不同:

	html 的作用是显示数据, 标签名是有固定含义的, 不同的标签会有不同的效果

	xml 的作用是存储和传输数据的, 标签名没有固定含义, 可以自定义





二 HTML基础【掌握】



2.1 快速入门

    # idea中工程和模块
    1. 工程: project  
    	1). 一个工程可以包含多个模块
    	2). 一个项目是用一个工程实现的
    2. 模块: module 
    
    # 方案
    1. 一天一个工程
    
    2. 一天一个模块
    	1). 好处: 方便, 不需要频繁切换idea界面
    	2). 坏处: A模块有问题,会影响到B模块



从今天开始，需要创建一个新的工作空间（空工程）

 



- jdk版本必须是1.8
 
- 字符集UTF-8
 



创建前端 static web（模块）

 



标准前端工程结构

    |-- 项目名
    	|- css 目录
    	|- js  目录 	
    	|- img 目录
    	index.html

    <!DOCTYPE html>
    <!-- 文档声明 document type html5.0(固定)-->
    <html lang="zh-CN"> <!-- 根标签html (language 语言: en 英语/ zh-CN 简体中文)-->
        <head>  <!-- 头信息: 主要给浏览器看的-->
            <meta charset="UTF-8">  <!-- 字符集: utf-8 -->
            <title>你好</title>  <!-- 网页标题: 标签栏 -->
        </head>
        <body><!-- 主体: 主要给用户看的 -->
            hello world
        </body>
    </html>
    <!--
        注释 : 快捷键  ctrl + shift + /
    -->



 



2.2 书写规范

    1. 文档声明
    	要求：必须在第一行，固定格式
    	
    2. 标签
    	1). 要求：正确嵌套，正确闭合
    	2). 双标签
    		<开始></结束>	 start tag/end tag  开标签/闭标签
    	3). 单标签
    		<开始,自关闭/>	
    	4). 补充: 元素(element) 从开标签到闭标签之间的所有内容	
    3. 属性
    	要求：必须在开始标签(单标签)中编写，属性值单双引都可
    		<开始 属性名="属性值"></结束>
    		
    4. 文本
    	要求：在标签体内编写
    	
    5. 注释
    		<!-- 注释内容 快捷键: ctrl+shift+/ -->





三 HTML常用标签【记忆】

3.1 标签语义

学习标签是有技巧的，重点记住标签的语义，简单的理解为：这个标签能干啥

 





3.2 标题标签

    <!DOCTYPE html>
    <html lang="zh">
    	<head>
    		<meta charset="UTF-8">
    		<title>01-网页标题（古诗三百首）</title>
    	</head>
    	<body>
    <!--
    	hn : header 正文标题
    		  number 1~6 (大到小)
    -->
    	<h1>静夜思</h1>
    	<h2>静夜思</h2>
    	<h3>静夜思</h3>
    	<h4>静夜思</h4>
    	<h5>静夜思</h5>
    	<h6>静夜思</h6>
    	床前明月光，疑是地上霜。
    
    
    
    	</body>
    </html>
    



3.3 水平线标签

    <!DOCTYPE html>
    <html lang="zh">
    <head>
        <meta charset="UTF-8">
        <title>02-水平线</title>
    </head>
    <body>
        <!--
            hr : horizontal 水平线
        -->
        <h1>静夜思</h1>
        床前明月光，疑是地上霜。
        <hr>
        <hr/>
        <h1>悯农</h1>
        春种一粒粟，秋收万颗子。
        <!--
            html属性（只能写在开标签或者单独标签）
            1. color 颜色
                1). 英文单词 red green blue
                2). RGB (红绿蓝, 光三原色)
                    I. 每个颜色取值 0~255 (16进制 00 ~ ff)
                    II. 语法: #ff0000
                        缩略 #f00 (相邻两位一样,可以只写一个)
            2. size 尺寸
                px : pixel 像素 (默认单位)
                (1080 * 1920) fhd
            3. width : 宽度
                1). 固定 500px
                2). 百分比 50%(占浏览器窗口)
    
            4. align 排列
                left  center right
    
           # 注意点 :  html属性非必要不使用
           1. html属性可能不通用 (举个例子: 不是所有的html标签都有color属性)
           2. html属性可能含义不同
                大部分html属性可以使用css替代
    
        -->
        <hr color="red">
        <hr color="pink">
        <hr color="#ff0000">
        <hr color="#000000" size="70" width="500px" align="left">
        <hr color="#0f0" size="50" width="50%" align="center">
        <hr color="#2932E1" size="50px" width="500px" align="right">
    
        <h1 color="red">标题</h1>
    
        <font size="3">font</font>
        <font size="7">font</font>
    </body>
    </html>



3.4 段落和换行标签

    <!DOCTYPE html>
    <html lang="zh">
    <head>
        <meta charset="UTF-8">
        <title>03-段落和换行</title>
        <style>
            /* css */
            p{
               text-indent: 2em;
            }
        </style>
    </head>
    <body>
    <!--
        window系统换行符: \r\n
        浏览器换行  <br>  break line
              段落  <p>  paragraph  (具有更大段间距)
    -->
    我是<br>
    <p>
    传智专修学院是一所为互联网、人工智能、工业4.0培养高精尖科技人才的应用型大学。学校经江苏省宿迁市教育局批准，由江苏传智播客教育科技股份有限公司投资创办。
    </p>
    <p>
    当今世界已进入人工智能、机器人时代，人工智能、机器人已成为未来30年、甚至50年科技革命最重要的发展方向。世界各国越来越重视，我国政府也高度关注人工智能的发展，无论是党的十八大、十九大，还是2017、2018、2019的政府工作报告，均提出要重点发展人工智能、机器人，并提升到国家战略层面。
    </p>
    技术发展首要是人才，而我国这方面人才非常紧缺。根据国家相关部门测算，目前我国人工智能人才的缺口就已经超过了500万，国内的供求比例仅为1:10，供需比例严重失衡。并且随着社会信息革命的进一步深入，相应人才的缺口会越来越大。但在这些新技术面前，目前我国关于这方面人才的规模化培养，无论是高校还是科研机构，均没有成熟的培养体系和方案，都还处于摸索阶段。
    </body>
    </html>



3.5 超链接标签

    <!DOCTYPE html>
    <html lang="zh">
    <head>
        <meta charset="UTF-8">
        <title>04-超链接</title>
    </head>
    <body>
    <!--
          # a : anchor 锚 (超链接)
            1. 必要属性 href
                0). hypertext reference 超文本链接
                1). 远程地址 : 网址
    
                2). 本地地址 : 当前工程内的网页
                    ./  当前路径  (可以省略)
                    ../ 上一级路径
    
                3). 扩展 : 锚点 (网页内跳转)
                     1. 给网页中的任意标签, 设置一个id属性(唯一)
                        id = myid
                     2. a.href = #myid
                     3. 效果: 点击a标签,回到id属性对应的标签位置
    
           2. target : 目标
                1). _self  在当前标签页打开链接  (默认)
                2). _blank 在新标签页打开链接
    -->
    <h1 id="myid">正文标题</h1>
    <h2 id="myid2">正文标题222</h2>
        <a href="http://www.baidu.com" target="_self">百度一下_本页面打开</a> <br>
        <a href="http://www.baidu.com" target="_blank">百度一下_新页面打开</a> <br>
        <a href="01-标题.html">标题页面</a> <br>
        <a href="./01-标题.html">标题页面</a> <br>
        <a href="../index.html">索引页</a>
           <br><br><br><br>
           <br><br><br><br>
           <br><br><br><br>
           <br><br><br><br>
           <br><br><br><br>
           <br><br><br><br>
           <br><br><br><br>
           <br><br><br><br>
           <br><br><br><br>
           <br><br><br><br>
           <br><br><br><br>
           <br><br><br><br>
        <a href="#myid2">回到顶部</a>
    
    
    </body>
    </html>



3.6 图像标签

    <!DOCTYPE html>
    <html lang="zh">
    <head>
        <meta charset="UTF-8">
        <title>05-图像</title>
    </head>
    <body>
    <!--
                img : image 图像
                    1. 必要属性 src (source 源)
                        a. 图片放在static web下的img文件夹
                        b. 设置两种
                            1). 本地图片 a.jpg (320*480)
                            2). 远程图片 (联网)
    
                    2. width: 宽度
                    3. height: 高度
                         只要设置单边, 另一边也会等比例缩放
                         所以一般宽高不会同时设置, 同时设置不好看
    
                    4. alt : 如果图片加载失败,出现的提示
                        (用户的网络不好/ 网络图片被删除)
    
                    5. title: 鼠标移上去出现的提示
            -->
    
            <img src="https://ss0.bdstatic.com/70cFvHSh_Q1YnxGkpoWK1HF6hhy/it/u=2445189716,31233286&fm=26&gp=0.jpg" alt="">
        <img src="../img/a.jpg" alt="" title="这是一个可爱的妹子">
        <img src="../img/a.jpg" alt="" width="160">
        <img src="../img/a.jpg" alt="图片加载失败" height="160">
        <img src="../img/b.jpg" alt="图片加载失败:呵呵">
    
    
    
    </body>
    </html>



3.7 列表标签

    <!DOCTYPE html>
    <html lang="zh">
    <head>
        <meta charset="UTF-8">
        <title>06-列表</title>
    </head>
    <body>
    <!--
        1. 有序列表
            父标签: ol (ordered list)
                 type=1, I, a
            子标签: li (list) 列表项
    
        2. 无序列表
            父标签: ul (unordered list)
                type=disc,circle,square
            子标签: li (list) 列表项
    
        快捷方式:
            1. ul>li*3 tab自动补全
                父标签>子标签*n
            2. ctrl + alt + l : 代码格式化,好看
    -->
        <h1>奥运奖牌榜</h1>
        <ol type="1">
            <li>中国</li>
            <li>美国</li>
            <li>俄罗斯</li>
        </ol>
    
        <h1>电器区</h1>
        <ul type="square">
            <li>苏宁</li>
            <li>美的</li>
            <li>海尔</li>
        </ul>
    
    
    
    </body>
    </html>

3.8 div和span标签

- 没有语义的，他们就是一个盒子，用来装内容

    <!DOCTYPE html>
    <html lang="zh">
    <head>
        <meta charset="UTF-8">
        <title>07-容器标签</title>
    </head>
    <body>
    <!--
        <div> 和 <span> 是没有语义的，它们就是一个盒子，用来装内容的
        1. div标签和span标签没有特殊效果
        2. div标签包裹的内容会自动换行
        3. span标签包裹的内容不会自动换行
    -->
        <div>div1</div>
        <div>div2</div>
        <span>span1</span>
        <span>span2</span>
    
    </body>
    </html>



3.9 转义（实体）字符



    重要!
    半个英语字母英文空格 &nbsp;
    一个汉字中文空格  &emsp;
    小于号 &lt;
    大于号 &gt;
    &符号 &amp;



    <!DOCTYPE html>
    <html lang="zh">
    <head>
        <meta charset="UTF-8">
        <title>08-实体字符</title>
    </head>
    <body>
    <!--
    常用的实体字符(了解)
        也称之为 转义字符
        语法: & 开头 ; 结尾 中间是英文缩写
    
        &lt; 小于  less than
        &gt; 大于  greater than
    
    -->
    效果 <br>
    &nbsp;半个英语字母英文空格   <br>
    &emsp; 一个汉字中文空格   <br>
    小于号 &lt;   <br>
    大于号 &gt;   <br>
    &符号 &amp;   <br>
    爱心 &hearts;   <br>
    元 &yen;   <br>
    
    </body>
    </html>



3.10 基本表格

- 有条理性的展示数据内容

 

 

    <!DOCTYPE html>
    <html lang="zh">
    <head>
        <meta charset="UTF-8">
        <title>09-基本表格</title>
    </head>
    <body>
    <!--
        表格思路:
            有一个表格, 具备怎样的特点
            第一行是几个数据
            第二个有几个数据...
    
        # 标签
        1. table 表格
            1). border : 边框
            2). cellspacing : 单元格之间的距离(google浏览器默认是2px)
                                外间距
            3). cellpadding :  单元格边框和内容之间的距离
                                内间距
            4). width : 宽度
            5). align : 当前表格在网页中的排列
    
        2. tr : table row 表格行
            1). align : 整行内容的排列
    
        3. td : table data 表格数据
           1). align : 单元格内容的排列
    -->
    <table border="1px" cellspacing="0px" cellpadding="10px" width="500px" align="center">
        <tr align="center">
            <td>姓名</td>
            <td>年龄</td>
            <td>身高</td>
            <td>体重</td>
        </tr>
        <tr>
            <td align="center">张三</td>
            <td>18</td>
            <td>180</td>
            <td>160</td>
        </tr>
        <tr>
            <td>张三</td>
            <td>18</td>
            <td>180</td>
            <td>160</td>
        </tr>
        <tr>
            <td>张三</td>
            <td>18</td>
            <td>180</td>
            <td>160</td>
        </tr>
    </table>
    
    
    
    
    </body>
    </html>





3.11 合并表格

 



    <!DOCTYPE html>
    <html lang="zh">
    <head>
        <meta charset="UTF-8">
        <title>10-表格合并</title>
    </head>
    <body>
    <!--
        # 合并单元格思路
        1. 先不用管合并, 先写出完整表格
        2. 接着考虑跨行还是跨列 (同行跨列,同列跨行)
        3. 最后删除多余单元格
    
        # 合并的关键
           让一个单元格膨胀
        1. 跨行 : rowspan
        2. 跨列 : colspan (column 列)
    
        需求A:  合并
             第一行第一列
             第二行第一列
             解决: 让11跨两行,删除21
    
        需求B : 合并
              第一行第三列
              第一行第四列
              解决: 让13跨两列,删除14
    
    -->
    <table border="1px" cellspacing="0px" cellpadding="10px" width="500px">
        <tr>
            <td rowspan="2">11</td>
            <td>12</td>
            <td colspan="2">13</td>
    
        </tr>
        <tr>
            <td>22</td>
            <td>23</td>
            <td>24</td>
        </tr>
        <tr>
            <td>31</td>
            <td>32</td>
            <td>33</td>
            <td>34</td>
        </tr>
        <tr>
            <td>41</td>
            <td>42</td>
            <td>43</td>
            <td>44</td>
        </tr>
    </table>
    
    </body>
    </html>





四 HTML表单【重点】

4.1 表单概述

1. 采集用户数据
2. 发送数据到服务器端（java服务器）





4.2 表单控件



    <!DOCTYPE html>
    <html lang="zh">
    <head>
        <meta charset="UTF-8">
        <title>11-表单控件</title>
    </head>
    <body>
    <!--
        表单的作用:收集用户数据,并发送服务器
    
        # form标签
        1. action属性 :  服务器的地址(请求地址)
        2. method属性 :   请求方式(http协议)
            1). get : 将请求参数拼接到请求地址
                    请求地址?name=value&name=value...
            2). post
    
        # form标签有三个子标签
            1. input标签 (复杂)
            2. select标签
            3. textarea标签
    -->
        <form action="http://www.baidu.com" method="get">
            <input type="text" name="username" placeholder="请输入用户名"> <br>
            <input type="password" name="password" placeholder="请输入密码"> <br>
            <input type="submit">
        </form>
    
    </body>
    </html>



    <!DOCTYPE html>
    <html lang="zh">
    <head>
        <meta charset="UTF-8">
        <title>11-表单控件</title>
    </head>
    <body>
    <!--
        # form标签有三个子标签
            1. input标签 (复杂)
            2. select标签
            3. textarea标签
    
        # input标签
            1. type属性
                1). text 文本 (默认)
                2). password 密码 (隐藏输入的内容)
                3). radio 单选框
                4). checkbox  复选框
                5). date 日期
                6). file 上传文件
                7). submit 提交(此按钮被点击,表单的数据会提交到服务器)
                8). reset 重置(恢复初始化)
    
                问题1: radio还不能单选?
                问题2: 点击submit,参数提交失败?
                        请求地址?name=value&name=value...
            2. name属性
                1). 需要提交数据的表单项必须要写
                2). 具有相同name属性的radio互斥,产生单选效果
    
               问题3: radio/checkbox 默认值为on,无法区分选项
    
            3. value属性
                1). radio/checkbox 必须要设置,以区分选项
                2). 文本型输入框 也设置, 达到默认值效果
    
            4. checked属性
                1). radio/checkbox的默认值设置
                2). 语法  checked = "checked"
                   (属性名和值相同的情况,都可以省略)  checked
    
             5. placeholder 属性
                    占位符(提示符)
    
    
    -->
       <form action="http://www.baidu.com" method="get">
           用户<input type="text" name="username" value="hehe"> <br>
           密码<input type="password" name="password" placeholder="请输入密码"> <br>
           性别
                <input type="radio" name="sex" value="male" checked="checked"> 男
                <input type="radio" name="sex" value="female"> 女
                <br>
           喜好
           <input type="checkbox" name="hobby" value="smoke" checked> 抽烟
           <input type="checkbox" name="hobby" value="drink"> 喝酒
           <input type="checkbox" name="hobby" value="firehead"> 烫头 <br>
           生日 <input type="date" name="birth"> <br>
           上传附件 <input type="file" name="file"> <br>
           <input type="submit" value="注册">
           <input type="reset">
    
    
    
       </form>
    
    </body>
    </html>



    <!DOCTYPE html>
    <html lang="zh">
    <head>
        <meta charset="UTF-8">
        <title>11-表单控件</title>
    </head>
    <body>
    <!--
        # form标签有三个子标签
            1. input标签 (复杂)
            2. select标签
            3. textarea标签
    
    
        # select标签 (下拉框)
        1. select属性
                name
        2. select子标签
                option 选项
                    value属性
         下拉框默认单选, 提交的参数 name=value(被选中option提供的)
    
       #textarea标签 (文本域)
        1. name属性
        2. cols : 显示的列数
        3. rows : 显示的行数
    
    -->
        <form action="http://www.baidu.com" method="get">
            地区
            <select name="area">
                <option value="1">福建</option>
                <option value="2">广东</option>
                <option value="3">上海</option>
            </select> <br>
            自我介绍 <br>
            <textarea name="self"  cols="30" rows="3"></textarea> <br>
            <input type="submit">
        </form>
    
    </body>
    </html>

CSS

---

    # 今日目标
    1. 理解CSS的基础语法
    2. 会使用CSS基本选择器
    3. 会使用常见的CSS样式



一 CSS概述

层叠样式表（Cascading Style Sheet）

作用：给html标签添加样式, 达到美化页面的目的

层叠样式: 对同一个标签添加多个不同的样式,所有样式会叠加在一起展示出效果



初体验

    <!DOCTYPE html>
    <html lang="zh-CN">
    <head>
        <meta charset="UTF-8">
        <title>Title</title>
        <!--
            css 层叠样式表
            1. 层叠
            2. 样式表: 给html添加样式的一种语言
    
            问题: html属性也可以给html标签添加样式,为啥还需要css呢?
                css更专业
             1. html属性有的,css都有,html属性没有的css也有
             2. 分工更加明确,html专注网页的布局构造, css 专注网页美化,代码更清晰
        -->
        <style>
            div{
                color : red;
            }
            h1{
                color : green;
            }
            span{
                color : deeppink;
                font-size: 50px;
                font-family: 楷体;
            }
        </style>
    </head>
    <body>
            <div>div</div>
            <h1>正文标题</h1>
            中文
            <font color="blue" size="8" face="楷体">中文1</font>
            <font color="blue" size="7" face="楷体">中文2</font>
            <font color="blue" size="7" face="楷体">中文3</font>
            <hr>
            <span>中文4</span>
            <span>中文5</span>
            <span>中文6</span>
    </body>
    </html>



优点

    1. 实现了样式和内容的分离，提高了显示效果和样式的复用性。
    
    2. 降低耦合性，分工更加明确，CSS专门用于美化，HTML专门用于结构搭建。



二 CSS基础语法【看懂】

2.1 HTML引入CSS

    <!DOCTYPE html>
    <html lang="zh-CN">
    <head>
        <meta charset="UTF-8">
        <title>01-HTML引入CSS</title>
        <!--
            html中引入css的三种方式
            0. css必须要引入到html中才会运行
            1. 行内样式
                1). 以属性的方式写在html标签中,只对当前行其作用
                2). 每个标签都有style属性
                3). style= css属性
                  css属性语法 -> css属性名 : 值;
                                css属性名 : 值...
    
            2. 内部样式
                1). 在当前html内部声明的css样式
                2). 书写一个style标签,内部编写css(推荐放在head标签)
                3). css语法
                    选择器{
                        css属性名 : 值;
                                css属性名 : 值...
                    }
    
            3. 外部样式
                 1). 使用在当前html外部声明的css样式
                 2). 先书写一个css文件,内部编写css  (推荐放在css文件夹)
                 3). 用link标签进行引入
                     <link rel="stylesheet" href="css文件的位置">
                        rel : relationship 关系
    
            # 优先级
                行内 > 内部 = 外部
                原因: 网页加载html,从上之下加载,后加载覆盖先加载
    
            # 解释 层叠
                多处设置,只要不冲突,就可以叠加在一起
        -->
    
        <style>
            div{
                color : green;
                font-size: 40px;
            }
            span{
                color : blue;
            }
        </style>
        <link rel="stylesheet" href="../css/my.css">
    
    </head>
    <body>
            div
            <div style="color: red;font-size: 30px">div</div>
            <div>div</div>
            <div>div</div>
            <span style="font-size: 50px">span</span>
    </body>
    </html>



2.2 CSS书写规范

    <!DOCTYPE html>
    <html lang="zh-CN">
    <head>
        <meta charset="UTF-8">
        <title>02-CSS语法</title>
        <style>
            span{
                color: red;
                font-size: 30px;
                /*
                    边框: 1px宽 绿色 实线
                */
                border: 1px green solid
            }
        </style>
    </head>
    <body>
    <!--
    
    -->
    <span>样式名多个单词用横杠分割</span><br/>
    <span>样式值多个单词用空格分割</span><br/>
    <span>多个样式之间，以分号分割</span><br/>
    </body>
    </html>





2.3 基本选择器

    <!DOCTYPE html>
    <html lang="zh-CN">
    <head>
        <meta charset="UTF-8">
        <title>03-基本选择器</title>
    
        <style>
            /*
                内部样式/外部样式 有的, 但是行内样式没有
    
                # 三大基本选择器 (selector)
                  0. 作用: 通过选择器,定位html中的一些标签
    
                  1. id选择器
                       1). 每个标签都有id属性,属性值必须唯一
                       2). 语法
                            #id值
                            #boss -> 选中id=boss的标签
                       3). 特点: 一般只选中一个标签
    
                  2. class选择器 -> 类加载器
                       1). 每个标签都有class属性,属性值可以重复,而且还可以设置多个值
                       2). 语法
                            .class值
                             .female -> 选中class=female的一组标签
    
                  3. 标签选择器
                      语法: 标签名
    
               选择器优先级:
                    id > class > 标签
    
                    特点: 定位越精确, 优先级越高
            */
            #boss{
                color:red;
                font-size: 50px;
            }
            .female{
                color : green;
            }
            .hero{
                font-size: 30px;
            }
            span{
                font-size: 10px;
            }
        </style>
    </head>
    <body>
    
    <span>马尔扎哈</span>
    <span class="female">古力娜扎</span>
    <span class="female">迪丽热巴</span>
    <span class="female hero">黑寡妇</span>
    
    <span class="male hero">钢铁侠</span>
    <span class="male hero">超人</span>
    
    
    <span id="boss">灭霸</span>
    
    
    </body>
    </html>

三 CSS常用样式【了解】

3.1 字体和文本属性

    <!DOCTYPE html>
    <html lang="zh-CN">
    <head>
        <meta charset="UTF-8">
        <title>05-字体和文本属性</title>
        <style>
            /*
            渲染需求 (绘制)
                1.所有文字绿色
                2.所有文字大小20px
                3.所有行高40px
                4.所有字体加粗
                5.所有字体楷体
                6.第一句文字倾斜
                7.第一句隐藏下划线
            */
            div{
                color : green;
                font-size: 20px;
                line-height: 40px;
                font-weight: bold;
                font-family: 楷体;
            }
            a{
                font-style: italic;
                text-decoration: none;
            }
            a:link{
                color: pink;
            }
        </style>
    
    </head>
    <body>
    <div>
        <p>
            <a href="#"> 学习的误区：</a><br/>
            眼睛：看了一遍记住了<br/>
            耳朵：听了一遍明白了<br/>
            脑子：想了一遍搞懂了<br/>
            手：你们会个屁！^_^ <br>
        </p>
    </div>
    </body>
    </html>





3.2 案例：公司简介(作业)





    <!DOCTYPE html>
    <html lang="zh-CN">
    <head>
        <meta charset="UTF-8">
        <title>06-案例：公司简介</title>
    
        <style>
            p{
                text-indent: 2em;
            }
            span{
             color: red;
            }
            #myspan{
                font-weight: bold;
                font-style: italic;
                color: black;
            }
            div{
                color: grey;
                font-size: 15px;
    
            }
        </style>
    </head>
    <body>
    
        <h1 align="center">公司简介</h1>
    <hr color="orange">
        <p>
    <span>“中关村黑马程序员训练营”</span>是由 <span id="myspan">传智播客</span>联合中关村软件园、CSDN， 并委托传智播客进行教学实施的软件开发高端培训机构，致力于服务各大软件企业，解决当前软件开发技术飞速发展， 而企业招不到优秀人才的困扰。
    目前，“中关村黑马程序员训练营”已成长为行业“学员质量好、课程内容深、企业满意”的移动开发高端训练基地， 并被评为中关村软件园重点扶持人才企业。
        </p>
        <p>
    黑马程序员的学员多为大学毕业后，有理想、有梦想，想从事IT行业，而没有环境和机遇改变自己命运的年轻人。 黑马程序员的学员筛选制度，远比现在90%以上的企业招聘流程更为严格。任何一名学员想成功入学“黑马程序员”， 必须经历长达2个月的面试流程，这些流程中不仅包括严格的技术测试、自学能力测试，还包括性格测试、压力测试、 品德测试等等测试。毫不夸张地说，
    黑马程序员训练营所有学员都是精挑细选出来的。百里挑一的残酷筛选制度确 保学员质量，并降低企业的用人风险。
        </p>
    <p>
    中关村黑马程序员训练营不仅着重培养学员的基础理论知识，更注重培养项目实施管理能力，并密切关注技术革新， 不断引入先进的技术，研发更新技术课程，确保学员进入企业后不仅能独立从事开发工作，更能给企业带来新的技术体系和理念。
    </p>
        <p>
    一直以来，黑马程序员以技术视角关注IT产业发展，以深度分享推进产业技术成长，致力于弘扬技术创新，倡导分享、 开放和协作，努力打造高质量的IT人才服务平台。
        </p>
        <hr color="orange">
        <div align="center">
    江苏传智播客教育科技股份有限公司 版权所有Copyright 2006-2020, All Rights Reserved 苏ICP备16007882
        </div>
    </body>
    </html>





3.3 背景属性

    <!DOCTYPE html>
    <html lang="zh-CN">
    <head>
        <meta charset="UTF-8">
        <title>07-背景属性</title>
        <!--
            background : 背景
    
        -->
        <style>
            body{
                background-color: pink;
                background-image: url("../img/a.jpg");
                background-repeat: no-repeat;
                background-position: 10px 20px;
            }
        </style>
    </head>
    <body>
    
    </body>
    </html>







3.4 显示属性

    <!DOCTYPE html>
    <html lang="zh-CN">
    <head>
        <meta charset="UTF-8">
        <title>08-显示属性</title>
    
        <style>
            /*
                display : 展示
                    1. block : 块级 (自动换行)
                    2. inline : 本行 (不会自动换行)
                    3. none : 隐藏
            */
            span{
                display: block;
            }
            div{
                display: none;
            }
            li{
                display: inline;
            }
        </style>
    
    </head>
    <body>
    
        <span>内联标签span1</span>
        <span>内联标签span2</span>
        <span>内联标签span3</span>
        <div>块级标签div1</div>
        <div>块级标签div2</div>
        <div>块级标签div3</div>
    
        <ul>
            <li>美的</li>
            <li>苏宁</li>
            <li>格力</li>
        </ul>
    </body>
    </html>





