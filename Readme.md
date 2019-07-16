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
例如：
浏览器会根据`<img>`标签的src属性的 值来读取图片信息并显示出来，而如果查看(x)html代码，则看不到图片的实际内容。<br>
`<input>`标签的type属性来决定是显示输入框，还是单选按钮等。 <br>
html中的`<img>、<input>、<textarea>、<select>、<object>` 都是置换元素。<br>
这些元素往往没有实际的内容，即是一个空元素。置换元素在其显示中生成了框，这也就是有的内联元素能够设置宽高的原因。<br>
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
<br>
下面哪个属性不会让 div 脱离文档流（normal flow）？<br>
正确答案: C   你的答案: C (正确)<br>
position: absolute;<br>
position: fixed;<br>
position: relative;<br>
float: left;<br>

A：position: absolute;生成绝对定位的元素，相对于static 定位以外的第一个父元素进行定位；都绝对定位了，肯定脱离了文档流。<br>
B:position: fixed;生成绝对定位的元素，相对于浏览器窗口进行定位;相对于浏览器了，也和正常顺序排下来没什么关系。<br>
C:position: relative;生成相对定位的元素，相对于其正常位置进行定位。生成相对定位，也就是说还在原本的上下左右之间，上下左右的元素都不变，so这个没有能脱离文档流。<br>
D:float: left;都浮动出去了，还上哪保持原位置去。<br>
最终答案选择C<br>

text-transform:capitalize是首字母大写<br>
text-transfrom:lowercase是全部字母为小写<br>
text-transfrom:uppercase是全部字母为大写<br>
font-weight: bold;字体为粗体，<br>
用法：`#p{text-transform:lowercase;}`<br>

假设在今日头条里面,有很多工作人员检查新闻是不是属于虚假新闻,所有新闻真实率到达了98%,工作人员在检验一个真实的新闻把它检验为一个虚假的新闻的概率为2%,而一个虚假的新闻被检验为真实的新闻的概率为5%.那么,一个被检验为真实的新闻确实是真实的新闻的概率是多大?<br>
解：<br>
假设总共100个新闻，那么真实新闻为98个，虚假新闻为2个，检验为真实的新闻 总个数为真实的检验为真实的 和虚假的检验为真实的 之和：98x(1-2%)+2x5%=96.14个，其中检验为真实的真实新闻个数即是真实的检验为真实的 个数：98x(1-2%)=96.04个，所以其真实概率为96.04/96.14=0.9989<br>

现在有两堆石子,小今与小条玩游戏,2个人都足够聪明,两个人规定:每次每人只能从其中一堆中取走1个或2个或3个石子,最后将石子全部取完的人胜利.现在两堆石子的个数为8和9,请问如何安排才能让小今必胜?<br>
解：<br>
以4为倍数，取完后两堆石头为0 0，0 4，4 4,8 4，8 8的必胜。如A取完为4 4，无论B怎么取，A都能保证为0 4，B再取，A就可以为0 0，就赢了。同理,A只要保证取完为8 8，就一定可以保证自己可以获得4 4，还可以一直往上推，12 12.....<br>


以下描述正确的：
正确答案: B C D   你的答案: A C (错误)
Http协议所使用的运输层协议是UDP
Https的端口号是443
TCP注重数据可靠性，UDP注重数据传输快
传输层提供端到端的可靠报文传递和错误恢复

总结：<br>
HTTP的端口号是80，https的端口号是443，两者不能混淆了。<br>

OSI七层模型
7 应用层：允许访问网络资源。 通信单位：报文（指的是TCP/IP协议里广义的应用层 ） 
6 表示层：数据的转换，加密，压缩  
5 会话层：建立，管理，终止会话  
4 运输层：提供可靠的进程到进程的交付和差错恢复。  
3 网络层：从源到终点传送分组，提供网络互联。通信单位 数据报 
2 数据链路层：将比特组织成帧结构，提供逐跳交付。通信单位 帧 
1 物理层：经过媒体传送比特

TCP与UDP<br>
UDP（ User Datagram Protocal， 用户数据报协议 ）<br>
（1）简介<br>
面向数据报的不可靠的 传输层通信协议<br>
（2）特点<br>
UDP不能保证可靠传输，也就更不能保证所发送的数据的到达顺序，它所实现的是尽最大的努力交付。<br>
UDP是面向数据报文的、无连接的协议，因此它的开销低并且发送器前的时延小（因为不用建立连接啊），面向报文也使得IP层在传输UDP协议的报文时既不会拆分也不会合并。<br>
UDP可以支持一对一、一对多、多对一、多对多的通信。<br>
UDP没有拥塞控制功能，它的发送速率不会随着网络出现的拥塞而降低，所以它的实时性较好。这也是许多视频聊天应用采用它的原因。<br>
（3）报文格式<br>
<br>
TCP（ Transmission Control Protocol， 传输控制协议  ）<br>
（1）简介<br>
面向连接的、可靠的、基于字节流的传输层通信协议<br>
（2）特点<br>
TCP协议保证可靠传输，也就是说发送的数据是什么样，接收的数据也是什么样。<br>
TCP协议是有连接的、面向数据流的协议。有连接是说数据传送前通信双方需要建立连接、通信完毕后需要断开连接，不过这里所提到的连接都是逻辑上的连接。面向数据流的意思是说发送方应用程序发送的数据是什么顺序，接收方应用读取的接收到的数据也是什么顺序。<br>
TCP协议提供的是端到端的通信，也就是说一条TCP连接只能提供一对一的通信。不过，一个应用可以同时建立多条TCP连接来实现与多个目标的通信。<br>
TCP协议提供拥塞控制功能，会在网络状况良好的情况下适当提高发送/接收速率，反之则适当降低发送/接收速率。这样，将会提高对网络的利用率。<br>
（3） 数据封包结构<br>
<br>
SQL提供了四种匹配模式：<br>
1. % 表示任意0个或多个字符。如下语句：Select * FROM user Where name LIKE '%三%'; 将会把name为“张三”，“三脚猫”，“唐三藏”等等有“三”的全找出来。%三：表示左匹配。三%：表示右匹配。%三%：表示模糊查询。<br>
2. _ 表示任意单个字符。语句： Select * FROM user Where name LIKE '_三_'；只找出“唐三藏”。这样name为三个字且中间一个字是“三”的； Select * FROM user Where name LIKE '三__'； 只找出“三脚猫”这样name为三个字且第一个字是“三”的；<br>
3. [ ] 表示括号内所列字符中的一个（类似与正则表达式）。语句：Select * FROM user Where name LIKE '[张李王]三'; 将找出“张三”、“李三”、“王三”（而不是“张李王三”）； 如 [ ] 内有一系列字符（01234、abcde之类的）则可略写为“0-4”、“a-e“。Sele<br>ct * FROM user Where name LIKE '老[1-9]'；将找出“老1”、“老2”、……、“老9”；如要找“-”字符请将其放在首位：'张三[-1-9]'；<br>
4. [^ ] 表示不在括号所列之内的单个字符。语句：Select * FROM user Where name LIKE '[^张李王]三'；将找出不姓“张”、“李”、“王”的“赵三”、“孙三”等；Select * FROM user Where name LIKE '老[^1-4]'; 将排除“老1”到“老4”寻找“老5”、“老6”、……、“老9”。<br>
5.* 表示查找的是所有信息,例如select * from tbl_user<br>

