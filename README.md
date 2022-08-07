# BYD_STUDY
## HTML学习笔记
***
#### HTML文档的基本结构  
  ```html
  <!DOCTYPE html>
  <html>
    <head>
      <title></title>
    </head>
    <body>
    </body>
  </html>
  ```
#### 语义标签分两种：  
  1、inline，可与其他元素在一行内，常用的有span、strong、a...  
  2、block，单独占一行，常用的有h1-h6、img、div、table...  
#### table  

标签 |含义 |常用属性
---|---|---
th |theadercell表头单元格 |  
tr |trow行 |  
td |tdatacell表中数据单元 |align：left/center/right<br>valign:top/middle/bottom<br>rowspan:跨越的行数<br>colspan：跨越的列数
#### list

标签 |含义 |常用属性
---|---|---
ol |orderedlist有序列表 |type:1/a/A/i/I
ul |unorderedlist无序列表 |type:disc/circle/square
dl |definitionlist定义列表 |
li | |
#### form

标签 |含义 |常用属性
---|---|---
form |表单 |action：指定表单数据的处理页面<br>method：GET/POST<br>GET：把请求数据追加在地址栏查询字符串中（有长度限制)<br>POST：把数据以单独的数据包发送给服务器（无长度限制且可用于文件上传）

#### 页面布局
1. TABLE布局：过时
2. DIV+CSS：当前主流，表达的语义不清
3. HTML5布局标签：未来趋势
```html
<header></header>
<nav></nav>         navigator
<article></article>
<content></content>
<footer></footer>
<aside></aside>
<section></section>
```
## task1_internship完成个人简历
### code files: [internship.html](task1_internship/internship.html), [internship.css](task1_internship/internship.css)
### 成果展示：[个人简历.pdf](task1_internship/个人简历.pdf)
将写好的个人简历html文件打印成pdf
