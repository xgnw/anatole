+++
title = "HTML常见标签用法！"
date = "2022-06-02T11:52:03+08:00"
tags = [
    "网站制作",
]

+++

前言
当我们开始学习HTML时，我们会接触到各种不同的HTML标签，每个标签都有其独特的用途和功能。在这篇博客文章中将详细介绍每个标签的用法，以更好地理解HTML的基础知识。

HTML标签（一）：标题和段落
在HTML中，标题和段落是构建文档结构和组织内容的基础。以下是标题和段落标签的详细用法：

1. <h1> - <h6> 标题标签：

HTML提供了六个级别的标题标签，用于表示不同级别的标题。<h1> 表示最高级别的标题，而 <h6> 表示最低级别的标题。标题标签通常用于定义文档的结构和层次。

<h1>这是一个<h1>级别的标题</h1>
<h2>这是一个<h2>级别的标题</h2>
<h3>这是一个<h3>级别的标题</h3>
<!-- ... -->
<h6>这是一个<h6>级别的标题</h6>
2. <p> 段落标签：

<p> 标签用于定义文本段落，可以包含文本、图像、链接等内容。段落标签通常用于将相关内容组织成段落。

<p>这是一个段落。段落可以包含文本、图像和链接等。</p>
<p>另一个段落。</p>
3. <br> 换行标签：

<br> 标签用于强制换行，通常用于在段落中插入换行符。

<p>这是一行文本。<br>这是另一行文本，位于上一行下方。</p>
4. <hr> 分隔线标签：

<hr> 标签用于插入水平分隔线，用于分隔内容或创建视觉分隔。

<p>这是一些文本内容。</p>
<hr>
<p>这是另一部分文本内容。</p>
5. <pre> 预格式化文本标签：

<pre> 标签用于保留文本中的空格和换行符，通常用于显示代码或预格式化文本。

<pre>
  function sayHello() {
    console.log("Hello, World!");
  }
</pre>
HTML标签（二）：链接和图像
1. <a> 链接标签：

<a> 标签用于创建链接，将文本或图像与其他网页或资源相关联。它有一个href属性，用于指定链接的目标URL。

<a href="https://www.example.com">这是一个链接到示例网站的文本</a>
您还可以使用target属性来指定链接如何在浏览器中打开，例如在新窗口中打开：

<a href="https://www.example.com" target="_blank">在新窗口中打开示例网站</a>
2. <img> 图像标签：

<img> 标签用于在网页中插入图像。它有一个src属性，用于指定图像的文件路径。您可以设置alt属性来提供图像的替代文本，以便在图像无法加载时提供描述。

<img src="image.jpg" alt="美丽的风景图片">
HTML标签（三）：列表和表格
3. <ul> 无序列表标签：

<ul> 标签用于创建无序列表，其中列表项不带编号或序号。每个列表项由<li>标签定义。

<ul>
  <li>项目一</li>
  <li>项目二</li>
  <li>项目三</li>
</ul>
4. <ol> 有序列表标签：

<ol> 标签用于创建有序列表，其中每个列表项都带有编号或序号。同样，每个列表项由<li>标签定义。

<ol>
  <li>第一步</li>
  <li>第二步</li>
  <li>第三步</li>
</ol>
5. <table> 表格标签：

<table> 标签用于创建表格，包括行和列。表格中的内容通过<tr>（表格行）、<td>（表格数据单元格）和<th>（表头单元格）标签来定义。

<table>
  <tr>
    <th>姓名</th>
    <th>年龄</th>
  </tr>
  <tr>
    <td>张三</td>
    <td>25</td>
  </tr>
  <tr>
    <td>李四</td>
    <td>30</td>
  </tr>
</table>
6. <form> 表单标签：

<form> 标签用于创建Web表单，允许用户输入和提交数据。表单通常包含输入字段、复选框、单选按钮等。

<form action="submit.php" method="post">
  <!-- 表单元素在这里 -->
  <input type="text" name="username" placeholder="用户名">
  <input type="password" name="password" placeholder="密码">
  <button type="submit">提交</button>
</form>
HTML标签（四）：文本样式和媒体元素
1. <strong> 和 <em> 强调标签：

<strong> 和 <em> 标签用于强调文本内容。<strong> 表示强调文本更加重要或更显眼（通常以粗体显示），而 <em> 表示斜体文本以强调。

<p>这是一个<em>强调</em>文本。</p>
<p>这是一个<strong>重要的</strong>通知。</p>
2. <u> 下划线标签：

<u> 标签用于给文本添加下划线。请注意，虽然可以使用这个标签添加下划线，但通常更好的做法是使用CSS来控制文本的样式。

<p>这个文本有<u>下划线</u>。</p>
3. <s> 删除线标签：

<s> 标签用于在文本上添加删除线，通常表示文本已被删除或不再有效。与 <u> 一样，更好的做法是使用CSS来控制文本的样式。

