# Day 01 - 前端 Web 基础 (HTML & CSS)

## 一、 Web 前端基础与工作原理
* **Web 标准组成**：
  * [cite_start]**HTML**：负责网页的结构（页面元素和内容）[cite: 19, 48, 52]。
  * [cite_start]**CSS**：负责网页的表现（页面元素的外观、位置等页面样式，如：颜色、大小等）[cite: 20, 49, 52]。
  * [cite_start]**JavaScript**：负责网页的行为（交互效果）[cite: 21, 50]。
* [cite_start]**网页的本质**：网页本质上是程序员写的前端代码 [cite: 11][cite_start]。这些代码通过浏览器转换成用户看到的网页 [cite: 12]。
* [cite_start]**浏览器内核**：浏览器对代码进行解析渲染的部分称为浏览器内核 [cite: 13][cite_start]。不同浏览器内核不同，对于相同的前端代码解析的效果可能会存在差异 [cite: 14]。

---

## 二、 HTML 核心概念与基础
* [cite_start]**HTML 概念**：HTML（HyperText Markup Language）即超文本标记语言 [cite: 54][cite_start]。它由预定义好的标签构成，如 `<h1>` 展示标题，`<img>` 展示图片等 [cite: 56, 57][cite_start]。HTML 代码直接在浏览器中运行，由浏览器解析 [cite: 58]。
* **HTML 标签特点**：
  * [cite_start]html 标签不区分大小写，但建议小写 [cite: 93]。
  * [cite_start]属性值使用单引号或双引号都可以 [cite: 94]。
  * [cite_start]语法结构松散，建议规范书写 [cite: 95]。
* [cite_start]**页面基本骨架**：包含 `<html>` 根标签、`<head>`（网页头部，存放给浏览器看的信息，如 CSS 样式）、`<title>`（网页标题）以及 `<body>`（网页主体，存放给用户看的信息，如文字、图片等）[cite: 80, 81, 83, 86, 89, 90]。

---

## 三、 常见 HTML 标签及其用途

### 1. 排版与文本标签
* [cite_start]**标题标签**：`<h1>` - `<h6>`，用于定义页面标题 [cite: 126]。
* [cite_start]**段落标签**：`<p>`，用于定义文本段落 [cite: 258, 259]。
* **文本格式化标签**：
  * [cite_start]**加粗**：`<b>` / `<strong>`（其中 `<strong>` 具有强调语义）[cite: 267, 268, 269]。
  * [cite_start]**下划线**：`<u>` / `<ins>`（其中 `<ins>` 具有强调语义）[cite: 270, 271, 272]。
  * [cite_start]**倾斜**：`<i>` / `<em>`（其中 `<em>` 具有强调语义）[cite: 273, 274, 275]。
  * [cite_start]**删除线**：`<s>` / `<del>`（其中 `<del>` 具有强调语义）[cite: 276, 277, 278]。

### 2. 媒体与超链接标签
* [cite_start]**图片标签 (`<img>`)**：属性包括 `src`（指定图片路径）、`width` 和 `height` [cite: 255, 256, 257]。
* [cite_start]**视频标签 (`<video>`)**：属性包括 `src`（指定视频的 URL）、`controls`（是否显示播放控件）、`width` 和 `height` [cite: 249, 250, 251, 252, 253, 254]。
* [cite_start]**超链接标签 (`<a>`)**：`href` 指定资源访问的 url；`target` 指定在何处打开资源链接（`_self` 为默认值，在当前页面打开；`_blank` 在空白页面打开）[cite: 127, 128, 129, 130, 131]。

### 3. 表单标签 (`<form>`)
* [cite_start]**作用**：在网页中主要负责数据采集功能，如注册、登录等 [cite: 413, 418]。
* **核心属性**：
  * [cite_start]`action`：规定当提交表单时向何处发送表单数据（URL）[cite: 426]。
  * [cite_start]`method`：规定用于发送表单数据的方式（GET、POST）[cite: 427][cite_start]。GET 方式表单数据拼接在 url 后面，大小有限制；POST 方式表单数据在请求体中携带，大小没有限制 [cite: 428, 429]。
* **常用表单项**：
  * [cite_start]`<input>`：定义表单项，通过 `type` 属性控制输入形式 [cite: 421]。
  * [cite_start]`<button>`：定义按钮（如 submit、reset、button）[cite: 422]。
  * [cite_start]`<select>`：定义下拉列表 [cite: 423]。
  * [cite_start]`<textarea>`：定义文本域 [cite: 424]。

