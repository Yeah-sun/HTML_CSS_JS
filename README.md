# HTML_CSS_JS
前端三件套(用的webstorm)
* [ ] HTML5
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
#### 超文本链接
#### 文本
#### 列表
#### 表格
#### 块行