<p>这个文本已被<s>删除</s>。</p>
4. <audio> 和 <video> 媒体标签：

<audio> 和 <video> 标签用于在网页中嵌入音频和视频。它们允许您播放媒体文件，提供了控制和自定义选项。

<audio controls>
  <source src="music.mp3" type="audio/mpeg">
  您的浏览器不支持音频标签。
</audio>
<video controls>
  <source src="video.mp4" type="video/mp4">
  您的浏览器不支持视频标签。
</video>
HTML标签（五）：其他常用标签
1. <div> 分区标签：

<div> 标签用于创建一个通用的容器，通常用于分组和样式化网页中的元素。它本身不会添加任何可见的效果，但允许您将元素组织成块或部分，以便使用CSS进行样式化。

<div class="container">
  <p>这是一个容器中的文本。</p>
  <img src="image.jpg" alt="图片">
</div>
2. <span> 行内标签：

<span> 标签类似于<div>，但它是一个行内元素，通常用于内联样式化文本的一部分。

<p>这个<span style="color: red;">文本</span>是红色的。</p>
HTML标签（六）：表单元素和元数据
1. <input> 输入标签：

<input> 标签用于创建各种类型的表单输入字段，如文本框、密码框、单选按钮、复选框等。它的 type 属性确定了输入字段的类型。

<input type="text" name="username" placeholder="用户名">
<input type="password" name="password" placeholder="密码">
<input type="radio" name="gender" value="male"> 男性
<input type="radio" name="gender" value="female"> 女性
<input type="checkbox" name="subscribe" value="yes"> 订阅
2. <select> 选择框标签：

<select> 标签用于创建下拉选择框，允许用户从一组选项中选择一个或多个。选项由 <option> 标签定义。

<select name="country">
  <option value="us">美国</option>
  <option value="ca">加拿大</option>
  <option value="uk">英国</option>
</select>
3. <textarea> 文本区域标签：

<textarea> 标签用于创建多行文本输入框，通常用于用户输入大段文本。

<textarea name="comments" rows="4" cols="50">在这里输入您的评论...</textarea>
4. <label> 标签：

<label> 标签用于为表单元素提供标签文本，提高表单的可读性和可访问性。通常，<label> 与相关的表单元素通过 for 属性进行关联。

<label for="username">用户名：</label>
<input type="text" name="username" id="username">
5. <meta> 元标签：

<meta> 元标签用于提供有关HTML文档的元数据信息，如字符集、作者、关键词等。它通常位于文档的 <head> 部分。

<meta charset="UTF-8">
<meta name="author" content="John Doe">
<meta name="keywords" content="HTML, CSS, JavaScript">
HTML标签（七）：其他有用的标签
1. <iframe> 内联框架标签：

<iframe> 标签用于嵌入另一个网页或文档。这使得您可以将其他网页嵌入到您的网页中，例如嵌入地图、视频或其他内容。

<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3..."></iframe>
2. <abbr> 缩写标签：

<abbr> 标签用于定义缩写或首字母缩略词，并通过 title 属性提供完整的解释。

<abbr title="HyperText Markup Language">HTML</abbr> 是网页标记语言。
3. <time> 时间标签：

<time> 标签用于表示日期和时间。它可以帮助搜索引擎和浏览器正确地解释日期和时间信息。

<p>文章发布于 <time datetime="2023-09-30">2023年9月30日</time></p>
HTML标签（八）：更多常见标签
1. <dl>、<dt> 和 <dd> 标签：

<dl> 标签用于创建描述列表，<dt> 标签定义术语标题，<dd> 标签定义术语的描述。

<dl>
  <dt>HTML</dt>
  <dd>超文本标记语言</dd>
  <dt>CSS</dt>
  <dd>层叠样式表</dd>
</dl>
2. 嵌套标签：

HTML允许您嵌套标签，这意味着您可以将一个标签放在另一个标签内部。例如，您可以将链接标签<a>嵌套在列表项<li>内。

<ul>
  <li><a href="#">链接一</a></li>
  <li><a href="#">链接二</a></li>
</ul>
3. 特殊字符和实体引用：

某些字符在HTML中具有特殊意义，因此如果要在文本中显示它们，必须使用实体引用或字符实体。例如，< 必须写成 &lt;。

<p><div> 是一个 HTML 标签。</p>
4. <blockquote> 引用标签：

<blockquote> 标签用于引用文本，通常用于引用他人的言论或引用。

<blockquote>
  <p>“学而不思则罔，思而不学则殆。”</p>
  <cite>——孔子</cite>
</blockquote>
HTML标签（九）：链接、媒体元素、样式和元数据
1. <link> 链接标签：

<link> 标签通常用于将外部资源引入到HTML文档中，最常用于链接样式表（CSS文件）。

<link rel="stylesheet" type="text/css" href="styles.css">
2. <style> 内联样式标签：

