# HTML5+CSS3

## course structure

- welcome and first step
- HTML fundamentals
- CSS fundamentals
- building layouts
- web design framework
- components and layouts
- omnifood:desktop
- omnifood:responsive
- omnifood:optimizations

## 1. section: welcome and first step

### 1.0 lecture: a high-level overview of web development

高度概括网页开发

<font size="5">front-end vs back-end development:</font>

<font size="6">在访问一个静态网站的时候会发生什么？</font>

<font size="4">   <font color='blue'>首先</font></font>，browser 会向 <font size="6"> the serve</font> where this page is hosted on the Internet 发送request

![image-20230208161504905](https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/image-20230208161504905.png)

<font color='gray'>每个网站都会被存储在称为<font size="6">服务器</font>的东西上</font>

<font color='gray'>serve is basically a computer that is connected to the Internet and can receive requests like this one.</font>

<font color='blue'><font size="4">其次</font></font>， the serve会获取构成网站的所有文件，然后把它们发送回浏览器browser（服务器向浏览器发送响应）

<font color='blue'><font size="4">最后</font></font>，那些文件名后缀有html，css，js，所以我们有一些html，css，js代码，这是任何浏览器都能理解的三大核心技术，一旦browser从service response收到这些文件后，会获取这些代码然后显示在浏览器上

![](https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE_20230208_144140.png)

the process of writing HTML,CSS and javascript code that the browser can understand is the process that we call front-end web development.     <font color='blue'>写HTML，css，js这些浏览器懂的代码的过程被称作前端网页开发</font>

上面这个是<font color='blue'>static website</font>的大致过程

![](https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE_20230208_145846.png)





<font size="6">在访问一个动态网站的时候会发生什么？</font>

首先浏览器会向服务器发送请求

dynamic website是不断变化的，比如b站不断增加的投稿视频，不断增加的评论弹幕等等

为了实现这些，网站需要一个应用程序APP在服务器上运行，并且还需要一个大的包含了所有显示在网站的内容的数据库DB

写这些在服务器运行的应用程序就要使用后端语言，python ，Java， Node js， PHP之类的，这些语言所做的就是从数据库中取出数据，然后将这些数据组装到最终文件中，然后把这些文件作为响应发送给浏览器

最后browser从service response收到这些文件后，会获取这些代码然后显示在浏览器上。

这整个过程被称作后端开发。

![](https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE_20230208_150452.png)





<font size="5">the 3 languages of the front-end</font>

![](https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE_20230208_152407.png)



### 1.1 setting up our code editor

实战

prettier拓展是自动的格式化，或者自动编码

### 1.2 your first webpage!

**index.html**是任何网站第一页的默认名称，所以index是任何网站的入口点 ，所有的网络项目总是需要一个index.html

输入“!” 单

