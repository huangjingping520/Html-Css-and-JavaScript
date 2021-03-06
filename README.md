<!-- TOC -->

- [Html](#html)
    - [超文本标记语言](#超文本标记语言)
    - [作用](#作用)
    - [文件后缀](#文件后缀)
    - [特点](#特点)
    - [标签](#标签)
    - [元素](#元素)
    - [Html 的属性](#html-的属性)
    - [注释](#注释)
    - [基本结构](#基本结构)
    - [常用标签](#常用标签)
        - [标题](#标题)
        - [段落](#段落)
        - [强制换行<br/>](#强制换行br)
        - [水平线<br>](#水平线br)
        - [图片](#图片)
        - [文本格式化标签](#文本格式化标签)
        - [列表<br>](#列表br)
        - [表格<br>](#表格br)
        - [Form 表单](#form-表单)
        - [文件](#文件)
        - [隐藏域](#隐藏域)
        - [图片提交按钮](#图片提交按钮)
        - [下拉列表](#下拉列表)
        - [多行文本框](#多行文本框)
        - [<font color=red>H5新增内容</font>](#font-colorredh5新增内容font)
            - [新增标签](#新增标签)
            - [新增属性](#新增属性)
        - [`<div>`和`<span>`</br>](#div和spanbr)
        - [超链接](#超链接)
        - [特殊字符](#特殊字符)
    - [语义化标签](#语义化标签)
        - [优势](#优势)
        - [H5新增语义化标签](#h5新增语义化标签)
- [CSS](#css)

<!-- /TOC -->
# Html

## 超文本标记语言

- HyperText Markup Language

## 作用

- 写网页界面结构

## 文件后缀

- .html、.htm

## 特点

- Html 不区分大小写，建议小写
- Html 由浏览器解析执行，由上往下，由左往右
- HTML 标签之间可以相互嵌套

## 标签

- 定义：Html 由标签组成，包含在尖括号之间的内容
- 分类
  - 单标签 封闭类型标签
  - 双标签 非封闭类型标签 空标签

## 元素

- 指开始标签到结束标签之间的内容

## Html 的属性

- 描述 html 标签
- 双标签写在开始标签里面
- 一个标签有多个属性，且不区分前后顺序

## 注释

- `<!-- -->`
- 注释中的内容不会显示在浏览器之中

## 基本结构

- `<!DOCTYPE>` 文档类型声明（<font color = red>不是 html 标签</font>）<br>
  作用：告诉浏览器按当前标注解析代码<br>

  > W3C 标准之前，不同的浏览器对于页面的渲染有着不同的标准且存在差异，该模式称为**<font color = red>混杂模式</font>**；W3C 标准出现之后，浏览器对于页面的渲染有了统一的标准，称为**<font color = red>标准模式</font>**

    <hr>

  > <!doctype>不存在或者形式错误会使得HTML以混杂模式呈现，所以<!doctype>对于浏览器的兼容性有着重要意义

  目前使用的<!doctype html>属于 HTML5 标准，不区分大小写，双标记的结束标记可以省略（但是不建议省略）

  HTML4.01 ==> 严格、过渡、框架集

  XHTML ==> 严格的 HTML，区分大小写，结束标记必须写上

  DTD：文档类型声明，等同于 DOCTYPE

- head<br>
  `<title>` 网页标题<br>
  `<meta>` 用以告知文档的附加信息<br>
  > charset : 字符集 中文开发网站常用 UTF-8<br>
  > name：<br>
  > content：<br> > `<head lang="en">` lang 表示告知网页主要语言
- body<br>
  网站内容

## 常用标签

### 标题

```html
<h1 align="center">一级标题</h1>
<!-- 
    属性：
    align:水平对齐方式
        属性值：
        left:居左（默认值）
        center：居中
        right：居右
    title：鼠标悬停时候显示的文字
-->
<h2>二级标题</h2>
<h3>三级标题</h3>
<h4>四级标题</h4>
<h5>五级标题</h5>
<h6>六级标题</h6>
```

### 段落

```html
<p>段落内容</p>
<!-- 
    属性：
    align:水平对齐方式
        属性值：
        left:居左（默认值）
        center：居中
        right：居右
-->
```

### 强制换行<br/>
`<br/>`没有任何属性

### 水平线<br>

- 分割上下文
```html
<hr />
<!-- 
属性：
color:颜色
width:宽度  设置水平方向（默认单位是px）
size:尺寸  设置垂直方向（默认单位是px）
align:水平对齐方式
    属性值：
    left:居左
    center：居中（默认值）
    right：居右
-->
```

### 图片

```html
<img src="" alt="" />
<!--
    路径：
        绝对路径：
        1. 网址
        2. 盘符
        相对路径：
        1. 平级  直接写
        2. 下一级  / + 名称
        3. 上一级  ../ + 名称
           上两级  ../../ + 名称
    常用图片格式：
        jpg/jpeg
        png（支持背景透明）
        gif（支持动图）
        psd（ps中保存的图片）
    alt：
        图片无法显示的时候显示的文字描述
    title：
        鼠标悬停的时候显示的文字描述
    width/height：宽度/高度
        当只设置一个的时候，图片的两个属性 会相同
-->
```

### 文本格式化标签

![](https://cdn.jsdelivr.net/gh/huangjingping520/PicGo/文本格式化.png)

### 列表<br>

1. 无序列表
```html
基础结构：
<ul>
  <li></li>
</ul>
ul 和 li 的属性： 
type：设置项目符号的类型 取值： disc 黑色实心圆 circle
空心圆 square 实心矩形 none 不显示
```
2. 有序列表
```html
<ol>
  <li></li>
</ol>
属性： 
type：设置符号的类型 1、a、A、I... start：设置起始序号 reversed：倒序
```
3. 自定义列表
```html
<dl>
  <dt>主题</dt>
  <dd>描述</dd>
</dl>
```

### 表格<br>
`<caption>`标题<br>
`<tr>`行<br>
`<td>`列<br>
`<th>`表头：居中加粗<br>

```html
<table border="5" align="center" width="600">
  <caption>
    信息表
  </caption>
  <tr bgcolor="pink">
    <th colspan="3">学生基本信息</th>
    <th colspan="2">成绩</th>
  </tr>
  <tr>
    <th>姓名</th>
    <th>性别</th>
    <th>专业</th>
    <th>课程</th>
    <th>分数</th>
  </tr>
  <tr align="center">
    <td>球球</td>
    <td>男</td>
    <td rowspan="2">计算机</td>
    <td rowspan="3">程序设计</td>
    <td>68</td>
  </tr>
  <tr align="center">
    <td>喃喃</td>
    <td>女</td>
    <td>89</td>
  </tr>
  <tr align="center">
    <td>小明</td>
    <td>男</td>
    <td>会计</td>
    <td>68</td>
  </tr>
  <tr align="center">
    <td>小明</td>
    <td>男</td>
    <td>建筑</td>
    <td>建筑设计</td>
    <td>68</td>
  </tr>
</table>
```
效果：
<table border="5" align="center" width="600">
    <caption>信息表</caption>
    <tr bgcolor="pink">
        <th colspan="3">学生基本信息</th>
        <th colspan="2">成绩</th>
    </tr>
    <tr>
        <th>姓名</th>
        <th>性别</th>
        <th>专业</th>
        <th>课程</th>
        <th>分数</th>
    </tr>
    <tr align="center">
        <td>球球</td>
        <td>男</td>
        <td rowspan="2">计算机</td>
        <td rowspan="3">程序设计</td>
        <td>68</td>
    </tr>
    <tr align="center">
        <td>喃喃</td>
        <td>女</td>
        <td>89</td>
    </tr>
    <tr align="center">
        <td>小明</td>
        <td>男</td>
        <td>会计</td>
        <td>68</td>
    </tr>
    <tr align="center">
        <td>小明</td>
        <td>男</td>
        <td>建筑</td>
        <td>建筑设计</td>
        <td>68</td>
    </tr>
</table>

  表格结构标签：<br>
    `<thead>`表格的头部区域<br>
    用于定义表格头部，其内部必须拥有`<tr>`标签,一般位于第一行<br>
    `<tbody>`表格的主体区域<br>
    用于定义表格的主体，主要用于放数据本体

### Form 表单

1. 作用：提交数据使页面具有交互性
2. form 之间不可相互嵌套
3. 标签：<br>
   属性：<br>
   action:提交的地址<br>
   name:表单名称<br>
   method:提交的方式 GET/POST<br> 1. GET 提交数据不安全，会在地址栏显示；POST 不会<br> 2. GET 提交数据大小有限制（不能大于 2kb）；POST 理论上没有限制
```html
<form action="" name="Login">
  姓名：<input type="text" name="username" />
  <!-- text:单行完本框 -->
  <br />
  密码：<input type="password" name="password" />
  <!-- password:密码，不显示内容 -->
  <br />
  性别：<input type="radio" name="sex" />男
  <input type="radio" name="sex" />女
  <!-- radio:单选框，但是选择后不消失，所以必须加上name -->
  <br />
  爱好：<input type="checkbox" name="lovelything" />唱
  <input type="checkbox" name="lovelything" />跳
  <input type="checkbox" name="lovelything" />rap
  <input type="checkbox" name="lovelything" />篮球
  <!-- checkbox:多选框 -->
  <br />
  <input type="submit" value="登录" />
  <!-- submit:提交，默认GET value:修改显示文字-->
  <input type="reset" />
  <!-- reset:重置 同样可以使用value修改文字 -->
  <input type="button" value="无功能" />
  <!-- button:按钮样式，无功能 -->
  <button>提交</button>
  <!-- button（标签）默认属性submit，同样也可以使用  reset等属性 -->
</form>
```
**效果：**


      <form action="" name="Login">
          姓名：<input type="text" name="username">
          <!-- text:单行完本框 -->
          <br>
          密码：<input type="password" name="password">
          <!-- password:密码，不显示内容 -->
          <br>
          性别：<input type="radio" name="sex">男<input type="radio" name="sex">女
          <!-- radio:单选框，但是选择后不消失，所以必须加上name -->
          <br>
          爱好：<input type="checkbox" name="lovelything">唱
          <input type="checkbox" name="lovelything">跳
          <input type="checkbox" name="lovelything">rap
          <input type="checkbox" name="lovelything">篮球
          <!-- checkbox:多选框 -->
          <br>
          <input type="submit" value="登录">
          <!-- submit:提交，默认GET value:修改显示文字-->
          <input type="reset">
          <!-- reset:重置 同样可以使用value修改文字 -->
          <input type="button" value="无功能">
          <!-- button:按钮样式，无功能 -->
          <button>提交</button>
          <!-- button（标签）默认属性submit，同样也可以使用reset等属性 -->

### 文件

`````html
<form name="form" enctype="multipart/form-data">
    <!--当需要使用文件时，需要更改form表单的编码格式，即enctype="multipart/form-data"-->
    <p>
        文件：<input type="file">
    </p>
</form>
`````

### 隐藏域

定义隐藏字段隐藏字段对用户不可见。常常用来存储默认值，或者由JavaScript改变它们的值

````html
<form>
    <p>
        <input type="hidden">
    </p>
</form>
````

### 图片提交按钮

```html
<form>
    <p>
        <input type="image">
    </p>
</form>
```

### 下拉列表

````html
<form>
    <select name="city">
        <option>北京</option>
        <option>上海</option>
        <option>南京</option>
        <option>湖南</option>
        <option>河北</option>
    </select>
</form>
````

<form>
    <select name="city">
        <option>北京</option>
        <option>上海</option>
        <option>南京</option>
        <option>湖南</option>
        <option>河北</option>
    </select>
</form>

```html
<form>
    <select name="city">
        <optiongroup label="北京">
        	<option>朝阳</option>
            <option>海淀</option>
            <option>大兴</option>
        </optiongroup>
        <optiongroup label="江西">
        	<option>南昌</option>
            <option>抚州</option>
            <option>赣州</option>
        </optiongroup>
    </select>
</form>
```

<form>
    <select name="city">
        <optgroup label="北京">
        	<option>朝阳</option>
            <option>海淀</option>
            <option>大兴</option>
        </optiongroup>
        <optgroup label="江西">
        	<option>南昌</option>
            <option>抚州</option>
            <option>赣州</option>
        </optiongroup>
    </select>
</form>

### 多行文本框

```html
<textarea name="留言" cols="30" rows="10">

</textarea>
```

留言：

<textarea name="留言" cols="30" rows="10"></textarea>

### <font color=red>H5新增内容</font>

#### 新增标签

1. 邮箱

```html
<input type="email">
```

2. 网址

```html
<input type="url">
```

3. 搜索

```html
<input type="search">
```

4. 数字

```html
<input type="number" max="" min="" step="">
```

5. 范围（滑块）

```html
<input type="range" max="" min="" value="初始值" step="">
```

6. 颜色

```html
<input type="color">
```

7. 电话

```html
<input type="tel">
```

8. 日期

```html
<input type="date">
```

9. 周

```html
<input type="week">
```

10. 月

```html
	<input type="mouth">
```

#### 新增属性

1. placeholder--默认提示

   ```html
   <p>
       用户名：<input type="text" placeholder="用户名/手机/邮箱"
   </p>
   ```

   效果：

   <p>
       用户名：<input type="text" placeholder="用户名/手机/邮箱"
   </p>

2. autofocus--自动聚焦

3. required--必填项

4. multiple--可以输入多个内容，用`,`隔开

5. minlength

6. maxlength


### `<div>`和`<span>`</br>  

- 两者没有语义，只是一个盒子用来装内容的
    1. div标签用来布局，但一行只能放一个div，即`<div>`标签独占一行
    2. span同样用来布局，但一行可以有多个span    

### 超链接

  ```html
  <a href="" target=""></a>
  href:必须属性，用于指定连接目标的url
  target:用于指定链接的打开方式，_self在当前页面打开（默认值），_blank在新窗口打开
  ```
分类:
1. 外部链接：如

```html
<a href="https://www.baidu.com">百度</a>
```
2. 内部链接：网站内部页面的相互链接，直接链接内部页面名称即可。如

  ```html
  <a href="index.html">首页</a>
  ```

 3. 空链接：如果当时没有确定链接目标时，使用空链接<br>
  ```html
  <a href="#">首页</a>
  ```

4. 下载链接：如果href中的地址是一个文件或者压缩包，则会下载这个文件
  5. 网页元素链接：在网页中的各种网页元素，如文本、图像、表格、音频、视频等都可以添加超链接
  ```html
  <a href="https://www.baidu.com"><img src=img.jpg></a>
  ```
  6. 锚点链接：当我们点击链接，可以快速定位到页面中的某个位置

```html
(1) 在链接文本的href中，设置属性值为“#名字”的形式，如
<a href="#two">第二集</a>
(2)找到目标位置标签，里面添加一个id属性=名字，如
<h3 id="two">第二集</h3>
```
### 特殊字符

如下表
![](https://cdn.jsdelivr.net/gh/huangjingping520/PicGo/特殊字符.JPG)

## 语义化标签

语义化标签，旨在让标签有着自己的含义

### 优势

1. 代码结构清晰，方便阅读，有利于团队开发
2. 方便其他设备解析，以语义的方式来渲染网页
3. 有利于搜索引擎优化(SEO)

### H5新增语义化标签

<font color="red">Html5新增元素IE 6 7 8 （即低版本IE）都不支持</font>

<img src="https://cdn.jsdelivr.net/gh/huangjingping520/PicGo/div%E4%B8%8Eh5%E5%AF%B9%E6%AF%94.PNG" style="zoom: 80%;" />

一、 布局标签

1. header 头部
2. nav 导航
3. footer 页脚
4. aside 侧边栏
5. article 文章、帖子
6. section 章节

二、 视频与音频

1. video--定义视频，如电影片段或者其他视频流

   <img src="https://cdn.jsdelivr.net/gh/huangjingping520/PicGo/H5%E8%A7%86%E9%A2%91%E7%9A%84%E5%B1%9E%E6%80%A7.PNG" style="zoom: 80%;" />

2. audio--定义音频，如音乐或其他音频流

   <img src="https://cdn.jsdelivr.net/gh/huangjingping520/PicGo/20210304222521.png" style="zoom:80%;" />

3. source-- 媒介元素定义媒介资源

   允许规定可替换的视频/音频文件供浏览器根据它对媒体类型或者编解码器的支持进行选择

三、新增标签

1. figure--用于对元素进行组合，多用于图片与图片描述的组合

2. details--用于描述文档或文档的某个部分的细节，类似于下拉列表，兼容性比较差

   ```html
   <details>
   	<summary>描述</summary>
       <p>
           123456789
       </p>
   </details>
   ```

   效果：

   <details>
   	<summary>描述</summary>
       <p>
           123456789
       </p>
   </details

3. mark-- 主要用来在视觉上向用户呈现那些需要突出的文字

4. meter--（刻度）定义度量衡，仅用于已知最大值和最小值的度量

   1. low：最低临界点
   2. high：最高临界点
   3. min：最小值
   4. max：最大值
   5. value：当前值

5. progress--（进度条）运行中的进程，可以用progress标签来显示Javascript中耗费时间的函数的进程

6. datalist--定义可选数据的列表。

   与input元素配合，就可以制作出输入值的下拉列表。

   datalist及其选项不会被显示出来，仅仅是合法的输入值列表

7. canvas--定义图形，如图标和其他图像。

   该标签是为了客户端矢量图设计的，其本身没有行为，但却把一个绘图API展现给JavaScript以使脚本能够把想绘制的东西 都绘制到一块画布上

# CSS

## 作用

1. 让网页具有美观一致的页面
2. 内容与格式分离

## 概念

CSS(Cascading Style Sheets)层叠样式表，又叫级联样式表

1. 用于HTML文档中元素样式的定义

   实现了将内容与表现分离

   提高代码的可重用性和可维护性

2. .css

## 特征

<img src="https://cdn.jsdelivr.net/gh/huangjingping520/PicGo/css%E7%89%B9%E7%82%B9.PNG" style="zoom:80%;" />

## CSS引入方式

1. 内联样式----只对当前元素生效

   由于将表现和内容混杂在一起，内联样式会损失掉样式表的许多优势。<font color="red">慎用！！！</font>

   要使用内联样式，需要在相关的标签内使用样式（style）属性。Style属性可以包含任何CSS属性

   **缺乏整体性和规划性，不利于维护，维护成本高**

   ```html
   <p style="background:pink;color:red;font-size:25px;">
       CSS
   </p>
   ```

   效果：

   <p style="background:pink;color:red;font-size:25px;">
       CSS
   </p>

2. 内部样式----只对当前页面生效

   当单个文档需要特殊的样式时，就应该使用内部样式表。可以使用`<style>`标签在文档头部定义内部样式表

   ```html
   <head>
       <style>
           选择器{
               属性:属性值;
               属性:属性值;
               属性:属性值;
               属性:属性值;
               属性:属性值;
           }
       </style>
   </head>
   ```

   选择器的作用：选中写样式的元素


3. 外部样式--实现了内容与表现的分离，提高了代码的可重用性和可维护性
   
   1. 新建`.css`文件
   
      同一个`.css`可以被多个html引入
   
   2. 在`head`中用`link`引入
   
      ```html
      <link rel="stylesheet" href=".css">
      ```
   
4. 导入式--不推荐使用

   ```html
   <head>
       <style>
       	@import ".css";
       </style>
   </head>
   或者
   <head>
       <style>
       	@import url(".css");
       </style>
   </head>
   ```

   **@import与link的区别：**

   1. 加载顺序不同

      @import会先加载html再加载css

      link则是同时加载

   2. 