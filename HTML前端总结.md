# HTML前端总结

## 第二天学习

###              表格
(没有列说法只有行和单元格）

- 组成

	- table  创建表格
tr   行
td  单元格
th  表头（加粗居中）

- 属性

	- cellspacing  单元格与单元格之间距离
cellpadding  单元格内容与单元格边框距离

- 表格标题

	- caption  在表格里面标题居中显示

- 合并单元格

	- 跨行合并  rowspan
跨列合并  colspan
	- 先上后下，先左后右
	- 合并后删除多余单元格

### 列表

- 无序

	- <ul>
<li></li>
</ul>

- 有序

	- <ol>
<li></li>
</ol>

- 自定义

	- <dl>
<dt></dt>
<dd></dd>
</dl>

### 表单

- 表单三部分

	- 表单域   form
	- 提示信息
	- 表单控件

		- input  的 type属性

			- text  文本框
			- password  密码框
			- radio  单选框
			- checkbox  复选框
			- button  普通按钮
			- submit  提交按钮
			- reset  重置按钮
			- image  图片按钮
			- file  文件域

		- select
下拉菜单

			- <select>
<option></option>
</select>

		- <textarea></textarea>
文本域

	- 其他属性

		- required=“required”
内容不能为空
		- placeholder
占位符
		- autofocus=“autofocus”
自动对焦到输入框
		- autocomplete=“off/on"
点击输入框会有上次的输入记录提示
注：需要放在表单里并且加上name
同事成功提交
		- multiple=“multiple”
可以多选文件提交

### 表单属性

- name
表单名称区分对应表单和后端对接接口
- value
表单的值
- checked
默认选中状态
- required
验证表单是否为空
- readonly
只读属性
- disabled
禁用状态
- placeholder
提示占位符
- pattern要和required连用
和正则表达式连用验证更严格
^表示正则表达式开始符号
\d表示阿拉伯数字0-9
[]选择里面的字符
{}表示前面的字符出现的次数
{9}表示出现9次，{2，}出现打于2次，{2,5}表示出现2-5次

## 第一天学习

### <hr />横线

### <br /> 换行标签

### div   span标签

### 文本格式化
（XHTML推荐）第二个

- <b></b>
<strong></strong>
都是加粗字体，strong另外还有强调
- <i></i>
<em></em>
字体倾斜
- <s></s>
<del></del>
加删除线
- <u></u>
<ins></ins>
加下划线

### <img />
插入图片

- src
文件路径
- alt
图片不能显示替换文本
- title
鼠标悬停时显示文字
- width   height
图片大小  px
不支持百分比
- border   后面数字
设置图片宽度

### <a></a>
添加链接

- href
指定URL

	- mailto:
加邮箱

- target
链接打开方式

	- self
默认打开
	- _blank
新窗口打开

### 锚点链接

- id=“one"
href="#one"

### <base target="_blank"/>
在head标签里面，所有链接将在新窗口打开

### <pre></pre>
预格式化，原样输出显示

### 特殊字符

- &nbsp;空格符
&lt;小于号
&gt;大于号
&amp;     &号
&yen;人民币符
&copy;版权

*XMind: ZEN - Trial Version*