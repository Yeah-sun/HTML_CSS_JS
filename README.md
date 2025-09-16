# HTML_CSS_JS
前端三件套(用的webstorm)
* [x] HTML5
* [ ] CSS3
* [ ] JavaScript
* [ ] 实战项目
    * 火柴人
    * 跳动的心
    * 小米商城
---
## HTML5
&emsp; HTML5是用来描述网页的一种语言,被称为超文本标记语言,用HTML5编写的文本,后缀以.html结尾.
HTML5是一种**标记**语言,标记语言是一套标记标签(这是重点理解).标签是由尖括号包围的关键字, 列如:`<html>`.  
标签有两种格式:
1. 双标签,例如: `<html></html>`
2. 单标签,例如: `<img>`

### HTML5的DOCTYPE声明  
&emsp;DOCTYPE是 `document type` 的缩写.`<!DOCYTPE html>`是H5的声明位于文档的最前面,处于标签之前.他是网站必备的组成部分,避免浏览器的怪异模式:  
```<!DOCTYPE html>```

![](./image/DOCTYPE.png)
### [HTML5的基本框架](./HTML5/01_welcome.html)
#### html标签
&emsp;定义HTML文档,这个元素我们浏览器看到后就明白这个HTML文档了,所以你的其他元素要包括在里面.
该标签限定了文档的开始点和结束点.
```html
<!DOCTYPE html>
<html lang="en">
</html>
```
#### head标签
&emsp;head标签用于定义文档的头部.文档的头部描述了文档的各种属性和信息,包括文档的标题,web中的位置以及其他文档的关系等.  
绝大多数的文档头部包含的数据不会真正作为内容显示给读者.大部分是给开发者和浏览器看的.
```html
<!DOCTYPE html>
<html lang="en">
    <head>
    </head>
</html>
```
#### body标签
* body元素定义文档的主体.
* body元素包含文档的所有内容 (比如文本,超链接,图像,表格和列表等.)
* 它会直接在页面显示出来,也就是用户直观看到的内容.
```html
<!DOCTYPE html>
<html lang="en">
    <head>
    </head>
    <body>
        welcome
    </body>
</html>
```
#### title标签
* 可定义文档的标题.
* 它显示在浏览器窗口的标题栏或状态栏上.
* `<title></title>` 标签是 `<head></head>`标签中唯一必须要求包含的东西,就是说写head一定要写title.
* `<title></title>`的增加有利于SEO优化.
> SEO是搜索引擎优化的英文缩写.通过网站的内容调整,满足引擎的排名需求.
```html
<!DOCTYPE html>
<html lang="en">
    <head>
        <title>第一个界面</title>
    </head>
    <body>
        welcome
    </body>
</html>
```
#### meta标签
* meta标签用来描述一个HTML网页文档的属性,关键词等.
* 例如: `charset= "UTF-8"`是说当前使用的是`UTF-8`编码格式,在开发中我们经常看到`UTF-8`,或者是`GBK`,这些都是编码格式.
```html
<!DOCTYPE html>
<html lang="en">  <!--这个lang是代表语言,en是指英文-->
    <head>
        <meta charset="UTF-8"> <!--显然 meta 是一个单标签-->
        <title>第一个界面</title>
    </head>
    <body>
        welcome
    </body>
</html>
```
### 标签(标题 段落 换行 水平线 图片 超文本链接 文本 列表 表格 块行 )
#### [标题](./HTML5/02_标题.html)
* 标题是一个双标签.
* 标题(Heading) 是通过 `<h1>~<h6>`标签来定义的.
* `<h1></h1>`定义最大的标签,`<h6></h6>`定义最小的标签.
```html
<h1>一级标题</h1>
<h2>二级标题</h2>
<h3>三级标题</h3>
<h4>四级标题</h4>
<h5>五级标题</h5>
<h6>六级标题</h6>
```
* **正确使用标题**
  * 确保HTML标题标签只用于标题.
  * 应该将 `<h1>` 用作主标题,其他重要性依次递减.
* **标题标签位置摆放**  
  * 在标签中添加属性: `align = "left|center|right"` 默认都是居左的.  
  * 应该会提示你,这个已经被废弃了,后续学CSS会有更好的.

#### 段落,换行,水平线
* 段落是通过 `<p></p>` 标签定义的
  ```html
  <p> 这是一个段落 </p>
  <p> 这是另一个段落 </p>
  ```