“进程是资源分配的最小单位，线程是CPU调度的最小单位”。<br>
进程：是执行中一段程序，即一旦程序被载入到内存中并准备执行，它就是一个进程。进程是表示资源分配的的基本概念，又是调度运行的基本单位，是系统中的并发执行的单位。
线程：单个进程中执行中每个任务就是一个线程。线程是进程中执行运算的最小单位。
注意：一个线程只能属于一个进程，但是一个进程可以拥有多个线程。多线程处理就是允许一个进程中在同一时刻执行多个任务。
图：
CPU指向线程1/2/3，线程1是进程1的主线程，线程2/3是进程2的线程，其中线程2是进程2的主线程

LRU全称是Least Recently Used，即最近最久未使用的意思。 下面说一下LRU算法的核心思想，LRU算法的设计原则是：如果一个数据在最近一段时间没有被访问到，那么在将来它被访问的可能性也很小。也就是说，当限定的空间已存满数据时，应当把最久没有被访问到的数据淘汰。<br>
FIFO（First in First out），先进先出。在FIFO Cache设计中，核心原则就是： 如果一个数据最先进入缓存中，则应该最早淘汰掉 。也就是说，当缓存满的时候，应当把最先进入缓存的数据给淘汰掉。<br>
LFU（Least Frequently Used）最近最少使用算法。它是基于“如果一个数据在最近一段时间内使用次数很少，那么在将来一段时间内被使用的可能性也很小”的思路。
注意：<br>
1.LFU和LRU算法的不同之处，LRU的淘汰规则是基于访问时间，而LFU是基于访问次数的。<br>
2.FIFO算法会产生当所分配的物理块数增大而页故障数不减反增的异常现象，这是由 Belady于1969年发现，故称为Belady异常。<br>

算法稳定性：
1)冒泡排序

冒泡排序就是把小的元素往前调或者把大的元素往后调。比较是相邻的两个元素比较，交换也发生在这两个元素之间。所以，如果两个元素相等，我想你是不会再无聊地把他们俩交换一下的；如果两个相等的元素没有相邻，那么即使通过前面的两两交换把两个相邻起来，这时候也不会交换，所以相同元素的前后顺序并没有改变，所以冒泡排序是一种稳定排序算法。

(2)选择排序

选择排序是给每个位置选择当前元素最小的，比如给第一个位置选择最小的，在剩余元素里面给第二个元素选择第二小的，依次类推，直到第n - 1个元素，第n个元素不用选择了，因为只剩下它一个最大的元素了。那么，在一趟选择，如果当前元素比一个元素小，而该小的元素又出现在一个和当前元素相等的元素后面，那么交换后稳定性就被破坏了。比较拗口，举个例子，序列5 8 5 2 9，我们知道第一遍选择第1个元素5会和2交换，那么原序列中2个5的相对前后顺序就被破坏了，所以选择排序不是一个稳定的排序算法。

(3)插入排序 
插入排序是在一个已经有序的小序列的基础上，一次插入一个元素。当然，刚开始这个有序的小序列只有1个元素，就是第一个元素。比较是从有序序列的末尾开始，也就是想要插入的元素和已经有序的最大者开始比起，如果比它大则直接插入在其后面，否则一直往前找直到找到它该插入的位置。如果碰见一个和插入元素相等的，那么插入元素把想插入的元素放在相等元素的后面。所以，相等元素的前后顺序没有改变，从原无序序列出去的顺序就是排好序后的顺序，所以插入排序是稳定的。

(4)快速排序 
快速排序有两个方向，左边的i下标一直往右走，当a[i] <= a[center_index]，其中center_index是中枢元素的数组下标，一般取为数组第0个元素。而右边的j下标一直往左走，当a[j] > a[center_index]。如果i和j都走不动了，i <= j，交换a[i]和a[j],重复上面的过程，直到i > j。 交换a[j]和a[center_index]，完成一趟快速排序。在中枢元素和a[j]交换的时候，很有可能把前面的元素的稳定性打乱，比如序列为5 3 3 4 3 8 9 10 11，现在中枢元素5和3（第5个元素，下标从1开始计）交换就会把元素3的稳定性打乱，所以快速排序是一个不稳定的排序算法，不稳定发生在中枢元素和a[j] 交换的时刻。
https://blog.csdn.net/adusts/article/details/80882649

(5)归并排序 
归并排序是把序列递归地分成短序列，递归出口是短序列只有1个元素（认为直接有序）或者2个序列（1次比较和交换），然后把各个有序的段序列合并成一个有序的长序列，不断合并直到原序列全部排好序。可以发现，在1个或2个元素时，1个元素不会交换，2个元素如果大小相等也没有人故意交换，这不会破坏稳定性。那么，在短的有序序列合并的过程中，稳定是是否受到破坏？没有，合并过程中我们可以保证如果两个当前元素相等时，我们把处在前面的序列的元素保存在结果序列的前面，这样就保证了稳定性。所以，归并排序也是稳定的排序算法。