[my first webpage](file:///C:/Users/23248/Desktop/01%20test/index.html)

![image-20230210142111300](https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/image-20230210142111300.png)

### 1.3 downloading course material

[我的HTML + CSS课程的入门文件，最终项目和常见问题解答 (github.com)](https://github.com/jonasschmedtmann/html-css-course)

## 2. section: HTML fundamentals

### 2.0 introduction to html

HTML是什么？What we can do with it?

[HTML 教程 (w3school.com.cn)](https://www.w3school.com.cn/html/index.asp)

**在上面的这个链接中有更多关于  标签(tag)、元素、属性的介绍，更加全面**

- HyperText Markup Language

- HTML is a markup language that web developers use to structure and describe the content of a webpage (not a programming language)

- HTML consists of elements that describe different types of content: paragraphs, links, headings, images, video, etc.

- Web browsers understand HTML and [render](https://blog.csdn.net/wishfly/article/details/82993278) HTML code as websites 

  - 翻译：

    - 超文本标记语言

    - HTML是一种标记语言，web开发人员使用它来构造和描述网页的内容(不是一种程序设计语言)。

    - HTML由描述不同类型内容的元素组成:段落、链接、标题、图像、视频等。

    - 浏览器理解HTML并且将HTML代码渲染成网站 呈现为网站

HTML元素的剖析the anatomy of HTML element：

- ![image-20230214162245306](https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/image-20230214162245306.png)

- 翻译版

  ![ ](https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/image-20230214162416740.png)

用p打开，用/p关闭；当元素没有内容时，比如<img>就只有opening tag。

学到这里，我：这跟markdown好像

### 2.1 HTML Document structure

在课程材料中打开start，复制02这个文件夹到另外的地方，这样会使学习过程更有序

打开vs code，然后在vs code里打开复制的那个文件夹，然后打开.txt文件放到一边，然后再在打开的文件夹中创建一个.html文件

这回，虽然有打出感叹号vs code自己帮我们写结构的方法，但是我们要自己写HTML的结构。

- 首先要做的是声明一个所谓的 doc类型  像这样： `<!DOCTYPE html>`

  告诉浏览器这个文档使用HTML。所有的浏览器都会因此知道用HTML5的规范来render 这个HTML

- 接下来，我们需要创建一个HTML元素  像这样：`<html></html>`

  - 在创建元素时，vs code会自动帮我们写出closing tag，在设置里搜`auto closing tags`然后把HTML的取消勾选就可以自己写了

- 然后在html元素里，我们要插入其它元素；首先需要一个head元素，再是body元素  像这样：

```html
<!DOCTYPE html>
<html>
    <head></head>
    <body></body>
</html>
```

head元素是为了在浏览器窗口不可见的东西，所以head会包括页面标题、有关页面的一些附加信息、链接到css文件或者其它东西。

body其实是为了在页面上可见的所有元素。all of the element that we see here in the browser will always be inside of the body element.

```html
<!DOCTYPE html> 
<html>
    <head>
        <title>THe Basic Language of the Web:HTML</title>//页面标题
    </head>
    <body>
        <h1>THe Basic Language of the Web:HTML</h1>
    </body>
</html>
```

**summary: 首先要有!DOCTYPE html；再有html元素；在html元素中，分别有head和body；head管页面看不到的，body管页面看得到的。**

### 2.2 text element

[HTML 标题 (w3school.com.cn)](https://www.w3school.com.cn/html/html_headings.asp)

涵盖`<head> <h1>to<h6> <!--...-->`

[HTML 段落 (w3school.com.cn)](https://www.w3school.com.cn/html/html_paragraphs.asp)

涵盖`<p> <br>` 还有HTML 输出格式的提示

[HTML 文本格式化 (w3school.com.cn)](https://www.w3school.com.cn/html/html_formatting.asp)

涵盖各种格式

[HTML 注释 (w3school.com.cn)](https://www.w3school.com.cn/html/html_comments.asp)

涵盖`<!-- 在此处写注释 -->`  还有条件注释

- 标题`<h1></h1>`  有6级

![image-20230215144114005](https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/image-20230215144114005.png)

- 段落`<p></p>`   一对一个段落

![image-20230215144747675](https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/image-20230215144747675.png)

- 注释`<!-- -->`

<img src="https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/image-20230215150826576.png" alt="image-20230215150826576" style="zoom: 33%;" />

- 粗体`<b></b>`

![image-20230215151143167](https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/image-20230215151143167.png)

**但是想加粗请使用`<strong></strong>`**   b比较老 ， strong也更容易使代码看懂

- 斜体`<i></i>`

  ![image-20230215151754140](https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/image-20230215151754140.png)

**但是想斜体请使用`<em></em>  `   ** i比较老  em是emphasis

### 2.3 more text element: list

列表分有序（数字）和无序（点）

- 有序列表  ordered list `<ol></ol>`
  - 在有序列表元素中还要含有列表项 list item 元素 `<li></li>` 
  - ![image-20230215155644982](https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/image-20230215155644982.png)

- 无序列表 unordered list `<ul></ul>`
  - 在无序列表元素中我们仍然用`<li></li>`for the individual items
  - ![image-20230215160550704](https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/image-20230215160550704.png)





### **现在我们有了这个页面的基本脉络**

![image-20230215161801245](https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/image-20230215161801245.png)

记住，没有结构就没有意义，就像这样只是一大段文字

![image-20230215162057252](https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/image-20230215162057252.png)



### 2.4 images and attributes

- 图片 `<img  />`
- [HTML 图像 (w3school.com.cn)](https://www.w3school.com.cn/html/html_images.asp)
  - html如何知道它该显示哪个元素？ **通过属性attribute**  attribute是可以用来描述元素的数据片段  attributes are pieces of data which we can use to describe element.  意思就是属性为HTML提供附加信息。  HTML里有许多不同的属性attributes
  - [HTML 属性 (w3school.com.cn)](https://www.w3school.com.cn/html/html_attributes.asp)

  - 其中之一就是 source 属性 `src="" ` 用来告诉html是哪张图片   
    - ![image-20230215164203932](https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/image-20230215164203932.png)

  - 还有alternative text属性 `alt=""` 用来告诉html，当图片因为某些原因无法显示时就打印引号里的东西；永远不要跳过这个属性
    - ![image-20230215185327923](C:\Users\23248\AppData\Roaming\Typora\typora-user-images\image-20230215185327923.png)
  - 还有width宽度，height高度属性 `width=""` `height=""`    只写其中一个的话会自动保持横纵比例
    - ![image-20230215185739265](https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/image-20230215185739265.png)

还有一些HTML的属性，比如lang（中文是zh），charset 

![image-20230215232633595](https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/image-20230215232633595.png)

[HTML  <meta>标签 (w3school.com.cn)](https://www.w3school.com.cn/tags/tag_meta.asp)

![image-20230215233709835](https://abigail-1315839746.cos.ap-nanjing.myqcloud.com/typora/image-20230215233709835.png)

