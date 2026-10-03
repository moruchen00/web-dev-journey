项目	说明
标签名	比如 <img>
作用	一句话，用自己的话说
关键属性	只记最常用的 1-2 个
最小例子	一行能跑起来的代码
注意点	容易忘的、特殊的，没有就不写

## <img> 图片

**作用**：在页面里插入一张图片。

**关键属性**：
- `src`：图片地址（本地路径或网址）
- `alt`：图片加载失败时显示的文字，屏幕阅读器也会读

**例子**：
<img src="cat.jpg" alt="一只橘猫">

**注意**：`<img>` 是自闭合标签，不需要 `</img>`。

## <!----> 注释

**作用**：注释允许你留下消息而不影响浏览器显示。它还允许你使代码失效。HTML中的注释以<!--开始，包含任何行的文本，并以-->结束。

**关键属性**：
<!--和-->中间是包含任何行的文本

**例子**：
<!-- TODO: Add link to cat photos -->

**注意**：`<!---->` 是自闭合标签,文本输入在左右两个箭头中间。

## <main> 主要内容

**作用**：main元素用于表示 HTML 文档主体的主要内容。main元素里的内容应该是文档中唯一的，不应该在文档的其他部分重复。

**关键属性**：
<main>元素里的内容应该是文档中唯一的，不应该在文档的其他部分重复。

**例子**：
<main>
    <h1>CatPhotoApp</h1>
    <h2>Cat Photos</h2>
    <!-- TODO: Add link to cat photos -->
    <p>Everyone loves cute cats online!</p>
</main>

**注意**：`<mian>` 不是自闭合标签，需要 `</main>`。
          为了易于阅读，main元素中的元素最好要比main元素多两个空格。


## <a> 链接

**作用**：你可以使用一个元素<a>链接到另一个页面。

**关键属性**：
- `href`：链接地址
- `target` 打开链接文档的位置。target="_blank"可以在新建标签页或窗口中打开链接文档
**例子**：
<a href="https://freecatphotoapp.com"></a>
<a href="https://freecatphotoapp.com">cat photos</a>
cat photos 是链接的文本
<p>See more <a href="https://freecatphotoapp.com" target="_blank">cat photos</a> in our gallery.</p>
图片也可以作为链接的文本。
例子：
 <a href=https://freecatphotoapp.com><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back."></a>
**注意**：`<a>` 不是自闭合标签，需要 `</a>`。
        链接的文本必须放在元素（a）的开始和结束标签之间。


## <section> 段落

**作用**：在添加任何新内容之前，您应该使用section元素将猫咪照片内容与未来的内容分开。

section用于在文档中定义各个部分的元素，例如章节、页眉、页脚或文档的任何其他部分。它是一个对 SEO 且不易有帮助的语义化元素。

**关键属性**：


**例子**：
<section>
        <h2>Cat Photos</h2>
        <p>Everyone loves <a href="https://cdn.freecodecamp.org/curriculum/cat-photo-app/running-cats.jpg">cute cats</a> online!</p>
        <p>See more <a target="_blank" href="https://freecatphotoapp.com">cat photos</a> in our gallery.</p>
        <a href="https://freecatphotoapp.com"><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back."></a>
      </section>

**注意**：`<section>` 不是自闭合标签，需要 `</section>`。


## <ul> 无序项目列表

**作用**：要创建一个无序项目列表，你可以使用ul元素

**关键属性**：


**例子**：
      <ul>Things cats love:</ul>

**注意**：`<ul>` 不是自闭合标签，需要 `</ul>`。


## <li> 无序列表项

**作用**：用于在村庄或无序列表中创建列无序表项

**关键属性**：


**例子**：
 <ul>
          <li>catnip</li>
          <li>laser pointers</li>
          <li>lasagna</li>
        </ul>
**注意**：`<li>` 不是自闭合标签，需要 `</li>`。


## <figure> 自包含的内容

**作用**：figure元素代表自包含的内容，允许您将图像与标题相关联。

**关键属性**：

**例子**：
 <figure>
        <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="A slice of lasagna on a plate.">
        </figure>

**注意**：`<figure>` 不是自闭合标签，需要 `</figure>`。


## <figcaption> 图题

**作用**：元素用于添加标题给<figure>元素中包含的图像。

**关键属性**：

**例子**：
<figure>
          <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="A slice of lasagna on a plate.">
          <figcaption>Cats love lasagna.</figcaption>
        </figure>

**注意**：`<figcaption>` 不是自闭合标签，需要 `</figcaption>`。


## <em> 斜体

**作用**：强调一个特定的单词或句子。

**关键属性**：

**例子**：
<figcaption>Cats <em>love</em> lasagna.</figcaption>

**注意**：`<iem>` 不是自闭合标签，需要 `</em>`。


## <ol> 有序项目列表

**作用**：类似于无序列表<li>，但是<ol>小区列表中的列表项在显示时是编号的。

**关键属性**：

**例子**：
<ol>
          <li>flea treatment</li>
          <li>thunder</li>
          <li>other cats</li>
        </ol>

**注意**：`<ol>` 不是自闭合标签，需要 `</ol>`。


## <strong> 加粗

**作用**：在页面里插入一张图片。

**关键属性**：

**例子**：
Cats <strong>hate</strong> other cats.

**注意**：`<strong>` 不是自闭合标签，需要 `</strong>`。


## <footer> 页脚

**作用**：用于定义文档或章节的页脚的元素。页脚通常包含文档作者信息、版权数据、使用条款链接、联系信息等。。

**关键属性**：

