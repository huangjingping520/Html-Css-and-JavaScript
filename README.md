# Html
### 超文本标记语言
- HyperText Markup Language
### 作用
- 写网页界面结构
### 文件后缀
- .html、.htm
### 特点
- Html不区分大小写，建议小写
- Html由浏览器解析执行，由上往下，由左往右
- HTML标签之间可以相互嵌套
### 标签
- 定义：Html由标签组成，包含在尖括号之间的内容
- 分类
    - 单标签 封闭类型标签
    - 双标签 非封闭类型标签 空标签
### 元素
- 指开始标签到结束标签之间的内容
### Html的属性
- 描述html标签
- 双标签写在开始标签里面
- 一个标签有多个属性，且不区分前后顺序 
### 注释
- `<!--  -->`
- 注释中的内容不会显示在浏览器之中
### 基本结构
- `<DOCTYPE>` 文档类型声明（<font color = red>不是html标签</font>）<br>
    作用：告诉浏览器按当前标注解析代码<br>
    > W3C标准之前，不同的浏览器对于页面的渲染有着不同的标准且存在差异，该模式称为**<font color = red>混杂模式</font>**；W3C标准出现之后，浏览器对于页面的渲染有了统一的标准，称为**<font color = red>标准模式</font>**
        
    <hr>

    > <!doctype>不存在或者形式错误会使得HTML以混杂模式呈现，所以<!doctype>对于浏览器的兼容性有着重要意义
        
    目前使用的<!doctype html>属于HTML5标准，不区分大小写，双标记的结束标记可以省略（但是不建议省略）

    HTML4.01 ==> 严格、过渡、框架集

    XHTML ==> 严格的HTML，区分大小写，结束标记必须写上

    DTD：文档类型声明，等同于DOCTYPE
- head<br>
    `<title>` 网页标题<br>
    `<meta>` 用以告知文档的附加信息<br>
    > charset : 字符集 中文开发网站常用UTF-8<br>
    > name：<br>
    > content：<br>
    
     `<head lang="en">` lang 表示告知网页主要语言
- body<br>
    网站内容
### 常用标签
1. 标题
    ```html
    <h1 align = "center">一级标题</h1>
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
2. 段落
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
3. 强制换行<br/>
    `<br/>`没有任何属性
4. 水平线<br>
    - 分割上下文
    ```html
    <hr/>
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
5. 图片
    ```html
    <img src="" alt="">
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
            当今设置一个的时候，图片两者会相同
    -->
    ```
6. 文本格式化标签

    ![](https://cdn.jsdelivr.net/gh/huangjingping520/PicGo/文本格式化.png)
7. 列表<br>
    1. 无序列表
    > 在文字前有一个黑点 
    ```html
    基础结构：
    <ul>
        <li></li>
    </ul>
    a：超链接
    <ul>
        <li>
            <a href="链接地址" target = "_blank"(新窗口)></a>
        </li>
    </ul>
    
    ```