<style> 标签用于在HTML文档内部定义样式规则，它通常位于文档的 <head> 部分。这样的样式称为内联样式。

<style>
  p {
    color: blue;
  }
</style>
3. <script> 脚本标签：

<script> 标签用于在HTML文档中嵌入JavaScript代码，可以实现网页的交互和动态效果。

<script>
  function sayHello() {
    alert("Hello, World!");
  }
</script>
4. <noscript> 无脚本标签：

<noscript> 标签用于在用户禁用了JavaScript时提供替代内容，通常用于向用户提供必要的信息或指令。

<noscript>
  请启用JavaScript以查看此网站的全部功能。
</noscript>
HTML标签（十）：文本格式化、媒体元素控制和高级功能
1 <mark> 高亮标签：

<mark> 标签用于在文本中突出显示或高亮特定的部分，通常以黄色背景显示。

<p>这段文字中的 <mark>关键信息</mark> 需要特别注意。</p>
2. <ins> 和 <del> 标签：

<ins> 和 <del> 标签分别用于表示插入和删除的文本更改，通常以下划线或删除线显示。

<p>这是 <ins>新添加的文本</ins>。</p>
<p>这是 <del>已删除的文本</del>。</p>
3. <iframe> 内联框架标签：

<iframe> 标签用于嵌入另一个网页或文档，例如，您可以嵌入一个Google地图或其他网页。

<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3..."></iframe>
4. <canvas> 画布标签：

<canvas> 标签用于绘制图形，创建图表、动画和其他视觉效果的HTML5元素。

<canvas id="myCanvas" width="200" height="100"></canvas>
5. <svg> 可缩放矢量图形标签：

<svg> 标签用于在网页上创建矢量图形，支持缩放而不失真。它通常用于创建图标和图形。

<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" stroke="black" stroke-width="2" fill="red" />
</svg>
6. <details> 和 <summary> 标签：

<details> 和 <summary> 标签用于创建可折叠的内容区域，允许用户单击摘要来显示或隐藏详细信息。

<details>
  <summary>显示更多信息</summary>
  <p>这里是更多的详细内容。</p>
</details>
7 <template> 模板标签：

<template> 标签用于定义客户端模板，它的内容不会直接显示在页面上，但可以通过JavaScript进行克隆和显示。

<template id="myTemplate">
  <p>This is a template.</p>
</template>
HTML标签（十一）：表格、表单和高级功能
1. <table> 表格标签：

<table> 标签用于创建表格，可以包含行（<tr>）、表头单元格（<th>）和数据单元格（<td>）等。

<table>
  <tr>
    <th>姓名</th>
    <th>年龄</th>
  </tr>
  <tr>
    <td>张三</td>
    <td>25</td>
  </tr>
  <tr>
    <td>李四</td>
    <td>30</td>
  </tr>
</table>
2. <form> 表单标签：

<form> 标签用于创建表单，允许用户输入和提交数据。它可以包含文本字段、复选框、单选按钮等。

<form action="submit.php" method="post">
  <input type="text" name="username" placeholder="用户名">
  <input type="password" name="password" placeholder="密码">
  <button type="submit">提交</button>
</form>
3. <fieldset> 和 <legend> 组合标签：

<fieldset> 标签用于创建一组相关的表单元素，而 <legend> 标签用于为这组元素提供标题。

<fieldset>
  <legend>联系信息</legend>
  <label for="name">姓名：</label>
  <input type="text" id="name" name="name">
  <!-- 其他表单元素 -->
</fieldset>
4. <label> 标签：

<label> 标签用于为表单元素提供标签文本，提高表单的可读性和可访问性。通常，<label> 与相关的表单元素通过 for 属性进行关联。

<label for="email">电子邮件：</label>
<input type="email" id="email" name="email">
5. <select> 和 <option> 下拉选择框标签：

<select> 标签用于创建下拉选择框，而 <option> 标签用于定义选项。

<select name="country">
  <option value="us">美国</option>
  <option value="ca">加拿大</option>
  <option value="uk">英国</option>
</select>
6. <input type="file"> 文件上传标签：

<input type="file"> 标签用于允许用户选择并上传文件。

<label for="file">选择文件：</label>
<input type="file" id="file" name="file">

7. <progress> 进度标签：

<progress> 标签用于显示任务的完成进度，通常用于上传或下载任务等。

<progress value="50" max="100">50%</progress>
8. <details> 和 <summary> 标签：

<details> 和 <summary> 标签用于创建可折叠的内容区域，允许用户单击摘要来显示或隐藏详细信息，这在创建交互性网页时非常有用。

<details>
  <summary>显示更多信息</summary>
  <p>这里是更多的详细内容。</p>
</details>
这些是用于创建表格、表单以及其他高级功能的HTML标签。HTML提供了丰富的功能，可以满足各种不同类型的网页需求。

{{< timeline date="2025-10-01" title="国庆节" description="祖国生日快乐" tags="节日" url="" >}}