(6)基数排序 
基数排序是按照低位先排序，然后收集；再按照高位排序，然后再收集；依次类推，直到最高位。有时候有些属性是有优先级顺序的，先按低优先级排序，再按高优先级排序，最后的次序就是高优先级高的在前，高优先级相同的低优先级高的在前。基数排序基于分别排序，分别收集，所以其是稳定的排序算法。

(7)希尔排序(shell) 
希尔排序是按照不同步长对元素进行插入排序，当刚开始元素很无序的时候，步长最大，所以插入排序的元素个数很少，速度很快；当元素基本有序了，步长很小， 插入排序对于有序的序列效率很高。所以，希尔排序的时间复杂度会比O(n^2)好一些。由于多次插入排序，我们知道一次插入排序是稳定的，不会改变相同元素的相对顺序，但在不同的插入排序过程中，相同的元素可能在各自的插入排序中移动，最后其稳定性就会被打乱，所以shell排序是不稳定的。

(8)堆排序 
我们知道堆的结构是节点i的孩子为2 * i和2 * i + 1节点，大顶堆要求父节点大于等于其2个子节点，小顶堆要求父节点小于等于其2个子节点。在一个长为n 的序列，堆排序的过程是从第n / 2开始和其子节点共3个值选择最大（大顶堆）或者最小（小顶堆），这3个元素之间的选择当然不会破坏稳定性。但当为n / 2 - 1， n / 2 - 2， ... 1这些个父节点选择元素时，就会破坏稳定性。有可能第n / 2个父节点交换把后面一个元素交换过去了，而第n / 2 - 1个父节点把后面一个相同的元素没 有交换，那么这2个相同的元素之间的稳定性就被破坏了。所以，堆排序不是稳定的排序算法。（一般升序采用大顶堆，降序采用小顶堆)
https://www.cnblogs.com/chengxiao/p/6129630.html

综上，得出结论: 选择排序、快速排序、希尔排序、堆排序不是稳定的排序算法，而冒泡排序、插入排序、归并排序和基数排序是稳定的排序算法
即：
不稳定：快选堆希
稳  定：插冒归基

给定一个Excel表格中的列名称，返回其相应的列序号。<br>
解题思路：<br>
相当于26进制转化成十进制，类似于二进制与十进制之间的转换<br>

AC代码：<br>
JAVA：<br>
class Solution {<br>
public:<br>
    int titleToNumber(string s) {<br>
        int result = 0;<br>
        for(int i = 0; i < s.length(); i++)<br>
        {<br>
            result = result * 26 + (s[i] - 'A' + 1);<br>
        }<br>
        return result;<br>
    }<br>
    <br>
PYTHON：<br>
result = 0<br>
s='BA'<br>
for i in range(len(s)):<br>
    result = result * 26 + (ord(s[i]) - ord('A') + 1);<br>
print (result)<br>
<br>
运行以下程序<br>
    var m= 1, j = k = 0; <br>
    function add(n) { <br>
        return n = n+1; <br>
　 } <br>
    y = add(m); <br>
    function add(n) { <br>
        return n = n + 3; <br>
    } <br>
z = add(m); <br>
y和z的最终结果为:4,4<br>
<br>
js里面没有函数重载的概念，在其他语言中（如java）java中，可以存在同名函数。<br>
在js中，定义了两个同名函数后，后面的函数会覆盖前面定义的函数。<br>
由于存在同名函数，后面的add函数将覆盖第一个add函数，所以两次调用add()返回的值是相同的。<br>
也就是y,z都为4.<br>

(function() {<br>
      var a = b = 5;<br>
  })();   <br>
console.log(b);<br>
console.log(a);<br>
上面的输出结果:<br>
5，Uncaught ReferenceError: a is not defined<br>
解：<br>
第一个考点在于var a=b=5相当于拆解成 b=5; var a=b；<br>
然后，b=5前面没有var，相当于声明为全局变量（这种方式在严格模式下会报错，此题不考虑)。<br>
所以就相当于： var b; (fun…{ var a=b; b=5; })();<br>
console.log(b); //5 <br>
console.log(a); //报错 <br>
此处报错也就是另一个考点，a声明的是函数的局部变量，在函数结束是就销毁了，所以在全局下找不到a，于是报错。<br>

页面有一个按钮button id为 button1，通过原生的js如何禁用？(IE 考虑IE 8.0以上版本)<br>
正确答案: C D   你的答案: B D (错误)<br>
document.getElementById("button1").readolny= true;<br>
document.getElementById("button1").setAttribute(“readolny”,”true”);<br>
document.getElementById("button1").disabled = true;<br>
document.getElementById("button1").setAttribute(“disabled”,”true”);<br>
解：<br>
①disabled和readOnly都是表单的公有属性， readOnly是只读， disabled是禁用。这里问的是禁用，所以是disabled。<br>
②还有就是题目中的 readOnly写成了 readolny<br>
③小知识点：setArrtibute在ie7以前是不能通过style和class设置属性的<br>


页面有一个按钮button id为 button1，通过原生的js 设置背景色为红色？<br>
正确答案: A   你的答案: A (正确)<br>
document.getElementById('button1').style.backgroundColor="red";<br>
关键点：驼峰<br>

现在有一个字符串，你要对这个字符串进行 n 次操作，每次操作给出两个数字：(p, l) 表示当前字符串中从下标为 p 的字符开始的长度为 l 的一个子串。你要将这个子串左右翻转后插在这个子串原来位置的正后方，求最后得到的字符串是什么。字符串的下标是从 0 开始的，你可以从样例中得到更多信息。<br>
using namespace std;<br>
int main()<br>
{<br>
    string st;<br>
    while (cin >> st)<br>
    {<br>
        int n;<br>
        cin >> n;<br>
        while (n--)<br>
        {<br>
            int beg, len, index;<br>
            cin >> beg >> len;<br>
            string temp = st.substr(beg, len);<br>
            index = beg + len;<br>
            reverse(temp.begin(), temp.end());<br>
            st.insert(index, temp);<br>
        }<br>
        cout << st << endl;<br>
    }<br>
    return 0;<br>
}<br>

