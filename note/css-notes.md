## text-align

**作用**：控制元素内文字的水平对齐方式。

**常用值**：
- left：左对齐（默认）
- center：居中
- right：右对齐
- justify：两端对齐

**例子**：
h1 {
  text-align: center;
}

h1, h2, p {
        text-align: center;
      }

**注意**：它不是 HTML 元素，是 CSS 属性。

## background-color

**作用**：设置元素的背景颜色。

**例子**：
body {
  background-color: brown;
}

**注意**：
- 选择器 body 表示选中整个页面主体
- 颜色可以用英文名（brown）、十六进制（#a52a2a）或 rgb

## ID 选择器 #menu

**作用**：选中 id="menu" 的元素。

**例子**：
#menu {
  width: 300px;
}

**注意**：
- # 开头表示 ID 选择器
- 一个页面里 id 必须唯一
- width: 300px 表示宽度 300 像素

## 水平居中

**方法**：给有宽度的块级元素设置左右 margin 为 auto。

**例子**：
#menu {
  width: 80%;
  margin-left: auto;
  margin-right: auto;
}

**注意**：
- 元素必须有宽度（固定 px 或百分比）
- 只对块级元素有效，比如 div、p、h1

## 类选择器 .

**作用**：选中所有带有指定 class 的元素。

**写法**：点号 + 类名

**例子**：
.menu {
  width: 80%;
}

**对应 HTML**：
<div class="menu">...</div>

**注意**：
- `.` 开头表示类选择器
- `#` 开头表示 ID 选择器
- 类选择器可以同时选中多个元素
- 可以组合使用，比如 `p.menu-item` 只选中带该类的 `<p>`

## display

**作用**：决定元素在页面上如何排列。

**常用值**：
- block：独占一行，可设宽高（div、p、h1 默认）
- inline：不独占一行，宽高由内容决定（span、a 默认）
- inline-block：并排显示，但可设宽高
- none：隐藏元素
- flex：弹性布局，子元素灵活排列
- grid：网格布局

**例子**：
.item p {
  display: inline-block;
}

**注意**：
- block 元素可以设 width/height/margin/padding
- inline 元素设 width/height 通常无效
- inline-block 常用于菜单项、按钮

## 后代选择器 .item p

**作用**：选中 class="item" 元素里面的所有 <p> 元素。

**例子**：
.item p {
  display: inline-block;
}

**对应 HTML**：
<article class="item">
  <p class="flavor">French Vanilla</p>
  <p class="price">3.00</p>
</article>

**注意**：
- 空格表示“里面的”“后代”
- `.item` 只选中父元素本身
- `.item p` 选中父元素里面的 p
- 类似写法：`.item .flavor`、`.item > p`

## 左右对齐的菜单行

**思路**：
1. 用 .item p 让两个 p 并排（display: inline-block）
2. .flavor 靠左，宽度 49%
3. .price 靠右，宽度 49%

**例子**：
.item p {
  display: inline-block;
}

.flavor {
  text-align: left;
  width: 49%;
}

.price {
  text-align: right;
  width: 49%;
}

**注意**：
- 两个 49% 加起来 98%，留一点间隙
- 文字对齐用 text-align，元素并排用 display

## padding 内边距

**作用**：设置元素内容和边框之间的空间。

**常用写法**：
padding: 10px;
padding: 10px 20px;
padding: 10px 20px 30px 40px;

**单边写法**：
padding-top / padding-right / padding-bottom / padding-left

**和 margin 的区别**：
- padding：内边距，背景色延伸
- margin：外边距，背景色不延伸

**例子**：
.item p {
  padding: 5px;
}


## max-width 最大宽度

**作用**：限制元素的最大宽度，元素可以更小，但不会超过这个值。

**例子**：
.menu {
  width: 80%;
  max-width: 500px;
}

**和 width 的区别**：
- width：固定宽度，不随屏幕变化
- max-width：最大宽度，屏幕小时会自动缩小

**注意**：
- 常用于响应式设计，防止大屏幕上内容过宽
- 常和 width、margin: auto 一起用

## font-style

**作用**：设置字体的样式，最常用是斜体。

**常用值**：
- normal：正常
- italic：斜体
- oblique：倾斜

**例子**：
.established {
  font-style: italic;
}

**注意**：
- 和 font-weight（加粗）不同
- italic 常用于副标题、引用、强调

## font-size

**作用**：设置文字大小。

**例子**：
h1 {
  font-size: 40px;
}

h2 {
  font-size: 30px;
}

**注意**：
- 常见单位：px、rem、em、%
- 类型选择器直接用标签名，不加 . 或 #
- 浏览器有默认字号，写了会覆盖默认值

## 给 hr 加样式

**例子**：
hr {
  height: 2px;
  background-color: brown;
  border-color: brown;
}

**作用**：
- height：线的粗细
- background-color：线的颜色
- border-color：边框颜色
- 也可以用 border: none; 去掉边框

**注意**：
- hr 默认是灰色细线
- 同时设置背景色和边框色，整条线才是同一种颜色


## margin 简写

**两个值**：
margin: 5px 0;
- 第一个值：上下
- 第二个值：左右

**四个值**（顺时针）：
margin: 10px 20px 30px 40px;
- 上 10px、右 20px、下 30px、左 40px

**单边**：
margin-top / margin-right / margin-bottom / margin-left

**例子**：
.item p {
  display: inline-block;
  margin: 5px 0;
}

## CSS 注释

**写法**：
/* 注释内容 */

**例子**：
/* FOOTER */

**作用**：
- 给代码分段、做标记
- 浏览器不会执行注释内容
- 方便自己和别人阅读

## 伪类 :visited

**作用**：选中已访问过的链接，改变它的样式。

**例子**：
a:visited {
  color: gray;
}

**常见伪类**：
- :visited：已访问过的链接
- :hover：鼠标悬停
- :active：被点击时
- :focus：获得焦点时

**注意**：
- 冒号开头
- 写在选择器后面，比如 a:visited、a:hover
- 可以配合元素、类、ID 使用