* 换行(如果您希望在不产生一个新段落的情况下进行换行),请使用 `<br>` ->这是一个单标签且是一个空的HTML元素.
  ```html
  <p>这个<br>段落有<br>分行效果</p>
  ```
* 水平线 `<hr/>` 标签在HTML页面中创建水平线,单标签
    * color:   设置水平颜色
    * width:   设置水平线的像素宽度
    * size:    设置水平线的像素高度
    * align:   设置水平线的对齐方式(默认居中),可取值left|right
  ```html
  <hr color = ""  width = "" size = "" align = ""/>
  ```
#### 图片
* `<imag>`标签定义HTML页面中的图像  
  ```html
  <img src="" alt="" title="" width="" height="" >
  ```
  > **注意事项**
  > `<img>`是单标签,不需要闭合
* 属性
  * `src=""`:路径(图片地址与名字)
  * `alt=""`:规定图像的替代文本
  * `width=""`:规定图片的宽度 
  * `height=""`:规定图片的高度
  * `title=""`:鼠标悬停在图片上给予提示
* 图片路径详解:
  * 绝对路径
    * 绝对路径是电脑的盘符与访问的具体地址
    * `E:\single_variable_calculs\ppt_course\lec1.jpg` 
    * `<img src="E:\single_variable_calculs\ppt_course\lec1.jpg" alt="">`

  * 相对路径
    * 两者相对关系,两者在同一路径下可以直接访问
    * 子级关系:`/`
    * 父级关系:`../`
    * 同级关系:`./` 
  * 网络路径  
    * 具体网络地址
#### 超文本链接
&emsp;HTML使用标签`<a></a>`来设置超文本链接
&emsp;超链接可以是一个字,一个词,或者一组词,也可以是一幅图像,您可以点击这些内容来跳转到新的文档或者**当前文档的某个部分**.
```html
<a href="ur1">链接文本</a>
```
* **超链接属性**
  &emsp;在标签`<a>`中使用了`href`属性来描述链接的地址.
  &emsp;默认情况下,链接将以,一下形式出现在浏览器中:
  * 一个未访问的链接显示为蓝色字体并带有下划线.
  * 访问过的链接显示为紫色并带有下划线.
  * 点击链接时,链接显示为红色并带有下划线.
> 后期我们会通过CSS的样式修改这些效果.
#### 文本
* **常用文本标签**
    |标签|描述|
    |:--:|:--:|
    |`<em>文本</em>`|定义着重文本|
    |`<b>文本</b>`|定义粗体文文本|
    |`<i>文本</i>`|定义斜体字|
    |`<strong>文本</strong>`|定义加重语气|
    |`<del>文本</del>`|定义删除字|
    |`<span>文本</span>`|元素没有特定的含义|
> 常用文本标签和段落不同,段落代表一段文字,而文本标签一般表示文本词汇.
> 
#### 列表
##### 有序列表
&emsp;有序列表是一列项目,列表项目使用数字进行标记,有序列表始于`<ol>`标签,每个列表项始于`<li>`标签.
```html
<ol>
    <li>帅哥</li>
    <li>衰哥</li>
</ol>
```
* type属性
  &emsp;`ol`的属性type拥有的选项
  * 1 表示列表项目用数字标号 (1,2,3...)
  * a 表示列表项目用小写字母标号 (a,b,c...)
  * A 表示列表项目用大写字母标号 (A,B,C...)
  * i 表示列表项目用小写罗马数字标号 (i,ii,iii...)
  * I 表示列表用大写罗马数字标号(I,III...)
* 有序列表嵌套
  &emsp;列表是可以嵌套的
  ```html
  <ol>
      <li>水果</li>
      <li>蔬菜
        <ol>
          <li>胡萝卜</li>
          <li>豆芽菜</li>
        </ol>
      </li>
  </ol>
  ```
##### 无序列表
&emsp;无序列表是一个项目的列表,此项目使用粗体圆点(典型的小黑圆圈)进行标记.
无序列表始于`<ul>`标签,每个列表项始于`<li>`标签.
```html
<ul>
    <li>帅哥</li>
    <li>衰哥</li>
</ul>
```
* type属性
   `ul`的属性type拥有的选项
   * `disc` 默认实心圆
   * `circle` 空心圆
   * `square` 小方块
   * `none` 不显示