你作为一名出道的歌手终于要出自己的第一份专辑了，你计划收录 n 首歌而且每首歌的长度都是 s 秒，每首歌必须完整地收录于一张 CD 当中。每张 CD 的容量长度都是 L 秒，而且你至少得保证同一张 CD 内相邻两首歌中间至少要隔 1 秒。为了辟邪，你决定任意一张 CD 内的歌数不能被 13 这个数字整除，那么请问你出这张专辑至少需要多少张 CD ？<br>
import java.util.*;<br>
public class Main{<br>
    public static void main(String[] args){<br>
        Scanner in = new Scanner(System.in);<br>
        while(in.hasNext()){<br>
            int n = in.nextInt();<br>
            int s = in.nextInt();<br>
            int l = in.nextInt();<br>
            int count = (l+1)/(s+1);<br>
            count = Math.min(n, count);<br>
            if(count%13==0){<br>
                count--;<br>
            }<br>
            int sum = n/count;<br>
            int yu = n%count;<br>
            if(yu!=0){<br>
                sum++;<br>
                if(yu%13==0&&(count-yu)==1){//查看最后最后一张专辑的情况，yu是最后一张专辑的歌曲数，如果yu是13的倍数，为了不增加专辑的数量，我们可以考虑从倒数第二张专辑中借一首歌，此时倒数第二张专辑的歌曲数是count-1，若(count-1)==yu，这种情况只能在多出一张专辑。<br>
                    sum++;<br>
                }<br>
            }<br>
            System.out.println(sum);<br>
        }<br>
    }<br>
}<br>
<br>

变量a是一个64位有符号的整数，初始值用16进制表示为：0Xf000000000000000； 变量b是一个64位有符号的整数，初始值用16进制表示为：0x7FFFFFFFFFFFFFFF。 则a-b的结果用10进制表示为多少？<br>
方法一：<br>
0Xf000000000000000补码为1111000000000000000000000000000000000000000000000000000000000000<br>
0x7FFFFFFFFFFFFFFF补码为0111111111111111111111111111111111111111111111111111111111111111<br>
a-b=a+(-b)=<br>
1111000000000000000000000000000000000000000000000000000000000000+<br>
1000000000000000000000000000000000000000000000000000000000000001=<br>
10111000000000000000000000000000000000000000000000000000000000001(高位溢出舍去)<br>
则结果为<br>
0111000000000000000000000000000000000000000000000000000000000001=<br>
2^62+2^61+2^60+1<br>

方法二：<br>
0x7FFFFFFFFFFFFFFF+1=0X8000000000000000，那么<br>
a-b=0Xf000000000000000-0X8000000000000000+1<br>
=0X7000000000000001<br>
=16^15*7+16^0*1<br>
=2^60*7+1<br>
=2^60*(2^2+2^1+2^0)+1<br>
=2^62+2^61+2^60+1<br>

Boolean([]); //true<br>
Number([]); //0<br>
Number({}); // NaN<br>
Number(false); //0<br>

（1）行内元素有：`a b span img input select strong `
（2）块级元素有：`div ul ol li dl dt dd h1 h2 h3 h4…p form`
（3）常见的空元素：`<br> <hr> <img> <input> <link> <meta>`
块元素一般都从新行开始，它可以容纳内联元素和其他块元素,常见块元素是段落标签'P"。“form"这个块元素比较特殊，它只能用来容纳其他块元素。   

跨域：https://segmentfault.com/a/1190000015597029<br>
产生：浏览器的同源策略。<br>
同源策略限制了从同一个源加载的文档或脚本如何与来自另一个源的资源进行交互。这是一个用于隔离潜在恶意文件的重要安全机制。<br>
浏览器是从两个方面去做这个同源策略的，一是针对接口的请求（cookie），二是针对Dom的查询（getElementById）。<br>
解决：<br>
第一种方式：jsonp请求；jsonp的原理是利用<script>标签的跨域特性，可以不受限制地从其他域中加载资源，类似的标签还有<img>.只支持GET请求而不支持POST等其它类型的HTTP请求；它只支持跨域HTTP请求这种情况，不能解决不同域的两个页面之间如何进行JavaScript调用的问题<br>
第二种方式：document.domain；这种方式用在主域名相同子域名不同的跨域访问中<br>
第三种方式：window.name；window的name属性有个特征：在一个窗口(window)的生命周期内,窗口载入的所有的页面都是共享一个window.name的，每个页面对window.name都有读写的权限，window.name是持久存在一个窗口载入过的所有页面中的，并不会因新页面的载入而进行重置。<br>
第四种方式：window.postMessage；window.postMessages是html5中实现跨域访问的一种新方式，可以使用它来向其它的window对象发送消息，无论这个window对象是属于同源或不同源。<br>
第五种方式：CORS；CORS背后的基本思想，就是使用自定义的HTTP头部让浏览器与服务器进行沟通，从而决定请求或响应是应该成功还是应该失败。<br>
第六种方式：Web Sockets；web sockets原理：在JS创建了web socket之后，会有一个HTTP请求发送到浏览器以发起连接。取得服务器响应后，建立的连接会使用HTTP升级从HTTP协议交换为web sockt协议。<br>
不能ajax，因为域名不同不能ajax交互<br>

