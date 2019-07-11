牛客网学习笔记

下面标签嵌套正确的是
正确答案: D   你的答案: C (错误)<br>
`<ul><p>牛客网</p></ul>`<br>
`<a href="#"><a href="#">牛客网</a></a>`<br>
`<dl><li>牛客网</li></dl>`<br>
`<ol><li>牛客网</li></ol>`<br>

A.ul只能紧挨着li<br>
B.a中不能再嵌套a<br>
C.dl dt<br>
D.ol li是有序排列<br>
总结：
ul+li 是无序列表
ol+li 是有序列表
dl+dt+dd 是自定义列表

HTML5 新增的表单元素：datalist、keygen、output<br>
datalist 元素规定输入域的选项列表。 keygen 元素的作用是提供一种验证用户的可靠方法。 output 元素用于不同类型的输出<br>
其中datalist语法练习记录：<br>
姓名：<input type="text" list="name" />
		<datalist id="name">
			<option value="1">zhangsan</option>
			<option value="2">lisi</option>
		</datalist>
input里面要写list="xxx" 然后datalist里面id="xxx"才可以生效
mailto 后面加发送邮件地址<br>
a) 置换元素：浏览器根据元素的标签和属性，来决定元素的具体显示内容。 <br>
例如：浏览器会根据`<img>`标签的src属性的 值来读取图片信息并显示出来，而如果查看(x)html代码，则看不到图片的实际内容；`<input>`标签的type属性来决定是显示输入框，还是单选按钮等。 (x)html中的`<img>、<input>、<textarea>、<select>、<object>` 都是置换元素。这些元素往往没有实际的内容，即是一个空元素。置换元素在其显示中生成了框，这也就是有的内联元素能够设置宽高的原因。<br>
b) 不可替换元素：(x)html 的大多数元素是不可替换元素，即其内容直接表现给用户端（如浏览器）。例如标签`<label>`是一个非置换元素，文字label中的内容”将全被显示。<br>
总结：<br>
置换元素：`<img>、<input>、<textarea>、<select>、<object> <br>`
下面哪条声明能固定背景图片（）   <br>
正确答案: A   你的答案: A (正确)<br>
background-attachment:fixed;<br>
background-attachment:scroll;<br>
background-origin: initial;<br>
background-clip: initial;<br>
总结：<br>
background-attachment :定义背景图片随滚动轴的移动方式 <br>
取值: scroll | fixed | inherit <br>
scroll: 随着页面的滚动轴背景图片将移动 <br>
fixed: 随着页面的滚动轴背景图片不会移动 <br>
inherit: 继承初始值: scroll <br>

