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

## CSS学习笔记
***
#### CSS Cascade Style Sheet级联样式表
### CSS选择器
选择器 |示例 |含义
---|---|---
通用选择器 |*{...} |选择页面中的所有元素
元素选择器 |元素名{...} |选择指定的元素
ID选择器 |#ID值{...} |仅选择具有指定ID的元素
类别选择器 |.类名{...} |选择具有指定class的所有元素
子元素选择器 |选择器1 选择器2{...} |选择可被选择器1选择的元素下的所有子元素中可被选择器2选中的元素
直接子元素选择器 |选择器1>选择器2{...} |选中选择器1中的直接子元素中可被选择器2选中的
并列/过滤选择器 |选择器1 选择器2{...} |选择可被两个选择器同时选定的元素
多选/群组选择器 |选择器1，选择器2，...选择器n{...} |选择可被任何一个选择器选中的元素
伪类选择器 |:伪类名{...} |

### CSS样式属性

#### 尺寸属性
属性名 |含义 |可取值
---|---|---
width |block生效 |值/%
height |block生效 |
min-width
max-width
min-height
max-height

#### background背景属性
属性名 |含义 |可取值
---|---|---
background-color |元素背景色：内容+填充+边框,<br>不会占据外间距 |
background-image |背景图片 |url(xx.png) 
background-repeat ||
background-position |背景图的位置 |
background-attachment |背景滚动方式 |
background | |
background-image | |

#### border边框属性
属性名 |含义 |可取值
---|---|---
border-width |宽度<br>可用上右下左顺序指定4个值 |
border-style |样式<br>可用上右下左顺序指定4个值 |none,solid,double,dotted...
border-color |颜色<br>可用上右下左顺序指定4个值 |可以用transparent表示透明色
border |样式的集合，占用页面空间 |宽度 样式 颜色
outline |外轮廓，不占用页面空间 |颜色 样式 宽度
border-radius |边框半径，绘制圆角边框 |百分比
box-shadow |边框投影，不占用页面空间 |
border-image-source | |
border-image-width | |
border-image-repeat | |
border-image |使用图片做边框 |source：url(xx.png)<br>width:边框宽/九宫格格宽<br>repeat：stretch/repeat/round

#### font字体属性
属性名 |含义 |可取值
---|---|---
font-family |字体系列 |
font-size |字号 |px在老版IE中无法缩放<br>%<br>em
font-weight |字体粗细，代替B标签 |thicker、thick、normal、bold、bolder、100~900
font-style |字体样式，代替I标签 |normal、italic斜体、oblique斜体
font-variant |字体变数/变化 |normal、samll-caps小写字母会转换为大写字母
font |集合属性<br>style、variant、weight、size、family |font:2em 'Arial';

#### 文本属性
属性名 |含义 |可取值
---|---|---
color |文本颜色、前景色 |
text-align |文本水平对齐方式，只对block元素有效 |left center right
text-decoration |文本的修饰方式 |none 取消<a>的下划线 <br> underline <br> linet-hrough <br> overline
text-indent |文本缩进 |em px
text-shadow |文本阴影 |x y blur color
line-height |定义行高 |em：定义多行内容的行间距 <br> px：定义行高与区块的高一样，实现单行文本的竖直居中
text-overflow |溢出的文本如何显示 |clip：剪断不可见的文本 <br> ellipsis：若有不可见的文本，显示为...
word-wrap |单词包裹方式 |
word-break |单词打断方式 |
white-sapce ||
vertical-align ||用在td/th中或display:table-cell元素中：让当前元素中的文本在竖直方向上居中<br>用在IMG/TEXTAREA等inline-block元素中：让当前元素同一行中的其它元素与自己的竖直方向上的对齐方式

#### 列表属性
属性名 |含义 |可取值
---|---|---
list-style-type |列表前的提示符号 |none/disc/circle/square...
list-style-image |使用图片来代替默认列表项提示符号 |
list-style-position |列表项的标号处于li外部还是内部 |
list-style |集合属性 |