**例子**：
 <footer>
      <p>
        No Copyright - <a href="https://www.freecodecamp.org">freeCodeCamp.org</a>
      </p>
    </footer>

**注意**：`<footer>` 不是自闭合标签，需要 `</footer>`。


## <body> 本体

**作用**：所有应该添加到页面中的内容元素都位于body元素中。

**关键属性**：

**例子**：

**注意**：`<body>` 不是自闭合标签，需要 `</body>`。

## <head> 页面信息

**作用**：用于包含关于文档的元数据的元素，例如它的标题、样式表链接和脚本。元数据不直接显示在页面上的关于页面的信息。

**关键属性**：

**例子**：

**注意**：`<head>` 不是自闭合标签，需要 `</head>`。


## <title> 标题

**作用**：title元素决定浏览器在页面的标题栏或选项卡中显示的内容。

**关键属性**：

**例子**：
<title>CatPhotoApp</title>

**注意**：`<title>` 不是自闭合标签，需要 `</title>`。

## <html> 根元素

**作用**：注意，页面的所有内容都描绘在html元素中。html元素是 HTML 页面的根元素，包含页面上的所有内容。

**关键属性**：
- `lang`：语言，英文为 en

**例子**：
<html lang="en">

**注意**：`<html>` 不是自闭合标签，需要 `</html>`。

## <!DOCTYPE html> 开头

**作用**：所有页面均应以<!DOCTYPE html>开头。这个特殊的字串称为声明，确保浏览器尝试符合行业范围内的规格说明。
<!DOCTYPE html>告诉浏览器该文档是一个 HTML5 文档，是最新版本的 HTML。
**关键属性**：

**例子**：


**注意**：<!DOCTYPE html>在第一行


## <meta> 用于设置浏览器行为

**作用**：设置浏览器行为

**关键属性**：
- `attribute`：
- `charset`：字符集编码

**例子**：
 <meta charset="UTF-8">

**注意**：注意<meta>元素是一个空元素。。


## <style> 元素

**作用**：在 HTML 内部写 CSS，控制页面样式。

**位置**：通常放在 <head> 里。

**例子**：
<style>
  body {
    background-color: burlywood;
  }
</style>

**注意**：里面的内容不会显示，浏览器会当作 CSS 执行。


## 元素（element）

**定义**：开始标签 + 内容 + 结束标签，合起来叫一个元素。

**例子**：
<p>你好</p> 这是一个 p 元素。

**注意**：
- 元素可以嵌套，比如 <p> 里放 <strong>。
- 标签只是尖括号部分，元素是完整结构。

## <link> 元素

**作用**：链接外部资源，最常用是引入外部 CSS 文件。

**位置**：放在 <head> 里。

**关键属性**：
- rel="stylesheet"：说明这是样式表
- href="styles.css"：CSS 文件的路径

**例子**：
<link rel="stylesheet" href="styles.css">

**注意**：自闭合标签，不显示在页面上。

## <meta name="viewport">

**作用**：让网页在手机上按屏幕实际宽度显示，不缩小成桌面版。

**位置**：放在 <head> 里。

**例子**：
<meta name="viewport" content="width=device-width, initial-scale=1.0">

**注意**：
- width=device-width：宽度等于设备宽度
- initial-scale=1.0：初始缩放比例为 1
- 几乎所有响应式网页都会写这一行


## <div> 元素

**作用**：通用容器，把内容包起来，方便加样式或布局。

**例子**：
<div class="menu-item">
  <h3>拿铁</h3>
  <p>$4.00</p>
</div>

**注意**：
- 没有语义，只是盒子
- 常配合 class 使用
- 有语义的区块优先用 <section>、<main>、<article>

## id 属性

**作用**：给元素起一个唯一的名字，方便 CSS 或 JavaScript 定位。

**例子**：
<div id="menu">...</div>

**CSS 里选中它**：
#menu {
  width: 300px;
}

**注意**：
- 一个页面里 id 必须唯一
- 可以重复用的用 class

## class 属性

**作用**：给元素起一个或多个类名，方便 CSS 和 JavaScript 选中，并可以重复使用。

**例子**：
<div class="menu">...</div>
<p class="menu-item">拿铁</p>

**多个类名**：用空格分开
<div class="menu dark">...</div>

**注意**：
- class 可以重复，多个元素可以共用同一个类名
- 一个元素可以有多个 class
- 和 id 不同，id 在页面里必须唯一

## <article> 元素

**作用**：表示一段独立、完整、可单独存在的内容。

**例子**：
<article class="item">
  <p class="flavor">French Vanilla</p>
  <p class="price">3.00</p>
</article>

**注意**：
- 有语义，表示独立内容
- 常用于博客、帖子、菜单条目、产品卡片
- 和 <section> 的区别：article 更强调独立完整
- 和 <div> 的区别：div 没有语义

## <address> 元素

**作用**：表示联系信息，比如地址、邮箱、电话。

**位置**：通常放在 <footer> 里。

**例子**：
<footer>
  <address>
    <p>123 Free Code Camp Drive</p>
  </address>
</footer>

**注意**：
- 默认是斜体，可以用 font-style: normal; 去掉
- 里面可以放 <p>、<a>
- 语义化元素，表示联系信息

## <hr> 元素

**作用**：画一条水平分割线，表示内容主题的分隔。

**例子**：
<h2>Coffee</h2>
<hr>
<p>美式咖啡 $3.00</p>

**注意**：
- 自闭合标签，不需要 </hr>
- 默认有灰色线、上下间距
- 可以用 CSS 改颜色、粗细：
  hr {
    height: 2px;
    background-color: brown;
    border: none;
  }