可继承的样式属性包括（）<br>
正确答案: A C   你的答案: B C D E (错误)<br>
color<br>
background-color<br>
font-size<br>
border<br>
margin<br>
解：<br>
边框，盒子模型，背景属性属于不可继承属性 字体，文本样式属性属于可继承属性<br>
总结：<br>
一、无继承性的属性<br>
1、display：规定元素应该生成的框的类型<br>
2、文本属性：<br>
vertical-align：垂直文本对齐<br>
text-decoration：规定添加到文本的装饰<br>
text-shadow：文本阴影效果<br>
white-space：空白符的处理<br>
unicode-bidi：设置文本的方向<br>
3、盒子模型的属性：width、height、margin 、margin-top、margin-right、margin-bottom、margin-left、border、border-style、border-top-style、border-right-style、border-bottom-style、border-left-style、border-width、border-top-width、border-right-right、border-bottom-width、border-left-width、border-color、border-top-color、border-right-color、border-bottom-color、border-left-color、border-top、border-right、border-bottom、border-left、padding、padding-top、padding-right、padding-bottom、padding-left<br>
4、背景属性：background、background-color、background-image、background-repeat、background-position、background-attachment<br>
5、定位属性：float、clear、position、top、right、bottom、left、min-width、min-height、max-width、max-height、overflow、clip、z-index<br>
6、生成内容属性：content、counter-reset、counter-increment<br>
7、轮廓样式属性：outline-style、outline-width、outline-color、outline<br>
8、页面样式属性：size、page-break-before、page-break-after<br>
9、声音样式属性：pause-before、pause-after、pause、cue-before、cue-after、cue、play-during<br>
二、有继承性的属性<br>
1、字体系列属性<br>
font：组合字体<br>
font-family：规定元素的字体系列<br>
font-weight：设置字体的粗细<br>
font-size：设置字体的尺寸<br>
font-style：定义字体的风格<br>
font-variant：设置小型大写字母的字体显示文本，这意味着所有的小写字母均会被转换为大写，但是所有使用小型大写字体的字母与其余文本相比，其字体尺寸更小。<br>
font-stretch：对当前的 font-family 进行伸缩变形。所有主流浏览器都不支持。<br>
font-size-adjust：为某个元素规定一个 aspect 值，这样就可以保持首选字体的 x-height。<br>
2、文本系列属性<br>
text-indent：文本缩进<br>
text-align：文本水平对齐<br>
line-height：行高<br>
word-spacing：增加或减少单词间的空白（即字间隔）<br>
letter-spacing：增加或减少字符间的空白（字符间距）<br>
text-transform：控制文本大小写<br>
direction：规定文本的书写方向<br>
color：文本颜色<br>
3、元素可见性：visibility<br>
4、表格布局属性：caption-side、border-collapse、border-spacing、empty-cells、table-layout<br>
5、列表布局属性：list-style-type、list-style-image、list-style-position、list-style<br>
6、生成内容属性：quotes<br>
7、光标属性：cursor<br>
8、页面样式属性：page、page-break-inside、windows、orphans<br>
9、声音样式属性：speak、speak-punctuation、speak-numeral、speak-header、speech-rate、volume、voice-family、pitch、pitch-range、stress、richness、azimuth、elevation<br>
三、所有元素可以继承的属性<br>
1、元素可见性：visibility<br>
2、光标属性：cursor<br>
四、内联元素可以继承的属性<br>
1、字体系列属性<br>
2、除text-indent、text-align之外的文本系列属性<br>
五、块级元素可以继承的属性<br>
1、text-indent、text-align<br>
<br>
堆的插入操作：<br>
1.一开始的时候，元素80和其父亲节点比较，发现其大于父亲节点，因此要上溢，将元素80与其父亲节点进行交换<br>
2.交换后再重复上述过程，发现元素80仍然比其父亲节点大，继续上溢，将元素80与其父亲节点进行交换<br>
3.然后再将其与父亲节点比较，发现此时小于其父亲节点的值，说明此时堆中不再存在大小颠倒了，那么此时元素80找到了它在堆中的位置，插入操作结束<br>
<br>
http 请求方式 get 和 post 的区别包括：<br>
get和post的可传输内容大小不一样，一个有限制一个没有限制<br>
get和post传输的内容存放的位置不一样，一个放在header，一个放在body<br>
get的 Content-type不仅可以是 text/html，也可以是其他，如 application/json, text/plain 等等<br>
get请求可以跨域， post一样可以跨域<br>
<br>
typeof Symbol()    //"symbol"（ES6新增）<br>
typeof Number()    //"number"<br>
typeof String()    //"string"<br>
typeof Function()    //"function"<br>
typeof Object()    //"object"<br>
typeof Boolean()    //"boolean"<br>
typeof null    //"object"<br>
typeof undefined    //"undefined"<br>
记忆：<br>
SN SUN BOF（苏宁 太阳 BO5）<br>

老王有两个孩子，已知至少有一个孩子是在星期二出生的男孩。问：两个孩子都是男孩的概率是多大？<br>
解：<br>
先按照两个孩子的四种可能的性别组合进行划分，然后在每种组合里看看满足有至少一个周二男孩的情况数目：<br>
姐妹俩：不用看了，不满足至少有一个周二男孩的条件。<br>
兄妹俩：那哥哥一定是周二出生的了，妹妹出生的星期数有7种可能。<br>
姐弟俩：弟弟一定是周二出生，姐姐出生的星期数有7种可能。<br>
兄弟俩：兄弟二人出生的星期数总共有7 * 7 = 49种可能，但其中有6 * 6 = 36种都不满足至少有一个人是周二出生的条件，因此实际上有49 - 36 = 13种可能。<br>
因此，满足条件的情况（这里的情况是指综合考虑孩子的性别和出生星期数）总数为7 + 7 + 13 = 27。<br>
而其中有13中可能对应于两个孩子都是男孩。因此题目所求概率是13 / 27。<br>
<br>
TCP连接建立(“三次握手”)<br>
分为三步：<br>
（1）客户机的TCP向服务器的TCP发送一个连接请求报文段，其中不含应用层数据，首部中的SYN标志位被置为1。客户机会随机选择一个起始序号seq=x(连接请求报文不携带数据，但要消耗一个序号)。<br>
(SYN = 1, seq = x)<br>
（2）服务器的TCP收到连接请求报文段后，如同意建立连接，就向客户机发回确认，并为该TCP连接分配TCP缓存和变量。确认报文段中SYN和ACK位都被置为1，确认号字段的值为x+1，并且服务器随机产生起始序号seq = y(确认报文不携带数据，但也要消耗掉一个序号)。确认报文段同样不包含应用层数据。<br>
(SYN = 1, ACK = 1, seq = y, ack = x+1)<br>
（3）当客户机收到确认报文段后，还要向服务器给出确认，并且也要分配缓存和变量。报文段的ACK标志位被置1，序号字段为x+1，确认号字段为ack = y+1。该报文段可以携带数据，如果不携带数据则不消耗序号。<br>
(ACK = 1, seq = x+1, ack = y+1)<br>
<br>
TCP连接的释放(“四次挥手”)<br>
分为四步：<br>
（1）客户机打算关闭连接，就向其TCP发送一个连接释放报文段，并停止再发送数据，主动关闭TCP连接，该报文段的FIN标志位被置1，seq = u，它等于前面已传送过的数据的最后一个字节的序号加1(FIN报文段即使不携带数据，也要消耗掉一个序号)。TCP是全双工的，可以想象成是一条TCP连接上有两条数据通路。当发送FIN报文时，发送FIN的一端就不能再发送数据，也就是关闭了其中一条数据通路，但对方还可以发送数据。<br>
(FIN = 1, seq = u)<br>
（2）服务器收到连接释放报文段后即发出确认，确认号是ack = u+1，而这个报文段自己的序号是v，等于它前面已传送过的数据的最后一个字节的序号加1。此时，从客户机到服务器方向的连接就释放了，TCP连接处于半关闭状态。但服务器若发送数据，客户机仍要接收，即从服务器到客户机方向的连接没有关闭。<br>
(ACK = 1, seq = v, ack = u+1)<br>
（3）若服务器已经没有要向客户机发送的数据，就通知TCP释放连接，此时其发出FIN = 1的连接释放报文段。<br>
(FIN = 1, ACK = 1, seq = w, ack = u+1)<br>
（4）客户机收到连接释放报文段后，必须发出确认。在确认报文段中，ACK字段被置为1，确认号ack = w+1，序号seq = u+1。此时TCP连接还没有释放掉，必须经过时间等待计时器设置的时间2MSL后，客户机才进入到连接关闭状态。<br>
(ACK = 1, seq = u+1, ack = w+1)<br>
因此，服务器端结束TCP连接的时间要比客户端早一些。<br>

