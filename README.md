<!--
 * @Author: MerlinAlex
 * @Date: 2020-10-27 22:00:21
 * @LastEditTime: 2021-02-03 22:01:03
 * @LastEditors: Please set LastEditors
 * @Description: In User Settings Edit
 * @FilePath: \Html-Css-and-JavaScript\README.md
-->
# Html
- 超文本标记语言
    - HyperText Markup Language
- 作用
    - 写网页界面结构
- 文件后缀
    - .html、.htm
- Html不区分大小写，建议小写
- Html由浏览器解析执行，由上往下，由左往右
- 标签
    - 定义：Html由标签组成，包含在尖括号之间的内容
    - 分类
        - 单标签 封闭类型标签
        - 双标签 非封闭类型标签 空标签
- 元素
    - 指开始标签到结束标签之间的内容
- Html的属性
    - 描述html标签
    - 双标签写在开始标签里面
    - 一个标签有多个属性，且不区分前后顺序 
- HTML标签之间可以相互嵌套
- 注释
    - `<!--  -->`
    - 注释中的内容不会显示在浏览器之中
- 常用标签
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
    -->
    ```
    