### 4. 表格标签 (`<table>`)
* [cite_start]`<table>`：定义表格整体 [cite: 446, 447]。
* [cite_start]`<thead>`：用于定义表格头部（可选）[cite: 448, 449]。
* [cite_start]`<tbody>`：定义表格中的主体部分（可选）[cite: 450, 451]。
* [cite_start]`<tr>`：表格的行，可以包裹多个 `<td>` [cite: 452, 453]。
* [cite_start]`<td>`：表格普通单元格，如果是表头单元格可替换为 `<th>` [cite: 454, 455]。

### 5. 无语义布局标签
* [cite_start]**`<div>`**：一行只显示一个（独占一行）；宽度默认是父元素的宽度，高度默认由内容撑开；可以设置宽高（width、height）[cite: 303, 304, 305, 306]。
* [cite_start]**`<span>`**：一行可以显示多个；宽度和高度默认由内容撑开；不可以设置宽高 [cite: 307, 308, 309, 310]。

---

## 四、 CSS 样式控制与排版

### 1. CSS 引入方式
* [cite_start]**行内样式**：写在标签的 `style` 属性中（配合 JavaScript 使用）[cite: 146]。
* [cite_start]**内部样式**：写在 `<style>` 标签中（通常约定写在 `<head>` 标签中）[cite: 147]。
* [cite_start]**外部样式**：写在一个单独的 `.css` 文件中，通过 `<link>` 标签在网页中引入 [cite: 148, 155]。

### 2. CSS 选择器
[cite_start]选择器用来选取需要设置样式的元素 [cite: 191][cite_start]。优先级顺序为：**id选择器 -> 类选择器 -> 元素选择器** [cite: 232]。
* [cite_start]**元素选择器**：`元素名称 {...}`，如 `h1 {...}` [cite: 196, 197, 198]。
* [cite_start]**类选择器**：`.class属性值 {...}`，如 `.cls {...}` [cite: 200, 201, 202]。
* [cite_start]**ID 选择器**：`#id属性值 {...}`，如 `#hid {...}` [cite: 204, 205, 206]。
* [cite_start]**分组选择器**：`选择器1,选择器2 {...}`，如 `h1,h2 {...}` [cite: 208, 209, 210]。
* [cite_start]**属性选择器**：`元素名称[属性名="值"] {...}`，如 `input[type="text"] {...}` [cite: 216, 217, 218]。
* [cite_start]**后代选择器**：`元素1 元素2 {...}`，如 `form input {...}` [cite: 219, 220, 221]。

### 3. 颜色表示形式
* [cite_start]**关键字**：如 red、green、blue [cite: 163, 164, 165]。
* [cite_start]**rgb 表示法**：`rgb(r,g,b)`，红绿蓝三原色，取值 0-255 [cite: 167, 168, 169]。
* [cite_start]**rgba 表示法**：`rgba(r,g,b,a)`，a 表示透明度，取值 0-1 [cite: 171, 172, 173]。
* [cite_start]**十六进制表示法**：`#rrggbb`，将数字转换成十六进制表示 [cite: 175, 176, 177]。

### 4. 盒子模型 (Box Model)
[cite_start]页面中所有的元素都可以看做是一个盒子，由盒子将页面中的元素包含在一个矩形区域内 [cite: 294]。
* [cite_start]**组成部分**：内容区域（content）、内边距区域（padding）、边框区域（border）、外边距区域（margin）[cite: 295]。
* [cite_start]设置边距属性时，可以按上、右、下、左的顺序设置，也可以通过 `padding-top`、`margin-left` 等单独指定某一个方位 [cite: 339, 340, 341, 342, 343, 344, 348]。

### 5. Flex 弹性布局
[cite_start]Flex 是一种一维的布局模型，可以为元素之间提供强大的空间分布和对齐能力 [cite: 373]。
* [cite_start]**开启方式**：`display: flex;` [cite: 382, 383]。
* **主轴方向 (`flex-direction`)**：
  * [cite_start]`row`：主轴方向为 x 轴，水平向右（默认）[cite: 386, 387]。
  * [cite_start]`column`：主轴方向为 y 轴，垂直向下 [cite: 388, 389]。
* **主轴对齐方式 (`justify-content`)**：
  * [cite_start]`flex-start`：从头开始排列 [cite: 391, 392]。
  * [cite_start]`flex-end`：从尾部开始排列 [cite: 393, 394]。
  * [cite_start]`center`：在主轴居中对齐 [cite: 395, 396]。
  * [cite_start]`space-around`：平分剩余空间 [cite: 397, 398]。
  * [cite_start]`space-between`：先两边贴边，再平分剩余空间 [cite: 399, 400]。