CSS选择器优先级由高到低可分为：<br>
1.在属性后面使用!important会覆盖页面内任何位置定义的元素样式。<br>
2.作为style属性写在元素内的样式<br>
3.id选择器<br>
4.类选择器 = 伪类选择器 = 属性选择器 （后面的样式会覆盖前面的样式）<br>
5.标签选择器<br>
6.通配符选择器<br>
7.浏览器自定义的样式 <br>

假设 a 是一个由线程 1 和线程 2 共享的初始值为 0 的全局变量，则线程 1 和线程 2 同时执行下面的代码，最终 a 的结果不可能是（）<br>

<br><br>
<br><br>
boolean isOdd = false;

for(int i=1;i<=2;++i)<br>
{<br>
if（i%2==1）isOdd = true；<br>
else isOdd = false；<br>
a+=i*(isOdd?1:-1)；<br>
}<br>
解：<br>
易知：每个线程对a 均做了两次读写操作，分别是 “ +1 ” 和 “ -2 ”<br>
1.AB不并发：此时相当于两个方法顺序执行。A执行完后a=-1，B使用-1作为a的初值，B执行完后a=-2<br>
2.AB完全并发：此时读写冲突，相当于只有一个线程对a的读写最终生效。相同于方法只执行了一次。此时a=-1<br>
3.AB部分并发：假设A先进行第一次读写，得到a=1;之后A的读写被B覆盖了。B使用用1作为a的初值，B执行完后a=0<br>
<br>
算法排序：<br>
https://blog.csdn.net/hai_xiao_tian/article/details/81299229<br>
<br>
Object.defineProperty ：<br>
例子：<br>
var someOne = { };<br>
Object.defineProperty(someOne, "name", {<br>
    value:"coverguo" ,<br>
    configurable: false <br>
});  <br>
delete someOne.name; <br>
console.log(someOne.name);// 输出 coverguo<br>
someOne.name = "linkzhu";<br>
console.log(someOne.name); // 输出coverguo<br>
<br>
PWA技术+web worker+service worker：<br>
https://www.jianshu.com/p/61a1877d4b39<br>
好处：<br>
脱机游戏、加速响应、应用市场……<br>
<br>
设计模式：<br>
https://www.runoob.com/design-pattern/design-pattern-intro.html<br>

工厂模式：<br>
主要解决：主要解决接口选择的问题。<br>
何时使用：我们明确地计划不同条件下创建不同实例时。<br>
如何解决：让其子类实现工厂接口，返回的也是一个抽象的产品。<br>
关键代码：创建过程在其子类执行。<br>
应用实例：您需要一辆汽车，可以直接从工厂里面提货，而不用去管这辆汽车是怎么做出来的，以及这个汽车里面的具体实现。<br>

单例模式：<br>
意图：保证一个类仅有一个实例，并提供一个访问它的全局访问点。<br>
主要解决：一个全局使用的类频繁地创建与销毁。<br>
何时使用：当您想控制实例数目，节省系统资源的时候。<br>
如何解决：判断系统是否已经有这个单例，如果有则返回，如果没有则创建。<br>
关键代码：构造函数是私有的。<br>
应用实例：一个班级只有一个班主任。<br>

装饰器模式：<br>
意图：动态地给一个对象添加一些额外的职责。就增加功能来说，装饰器模式相比生成子类更为灵活。<br>
主要解决：一般的，我们为了扩展一个类经常使用继承方式实现，由于继承为类引入静态特征，并且随着扩展功能的增多，子类会很膨胀。<br>
何时使用：在不想增加很多子类的情况下扩展类。<br>
如何解决：将具体功能职责划分，同时继承装饰者模式。<br>
关键代码：1、Component 类充当抽象角色，不应该具体实现。 2、修饰类引用和继承 Component 类，具体扩展类重写父类方法。<br>
应用实例：孙悟空有 72 变，当他变成"庙宇"后，他的根本还是一只猴子，但是他又有了庙宇的功能。<br>
<br>
观察者模式：<br>
意图：定义对象间的一种一对多的依赖关系，当一个对象的状态发生改变时，所有依赖于它的对象都得到通知并被自动更新。
主要解决：一个对象状态改变给其他对象通知的问题，而且要考虑到易用和低耦合，保证高度的协作。
何时使用：一个对象（目标对象）的状态发生改变，所有的依赖对象（观察者对象）都将得到通知，进行广播通知。
如何解决：使用面向对象技术，可以将这种依赖关系弱化。
关键代码：在抽象类里有一个 ArrayList 存放观察者们。
应用实例：拍卖的时候，拍卖师观察最高标价，然后通知给其他竞价者竞价。

