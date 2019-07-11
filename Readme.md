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
置换元素：`<img>、<input>、<textarea>、<select>、<object> `<br>


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

display: none和visibility:hidden的区别就是visibility:hidden会保留元素的空间<br>
repaint(重绘) ，repaint发生更改时，元素的外观被改变，且在没有改变布局的情况下发生，如改变outline,visibility,background color，不会影响到dom结构渲染。<br>
reflow(渲染)，与repaint区别就是他会影响到dom的结构渲染，同时他会触发repaint，他会改变他本身与所有父辈元素(祖先)，这种开销是非常昂贵的，导致性能下降是必然的，页面元素越多效果越明显。<br>
所以display:none才会产生reflow<br>
visibility:hidden只会触发repaint<br>
总结：<br>
display:none可以理解为看不见摸不着 <br>
visibility：hidden可以理解为看不见摸得着 <br>
display的切换会触发reflow，而visibility不会。<br>

标准盒子模型 ＝ margin + border + padding + content （content =  width | height）<br>
IE盒子模型 ＝ margin + content （content = border + padding + width | height）<br>
（width|height指的是content的宽|高）

下面哪个属性不会让 div 脱离文档流（normal flow）？
正确答案: C   你的答案: C (正确)
position: absolute;
position: fixed;
position: relative;
float: left;

A：position: absolute;生成绝对定位的元素，相对于static 定位以外的第一个父元素进行定位；都绝对定位了，肯定脱离了文档流。
B:position: fixed;生成绝对定位的元素，相对于浏览器窗口进行定位;相对于浏览器了，也和正常顺序排下来没什么关系。
C:position: relative;生成相对定位的元素，相对于其正常位置进行定位。生成相对定位，也就是说还在原本的上下左右之间，上下左右的元素都不变，so这个没有能脱离文档流。
D:float: left;都浮动出去了，还上哪保持原位置去。
最终答案选择C

text-transform:capitalize是首字母大写
text-transfrom:lowercase是全部字母为小写
text-transfrom:uppercase是全部字母为大写
font-weight: bold;字体为粗体，
用法：`#p{text-transform:lowercase;}`

假设在今日头条里面,有很多工作人员检查新闻是不是属于虚假新闻,所有新闻真实率到达了98%,工作人员在检验一个真实的新闻把它检验为一个虚假的新闻的概率为2%,而一个虚假的新闻被检验为真实的新闻的概率为5%.那么,一个被检验为真实的新闻确实是真实的新闻的概率是多大?
解：
假设总共100个新闻，那么真实新闻为98个，虚假新闻为2个，检验为真实的新闻 总个数为真实的检验为真实的 和虚假的检验为真实的 之和：98x(1-2%)+2x5%=96.14个，其中检验为真实的真实新闻个数即是真实的检验为真实的 个数：98x(1-2%)=96.04个，所以其真实概率为96.04/96.14=0.9989

现在有两堆石子,小今与小条玩游戏,2个人都足够聪明,两个人规定:每次每人只能从其中一堆中取走1个或2个或3个石子,最后将石子全部取完的人胜利.现在两堆石子的个数为8和9,请问如何安排才能让小今必胜?
解：
以4为倍数，取完后两堆石头为0 0，0 4，4 4,8 4，8 8的必胜。如A取完为4 4，无论B怎么取，A都能保证为0 4，B再取，A就可以为0 0，就赢了。同理,A只要保证取完为8 8，就一定可以保证自己可以获得4 4，还可以一直往上推，12 12.....


以下描述正确的：
正确答案: B C D   你的答案: A C (错误)
Http协议所使用的运输层协议是UDP
Https的端口号是443
TCP注重数据可靠性，UDP注重数据传输快
传输层提供端到端的可靠报文传递和错误恢复

总结：
HTTP的端口号是80，https的端口号是443，两者不能混淆了。

OSI七层模型
7 应用层：允许访问网络资源。 通信单位：报文（指的是TCP/IP协议里广义的应用层 ） 
6 表示层：数据的转换，加密，压缩  
5 会话层：建立，管理，终止会话  
4 运输层：提供可靠的进程到进程的交付和差错恢复。  
3 网络层：从源到终点传送分组，提供网络互联。通信单位 数据报 
2 数据链路层：将比特组织成帧结构，提供逐跳交付。通信单位 帧 
1 物理层：经过媒体传送比特

TCP与UDP
UDP（ User Datagram Protocal， 用户数据报协议 ）
（1）简介
面向数据报的不可靠的 传输层通信协议
（2）特点
UDP不能保证可靠传输，也就更不能保证所发送的数据的到达顺序，它所实现的是尽最大的努力交付。
UDP是面向数据报文的、无连接的协议，因此它的开销低并且发送器前的时延小（因为不用建立连接啊），面向报文也使得IP层在传输UDP协议的报文时既不会拆分也不会合并。
UDP可以支持一对一、一对多、多对一、多对多的通信。
UDP没有拥塞控制功能，它的发送速率不会随着网络出现的拥塞而降低，所以它的实时性较好。这也是许多视频聊天应用采用它的原因。
（3）报文格式

TCP（ Transmission Control Protocol， 传输控制协议  ）
（1）简介
面向连接的、可靠的、基于字节流的传输层通信协议
（2）特点
TCP协议保证可靠传输，也就是说发送的数据是什么样，接收的数据也是什么样。
TCP协议是有连接的、面向数据流的协议。有连接是说数据传送前通信双方需要建立连接、通信完毕后需要断开连接，不过这里所提到的连接都是逻辑上的连接。面向数据流的意思是说发送方应用程序发送的数据是什么顺序，接收方应用读取的接收到的数据也是什么顺序。
TCP协议提供的是端到端的通信，也就是说一条TCP连接只能提供一对一的通信。不过，一个应用可以同时建立多条TCP连接来实现与多个目标的通信。
TCP协议提供拥塞控制功能，会在网络状况良好的情况下适当提高发送/接收速率，反之则适当降低发送/接收速率。这样，将会提高对网络的利用率。
（3） 数据封包结构

SQL提供了四种匹配模式：
1. % 表示任意0个或多个字符。如下语句：Select * FROM user Where name LIKE '%三%'; 将会把name为“张三”，“三脚猫”，“唐三藏”等等有“三”的全找出来。%三：表示左匹配。三%：表示右匹配。
%三%：表示模糊查询。
2. _ 表示任意单个字符。语句： Select * FROM user Where name LIKE '_三_'；只找出“唐三藏”。这样name为三个字且中间一个字是“三”的； Select * FROM user Where name LIKE '三__'； 只找出“三脚猫”这样name为三个字且第一个字是“三”的；
3. [ ] 表示括号内所列字符中的一个（类似与正则表达式）。语句：Select * FROM user Where name LIKE '[张李王]三'; 将找出“张三”、“李三”、“王三”（而不是“张李王三”）； 如 [ ] 内有一系列字符（01234、abcde之类的）则可略写为“0-4”、“a-e“。Select * FROM user Where name LIKE '老[1-9]'；将找出“老1”、“老2”、……、“老9”；如要找“-”字符请将其放在首位：'张三[-1-9]'；
4. [^ ] 表示不在括号所列之内的单个字符。语句：Select * FROM user Where name LIKE '[^张李王]三'；将找出不姓“张”、“李”、“王”的“赵三”、“孙三”等；Select * FROM user Where name LIKE '老[^1-4]'; 将排除“老1”到“老4”寻找“老5”、“老6”、……、“老9”。
5.* 表示查找的是所有信息,例如select * from tbl_user


