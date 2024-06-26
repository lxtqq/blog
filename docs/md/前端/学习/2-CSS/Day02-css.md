# CSS

## 简介

> CSS（Cascading Style
>
> Sheets）是一种用于网页样式设计的语言，它定义了网页的布局、颜色、字体、大小、背景、边框等视觉效果，可以实现对网页的美化和布局控制。使用CSS，网页的样式和结构可以分离，使得网页的内容和样式>
> 可以分别维护和修改，提高了网站的可维护性和可重用性。
>
> 具体来说，CSS可以实现以下功能：
>
> 1. 网页的布局控制，可以定义网页的盒子模型、定位方式、浮动、清除浮动等。
>
> 2. 网页的颜色、背景、边框、阴影等样式的定义，可以让网页看起来更加美观。
>
> 3. 网页的字体、大小、行高、对齐等文本样式的定义，可以让网页的内容更加易读。
>
> 4. 网页的交互效果的实现，例如鼠标悬停、点击、选中等事件的处理，可以增强网页的用户体验。
>
> 5. 响应式设计，根据设备的屏幕大小和方向，调整网页的布局和样式，适应不同的设备和分辨率。
>
> 总之，CSS是一种非常重要的网页设计语言，能够使网页更加美观、易读、易用和响应式，并提高网页的可维护性和可重用性。

## 样式

### 样式-边框

|                样式                | 说明                                                         |
| :--------------------------------: | :----------------------------------------------------------- |
|       border: 2px solid red;       | 实线边框，solid：实线，dashed 虚线，dotted ：点线，double 双线边框，none 无边框 |
| border-radius: 5px 15px 10px 20px; | 圆角的边框,需要与 `border` 属性一起使用，左 上5 像素，右上 15 像素，右下 10 像素，左下20 像素，在图片使用，方角图片变圆角 |
| box-shadow: 10px 10px 5px #888888; | 盒子阴影，表示给 `div` 元素添加一个阴影效果，阴影位于元素右下方 `10px` 的位置，阴影边缘清晰度为 `5px`，阴影的颜色为深灰色。 |
|           padding: 10px            | 内边距，内框到元素的距离                                     |
|            width:300px;            | 宽度 300像素                                                 |
|           height:100px;            | 高度 100像素                                                 |


### 样式-边框-复合属性

|                         样式                         | 说明                                                         |
| :--------------------------------------------------: | :----------------------------------------------------------- |
|                 background:#dddddd;                  | 一个复合属性，用于设置元素的背景。它可以包括多个子属性，这些子属性可以单独设置或组合在一起使用。背景色，可以是英语单词颜色，也可以是颜色值 |
|              background-color: #c5cedb;              | 背景色                                                       |
| background-image: url('/logo.png'),url('/logo.png'); | 背景图片,多个以逗号隔开                                      |
|     background-position: right bottom, left top;     | 设置背景图像的位置，使用逗号分隔多个位置。在这个例子中，第一个背景图像的位置设置为右下角，第二个背景图像的位置设置为左上角。配合image使用，contain自适应，center水平居中 |
|                   background-size                    | 配合image使用，contain自适应，center水平居中                 |
|        background-repeat: no-repeat, repeat;         | 配合image使用，默认值，表示背景图片在水平和垂直方向上都重复显示； `repeat-x`：表示背景图片只在水平方向上重复显示； `repeat-y`：表示背景图片只在垂直方向上重复显示； `no-repeat`：表示背景图片不重复显示，只显示一次。设置背景图像的重复方式，使用逗号分隔多个重复方式。在这个例子中，第一个背景图像不重复，第二个背景图像重复。 |

### 样式-边框-拖拽、偏移

| 样式                  | 说明                                                         |
| --------------------- | ------------------------------------------------------------ |
| resize:both;          | 允许用户通过拖动元素的边框来调整其尺寸。`both` 值表示元素的水平和垂直尺寸都可以调整。这通常用于 textarea 或可调整大小的元素，以允许用户根据需要调整元素的尺寸 |
| overflow:auto;        | 定义了当元素内部内容超出其指定尺寸时的处理方式。`auto` 值表示当内容溢出时，元素会自动显示滚动条以使用户能够查看超出尺寸范围的内容。如果内容没有溢出，滚动条将不可见。 |
| outline-offset:-15px; | 给当前的边框偏移出一个边框                                   |



### 样式-文本样式

|               样式                | 说明                                                         |
| :-------------------------------: | :----------------------------------------------------------- |
| text-shadow: 5px 5px 5px #ffc107; | text-shadow: h-shadow v-shadow blur-color;<br />  `h-shadow`：表示阴影的水平偏移量。可以是一个正值（向右偏移）或负值（向左偏移）。<br />  `v-shadow`：表示阴影的垂直偏移量。可以是一个正值（向下偏移）或负值（向上偏移）。 <br />  `blur-color`：表示阴影的模糊半径和颜色。模糊半径是一个可选值，用于指定阴影的模糊程度。如果不指定模糊半径，阴影将没有模糊效果。颜色可以使用颜色名称、十六进制值或 RGB 值表示。5px #ffc107，表示阴影有一个模糊半径为5个像素，颜色为 #ffc107（一种橙色） |
|        text-overflow:clip         | 设置了当文本内容溢出元素框时如何处理。<br />`clip`：表示文本溢出的部分将被裁剪，不会显示出来。<br />`ellipsis`：超出部分将被省略并用省略号表示。 |
|       word-wrap:break-word;       | 文本超过盒子宽度就换行。                                     |



### 样式-字体

|    样式     | 说明 |
| :---------: | :--- |
| font-family |      |
|             |      |