DNS原理及其解析过程
DNS domain name system 主要作用就是将主机域名转换为ip地址

为什么需要DNS解析域名为IP地址？
网络通讯大部分是基于TCP/IP的，而TCP/IP是基于IP地址的，所以计算机在网络上进行通讯时只能识别如“202.96.134.133”之类的IP地址，而不能认识域名。我们无法记住10个以上IP地址的网站，所以我们访问网站时，更多的是在浏览器地址栏中输入域名，就能看到所需要的页面，这是因为有一个叫“DNS服务器”的计算机自动把我们的域名“翻译”成了相应的IP地址，然后调出IP地址所对应的网页。

关于DNS的获取流程：
DNS是应用层协议，事实上他是为其他应用层协议工作的，包括不限于HTTP和SMTP以及FTP，用于将用户提供的主机名解析为ip地址。
具体过程如下：
①用户主机上运行着DNS的客户端，就是我们的PC机或者手机客户端运行着DNS客户端了
②浏览器将接收到的url中抽取出域名字段，就是访问的主机名，比如http://www.baidu.com/, 并将这个主机名传送给DNS应用的客户端
③DNS客户机端向DNS服务器端发送一份查询报文，报文中包含着要访问的主机名字段（中间包括一些列缓存查询以及分布式DNS集群的工作）
④该DNS客户机最终会收到一份回答报文，其中包含有该主机名对应的IP地址
⑤一旦该浏览器收到来自DNS的IP地址，就可以向该IP地址定位的HTTP服务器发起TCP连接

所谓死锁：
是指多个进程在运行过程中因争夺资源而造成的一种僵局，当进程处于这种僵持状态时，若无外力作用，它们都将无法再向前推进。
产生死锁的必要条件：

互斥条件：进程要求对所分配的资源进行排它性控制，即在一段时间内某资源仅为一进程所占用。
请求和保持条件：当进程因请求资源而阻塞时，对已获得的资源保持不放。
不剥夺条件：进程已获得的资源在未使用完之前，不能剥夺，只能在使用完时由自己释放。
环路等待条件：在发生死锁时，必然存在一个进程--资源的环形链。

预防死锁：
资源一次性分配：一次性分配所有资源，这样就不会再有请求了：（破坏请求条件）
只要有一个资源得不到分配，也不给这个进程分配其他的资源：（破坏请保持条件）
可剥夺资源：即当某进程获得了部分资源，但得不到其它资源，则释放已占有的资源（破坏不可剥夺条件）
资源有序分配法：系统给每类资源赋予一个编号，每一个进程按编号递增的顺序请求资源，释放则相反（破坏环路等待条件）

银行家算法：
当一个进程申请使用资源的时候，银行家算法通过先 试探 分配给该进程资源，然后通过安全性算法判断分配后的系统是否处于安全状态，若不安全则试探分配作废，让该进程继续等待。
假设资源P1申请资源，银行家算法先试探的分配给它（当然先要看看当前资源池中的资源数量够不够），若申请的资源数量小于等于Available，然后接着判断分配给P1后剩余的资源，能不能使进程队列的某个进程执行完毕，若没有进程可执行完毕，则系统处于不安全状态（即此时没有一个进程能够完成并释放资源，随时间推移，系统终将处于死锁状态）。
若有进程可执行完毕，则假设回收已分配给它的资源（剩余资源数量增加），把这个进程标记为可完成，并继续判断队列中的其它进程，若所有进程都可执行完毕，则系统处于安全状态，并根据可完成进程的分配顺序生成安全序列（如{P0，P3，P2，P1}表示将申请后的剩余资源Work先分配给P0–>回收（Work+已分配给P0的A0=Work）–>分配给P3–>回收（Work+A3=Work）–>分配给P2–>······满足所有进程）。

系统调用：
这是用户态进程主动要求切换到内核态的一种方式。用户态进程通过系统调用申请使用操作系统提供的服务程序完成工作。例如fork（）就是执行了一个创建新进程的系统调用，还有write、open等，这是直接调用，如果是间接调用的话可以是prift->write。系统调用的机制和新是使用了操作系统为用户特别开放的一个中断来实现，如Linux的int 80h中断。
即：
应用程序→（调用）→API→（存入系统调用号，中断）→中断处理函数【内核态】→（根据系统调用号调用）→系统调用→返回

用户级线程和内核级线程的区别：
用户线程：
指不需要内核支持而在用户程序中实现的线程，其不依赖于操作系统核心，应用进程利用线程库提供创建、同步、调度和管理线程的函数来控制用户线程。
内核线程：
由操作系统内核创建和撤销。内核维护进程及线程的上下文信息以及线程切换。一个内核线程由于I/O操作而阻塞，不会影响其它线程的运行。

以下是用户级线程和内核级线程的区别：
1.内核级线程：
（1）线程的创建、撤销和切换等，都需要内核直接实现，即内核了解每一个作为可调度实体的线程。
（2）这些线程可以在全系统内进行资源的竞争。
（3）内核空间内为每一个内核支持线程设置了一个线程控制块（TCB），内核根据该控制块，感知线程的存在，并进行控制。
2.用户级线程：
（1）用户级线程仅存在于用户空间。
（2）内核并不能看到用户线程。——>重要的区别
（3）内核资源的分配仍然是按照进程进行分配的；各个用户线程只能在进程内进行资源竞争。

内核线程的优点：
（1）当有多个处理机时，一个进程的多个线程可以同时执行。
缺点：
（1）由内核进行调度。

用户级线程的优点：
（1） 线程的调度不需要内核直接参与，控制简单。
（2） 可以在不支持线程的操作系统中实现。
（3） 创建和销毁线程、线程切换代价等线程管理的代价比内核线程少得多。
（4） 允许每个进程定制自己的调度算法，线程管理比较灵活。这就是必须自己写管理程序，与内核线程的区别
（5） 线程能够利用的表空间和堆栈空间比内核级线程多。
（6） 同一进程中只能同时有一个线程在运行，如果有一个线程使用了系统调用而阻塞，那么整个进程都会被挂起。另外，页面失效也会产生同样的问题。
缺点：
（1）资源调度按照进程进行，多个处理机下，同一个进程中的线程只能在同一个处理机下分时复用