#### animation动画属性
属性名 |含义 |可取值
---|---|---
animation-name |动画的名称 |
animation-duration |动画的持续时间 |
nimation-timing-function |动画的播放速度函数 |linear/ease-in/ease-out/ease-in-out
animation-delay |播放的延时时间 |
animation-iteration-count |动画播放次数 |如3、10、infinite（循环播放）
animation-direction |播放方向 |normal（第二次播放时从第一帧重新开始）<br> alternate（第偶数次播放时从最后一帧倒序播放）
animation |集合属性<br>name duration timing-function delay count direction |
animation-fill-mode | |backwards：动画尚未开始时即处于第一帧状态 <br> forwards：动画完后保持最后一帧状态 <br> both：上述二者的效果都要
animation-play-state | |paused（动画处于暂停状态）<br>running（动画处于运行状态）

### CSS布局属性
#### 定位属性
属性名 |含义 |可取值
---|---|---
overflow |溢出 |visible：默认值，超出的内容会显示在元素框外<br>hidden：超出的内容隐藏<br>scroll：有滚动条<br>auto：内容超出就有滚动条，不超出就没有
visibility |指定元素是否可见 |visibility:visible; 元素可见<br>visibility:hidden; 元素隐藏，但不释放所占的页面空间
dispaly |元素的显示模式 |display:none;元素消失，释放所占的页面空间<br>block：如div，独立占一整行，可以指定width/height<br>inline：如span，可与其他元素同处一行，不能指定width/height<br>inline-block：如img，可与其他元素同处一行，但可以指定width/height<br>table/table-cell：可使用vertical-align属性，IE6不支持
float |浮动 |none：默认值元素不浮动<br>left：元素向左浮动<br>right：元素向右浮动
clear |清除浮动 |none<br>left：清除之前的元素由于向左浮动对自己造成的影响<br>right：清除之前的元素由于向右浮动对自己造成的影响
position |定位 |static：默认值，就是流定位<br>relative：相对定位<br>absolute：绝对定位<br>fixed：固定定位<br>sticky：粘性定位
cursor |鼠标指针形状 |pointer：小手<br>move：可移动指示<br>text：可在此处进行文本输入<br>crosshair：显示为十字
clip |裁剪 |rect(top,right,bottom,left)

#### 表格属性
属性名 |含义 |可取值
---|---|---
border-collapse |表格边框合并/崩塌方式，用于TABLE |separate：分隔<br>collapse：崩塌
border-spacing |表格单元格间距；用于TABLE，边框分隔时使用 |

#### box-sizing
属性名 |含义 |可取值
---|---|---
content-box | |width=内容区
border-box | |width=内容区+内边距+边框

#### 多列属性
属性名 |含义 |可取值
---|---|---
column-count |竖直方向上列的数量 |
column-gap |内容列与列间距，每列文本的高度 |
column-width |每列文本的宽度 |
colunm-rule |集合属性 |width style color

#### flex弹性盒属性
#### 给父元素设置display:flex;
属性名 |含义 |可取值
---|---|---
flex-direction |决定主轴的方向 |row 默认值，从左向右<br>row-reverse<br>column 纵向排列<br>column-reverse
flex-wrap |指定弹性盒子的子元素换行方式 |nowrap 默认，弹性容器为单行<br>wrap 弹性容器为多行，弹性子项溢出部分会被放置到新行，子项内部会产生断行<br>wrap-reverse
justify-content |横轴对齐方式 |flex-star 默认值，行头开始<br>flex-end 行尾开始<br>center 居中分布<br>space-between 平均分布<br>space-around 平均分布，两边留一半间隔空间
align-items |纵轴对齐方式（单行）|flex-star<br>flex-end<br>center<br>baseline<br>stretch
align-content |纵轴对齐方式（多行）<br>用于修改flex-wrap |stretch 默认，各行伸展占剩余空间<br>flex-start 各行向弹性容器起始堆叠<br>flex-end<br>center<br>space-between 各行在弹性容器中平均分布<br>space-around 两端留间隔，间隔大小是子元素之间间距的一半
flex |指定弹性子元素如何分配空间 |flex-grow:n; 按比例分配剩余空间<br>flex-shrink:n; 按比例减少多出的空间<br>flex-basis 默认基准<br>auto 计算值为 1 1 auto<br>initial 计算值为 0 1 auto<br>none 计算值为 0 0 auto<br>inherit 从父元素继承
flex:参数一，参数二，参数三； |集合属性 |
order:n; |定义元素的排列顺序 |n为整数，数值越小越靠前，默认为0
align-self |定义单个元素在纵轴方向的方式 |flex-start<br>flex-end<br>strech<br>baseline<br>center

