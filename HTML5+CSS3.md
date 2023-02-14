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

### 1.4 introduction to html

HTML是什么？What we can do with it?

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