Java跟JavaScript两者间的关系和区别：
数据类型不同：
Java的数据类型分为8种，分别是：byte、short、int、long、float、double、char以及Boolean，而JavaScript的数据类型为三种，分别为：number、string和Boolean。
二者定位不同：
Java是一种完全面向对象的编程语言，想要运用Java写东西就必须先设计对象，而JavaScript不一样，它是基于对象的一种脚本语言，它为开发者自带提供了很多内部对象，要更为简易省时。
联编方式不同：
Java采用静态联编，Java的对象引用必须在编译时就进行，编译器需要实现强类型检查，而JavaScript不同，它采用动态联编，它的对象引用可以在运行时检查。
用处不一样：
它们最本质的不同就是用途，Java目前被广泛应用于PC端、手机端、互联网、数据中心等等，而JavaScript则被主要用于嵌入文本到HTML页面，读写HTML元素，控制cookies等。

JVM(Java Virtual Machine，Java虚拟机)
Java程序的跨平台特性主要是指字节码文件可以在任何具有Java虚拟机的计算机或者电子设备上运行，Java虚拟机中的Java解释器负责将字节码文件解释成为特定的机器码进行运行。因此在运行时，Java源程序需要通过编译器编译成为.class文件。众所周知java.exe是java class文件的执行程序，但实际上java.exe程序只是一个执行的外壳，它会装载jvm.dll（windows下），这个动态连接库才是java虚拟机的实际操作处理所在。

数据库索引
作用：
提高查询速度
确保数据的唯一性
可以加速表和表之间的连接，实现表和表之间的参照完整性
使用分组和排序子句进行数据检索时，可以减少分组和排序的时间
全文检索字段进行搜素优化

分类:
主键索引（PRIMAY KEY）：一般是在建表的时候同时创建主键索引
唯一索引（UNIQUE）：CREATE UNIQUE INDEX indexName ON mytable(username(length)) 
常规索引（INDEX）：CREATE INDEX indexName ON mytable(username(length))
全文索引（FULLTEXT）

什么时候不创建索引：
第一，对于那些在查询中很少使用或者参考的列不应该创建索引。
第二，对于那些只有很少数据值的列也不应该增加索引（如性别）。
第三，对于那些定义为text, image和bit数据类型的列不应该增加索引。
第四，当修改性能远远大于检索性能时，不应该创建索引。

JS继承的六种方式：
https://www.cnblogs.com/Grace-zyy/p/8206002.html
父类：
function Person(name){
    this.name=name;
    this.sum=function(){
        alert(this.name)
    }
}
Person.prototype.age=10;

1.原型链继承
function Per(){
    this.name="KER";
}
Per.prototype=new Person();
var per1=new Per();
console.log(per1.age);//10

2.借用构造函数继承
function Con(){
    Person.call(this,"jer");
    this.age=12;
}
var con1 = newCon();
console.log(con1.name);//"jer"
console.log(con1.age);//12

3.组合继承（原型链+借用）【常用】
function SubType(name){
   Person.call(this.name);
}
SubType.prototype=new Person();
var sub=new SubType("gar");
console.log(con1.name);//"gar"
console.log(con1.age);//10

4.原型式继承
function content(obj){
    function F(){}
    F.prototype=obj;
    return new F();
}
var sup=new Person();
var sup1=content(sup);
console.log(sup1.age);//10

5.寄生式继承

6.寄生组合式继承【常用】

CORS:
CORS（跨站点资源分享）通俗的讲是跨域问题，严格来说它是跨域问题的解决方案之一，而且是官方解决方案。
CORS是一种可以让你实现跨站点请求并同时阻止恶意js的请求，它会在你发送下面几种HTTP请求时触发：
- 不同的域名 （比如在网站 example.com 请求 api.com)
- 不同的子域名 （比如在网站 example.com 请求 api.example.com)
- 不同的端口 （比如在网站 example.com 请求 example.com:3001)
- 不同协议 （比如在网站 https://example.com 请求 http://example.com)

如何修复CORS“错误”？
你应该明白了CORS的行为并不是一个错误——它是一个机制，用来保护你的用户，你和你请求的服务器。有时，缺乏适当的头部信息是因为客户端实现错误（比如：丢失验证信息比如API key）。下面有几个适应不同情况，“修复这个错误”的方法：A——我在开发前端并且可以控制或者认识开发后端的人员这是一个最好的情况——你应该能让返回信息的头里包含适当的CORS字段。如果你请求的API使用node的experss，你可以使用cors包。如果你想让你的网站更加的安全，你应该使用白名单来返回Access-Control-Allow-Origin头。B——我在开发前端，但是我不能控制后端，我需要一个临时方案这是第二个最好的情况，特别是在有时间限制的情况里。临时的解决这个问题可以让你的浏览器忽略CORS机制——比如安装ACAOChrmoe插件或者启动Chrome时输入下面的指令:chrome --disable-web-security --user-data-dir重要:需要记住的是，这个方法会关闭整个浏览器的CORS机制，包含你浏览器正在访问的网站，要小心使用，非常不安全。（译者注：这个方法没有用过，个人觉得风险太大，临时测试也慎用，怕你开了插件忘记关掉）其他方法可以使用devServer.proxy(假设你使用webpack来启动你的app)或者使用CORS-as-a-service解决方案，比如https://cors-anywhere.herokuapp.com/C——我在开发前端，但是我控制不了后端，而且将来也控制不了好的。事情越来越复杂了。首先，你应该思考，为什么服务器没有返回适当的头部。也许你请求的API不许允第三方应用请求它们？或者这些API仅仅给APP使用，而不是浏览器？或者你应该发送一个验证token在你请求的URL里？假如你坚持要通过浏览器获得它们的数据，你应该自己写一个代理，在浏览器和你要请求的API之间。就像我们在方法B里做的那样。