* 无序列表嵌套
  &emsp;列表可以进行嵌套
  ```html
    <ul>
      <li>水果</li>
      <li>蔬菜
        <ul>
          <li>胡萝卜</li>
          <li>豆芽菜</li>
        </ul>
      </li>
    </ul>
  ```
* **常见效果**
  * 无序列表效果
  * **导航效果**(里面放超文本链接) 
#### 表格
> 表格组成与特点
> 行,列,单元格
> 单元格特点: 同行等高,同列等宽
> 
> ----
> 表格的标签
> 表格: `table`
> 行: `tr`
> 单元格(列): `td`
```html
<table>
  <tr>
    <td>1</td>
    <td>2</td>
    <td>3</td>
    <td>4</td>
  </tr>
  <tr>
    <td>5</td>
    <td>6</td>
    <td>7</td>
    <td>8</td>
  </tr>
</table>
```
* **表格的属性**
  * `border`: 设置表格的宽度(代表单元格的像素单位,边框的粗壮程度.)
  * `width`: 设置表格的宽度
  * `height`: 设置表格的高度
* **表格单元格合并** 
  * 水平合并: `colspan`
  * 垂直合并: `rowspan`
```html
    <p>合并单元格1和2: colspan</p>
    <p>合并单元格4和8: rowspan</p>
    <p>水平合并: 保留左边,删除右边</p>
    <p>垂直合并: 保留上边,删除下边</p>
    <!--我认为这个合并实际就是把它的空间放大了-->
    <table border="1" width="200" height="100">
        <tr>
            <td colspan="2">1</td>

            <td>3</td>
            <td rowspan="2">4</td>
        </tr>
        <tr>
            <td>5</td>
            <td>6</td>
            <td>7</td>

        </tr>
    </table>
```
#### 表单
&emsp;表单在Web网页中用来给用户填写信息,从而采集用户信息,是网页具有交互的功能.所有的用户输入内容的地方都用表单来写,比如登录注册,搜索框.
* 表格是由容器和控件组成的,一个表一般应该包含用户填写信息的输入框,提交按钮等,这些输入框,按钮叫做控件,表单就是容器,它能容纳各种各样的控件.
```html
<form action="url" method="get|post" name="myform"></form>
```
> 属性说明
> 1. action服务器地址
> 2. name表单名称
> 3. method中get和post的区别
>    1. 数据提交方式,get提交的数据url可以看到,post看不到.
>    2. get一般用于少量数据,post用来提交大量的数据. 
* 表单元素
  &emsp;一个完整的表单包括3个组成部分:表单标签,表单域,表单按钮.
  * 表单标签
  * 表单域
  * 表单按钮
  ```html
  <form>
      <input type="text">
      <input type="submit">
  </form>
  ```
  * **文本框**:
    文本域通过`<input type="text">`标签来设定,当用户要在表单中键入字母,数字等内容时,就会用到文本域.
    ```html
    <form>
      First name: <input type="text" name="firstname">
      <br>
      last name: <input type="text" name="lastname">
    </form>
    ```
  * **密码**:
    密码字段通过标签`<input type="password">`来定义
    ```html
    <form>
        Password: <input type="password" name="pwd">
    </form>
    ```
    密码字段字符不会以明文显示,而是以星号或者圆点代替.
  * **提交按钮**:
     当用户点击确认按钮时,表单内容会被传送到另一个文件,表单的动作属性定义了目的文化的文件名.由动作属性定义的这个文件通常会接收到输入数据进行相关的处理.
     ```html
     <form name="input" action="url" method="get">
      username: <input type="text" name="user">
      <input type="submit" value="submit">
     </form>
     ```

#### 块行
内联元素和块级元素的区别
|块级元素|内联元素|
|:---:|:---:|
|块元素会在页面独占一行(自上向下垂直排列)|行内元素不会独占页面中的一行,只占自身的大小|
|可以设置width,height属性|行内元素的width,height属性无效|
|一般块级元素可以包含行内元素和其他块级元素|一般内联元素包含内联元素不包含块级元素|
* 常见块级元素
  > div,form,h1~h6,hr,p,table,ul,等
* 常见内联元素
  > a,b,em,i,span,strong等
* 行内块级元素(特点:不换行,能够识别宽高)
  > button,img,input等



`div`容器元素,也是页面中见到最多的元素.
为了区分内容模块,用`<div></div>`来分隔每个区分.
```html
<div id="" class ="">  </div>
```
我们可以通过id,class和其他的属性来说明这个容器的性质和作用.
