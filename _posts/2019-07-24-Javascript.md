---
javascript!

---



# Javascript目录

1.工作原理

2.基本语法

3.变量的使用

4.运算符

5.流程控制

6.函数应用

7.js 对象

8.js常用的

9.js的事件处理

10.DOM中内及属性

11.html将html元素转为js

12.通过自己定义的方式

13.Dom节点的创建

14.JS的bom

15.bom的重点对象

16.位置和事件对象

17.应用event应用

18.js表单

19.表单注册

20.js开发

21.Ajax在开发中的应用

22.js的Dom

23.Dom的节点操作

24js 常见开发





# 1.概念

变量和常量的知识，基本数据类型，运算符，基本数据类型间的转换，流程控制语句

```
js一种直译型脚本语言，一种动态语言、弱类型语言、支持内置类型。它的解释器被称为javascript引擎。它浏览器的一部分。用于客户端的脚本语言，最早是html网页上使用用来给HTML增加动态效果。                                                                      没有任何关系

为了取得发展以及技术上的优势  微软曾推出过Jscript，跟javascript一样可以在浏览器上运行。为了统一规格，javascript兼容于ECMA标准，因此它也称为ECMAScript

ECMA欧洲计算机联合商协会
```

### js用途 

```
1、嵌入文本到我们的HTML页面上
2、对浏览器事件作出响应
3、读写HTML
4、在数据提交到服务器之前先做数据验证
5、检测访客的浏览信息
6、控制cookie
7、基于nodeJs技术进行服务端的编程
```

​	



### js组成部分

1、ECMAScript规定核心的语法
2、DOM（document object model）:文档对象模型
3、BOM（browser object model）：浏览器对象模型

### 二、javascrip的语法

js可以有几种写法：

​	
​	1、写在script标签内
​	2、写在外部js文件里面
​	3、写在标签内部的

​	

### 三、标识符和关键字

### 1、什么是标识符：

```
标识符
- - 在JS中所有的可以由我们自主命名的都可以称为是标识符
- - 例如：变量名、函数名、属性名都属于标识符

命名一个标识符时需要遵守如下的规则：
- 1.标识符中可以含有字母 、数字 、下划线_ 、$符号
- 2.标识符不能以数字开头
- 3.标识符不能是javascript中的关键字或保留字
- 4.标识符一般都采用驼峰命名法
- - 首字母小写，每个单词的开头字母大写，其余字母小写
- helloWorld  xxxYyyZzz
- 
- - JS底层保存标识符时实际上是采用的Unicode编码，
- 所以理论上讲，所有的utf-8中含有的内容都可以作为标识符
```

###    2、常用的标识符格式：

```
	i j
xxx_zzz
_xxxx
	$xxx
	a1
	aaaBbbCcc
	AaaBbbCcc
	！！！！注意一点：标识符不要跟关键字同名，数字不允许作为首字母出现，这样我们js比较容易的区分开标识符和数字
```

### 3、关键字：

关键字是指我js语言中有特定含义，称为js语法中一部分的 那些单词
var let const for if foreach break continue do while switch....

### 4、保留字：

未来某个js版本会称为关键字的单词，一样是不可以当成变量名或者方法名来使用      

### 5、注释：

//:单行注释
/**/：多行注释


​	

### 6.JavaScript 显示数据

JavaScript 可以通过不同的方式来输出数据：

- 使用 **window.alert()** 弹出警告框。
- 使用  **document.write()** 方法将内容写到 HTML 文档中。
- 使用 **innerHTML** 写入到 HTML 元素。
- 使用 **console.log()** 写入到浏览器的控制台。



```javascript
<script>
window.alert(5 + 6);
</script>

//段落更改
<p id="demo">我的第一个段落。</p>
<script>
document.getElementById("demo").innerHTML = "段落已修改。";
</script>


//Sun Jul 28 2019 10:00:31 GMT+0800 (中国标准时间)
<button onclick="myFunction()">点我</button>
<script>
document.write(Date());
</script>

<script>
a = 5;
b = 6;
c = a + b;
console.log(c);
</script>
```



# 2.基本语法

------

JavaScript 是一个程序语言。语法规则定义了语言结构。

------

### JavaScript 语法

JavaScript 是一个脚本语言。

它是一个轻量级，但功能强大的编程语言。

------

### JavaScript 字面量

在编程语言中，一般固定值称为字面量，如 3.14。

**数字（Number）字面量** 可以是整数或者是小数，或者是科学计数(e)。

```
3.14

1001

123e5
```

**字符串（String）字面量** 可以使用单引号或双引号:

```
"John Doe"

'John Doe'
表达式字面（！）量 用于计算：

5 + 6

5 * 10


**数组（Array）字面量** 定义一个数组：

[40, 100, 1, 5, 25, 10]

**对象（Object）字面量** 定义一个对象：

{firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"}

**函数（Function）字面量** 定义一个函数：

function myFunction(a, b) { return a * b;}

```



------

### JavaScript 变量

在编程语言中，变量用于存储数据值。

JavaScript 使用关键字 **var** 来定义变量， 使用等号来为变量赋值：

```javascript
var x, length
x = 5
length = 6
------------------
<!DOCTYPE html>
<html>
<head> 
<meta charset="utf-8"> 
<title>菜鸟教程(runoob.com)</title> 
</head>
<body>

<p id="demo"></p>
<script>
var length;
length = 6;
document.getElementById("demo").innerHTML = length;
</script>

</body>
</html>

//输出：6
```

变量可以通过变量名访问。在指令式语言中，变量通常是可变的。字面量是一个恒定的值。 

变量是一个**名称**。字面量是一个**值**。



### JavaScript 操作符

| 类型                   | 实例          | 描述                   |
| :--------------------- | :------------ | :--------------------- |
| 赋值，算术和位运算符   | =  +  -  *  / | 在 JS 运算符中描述     |
| 条件，比较及逻辑运算符 | ==  != <  >   | 在 JS 比较运算符中描述 |

------

### JavaScript 语句

在 HTML 中，JavaScript 语句向浏览器发出的命令。

语句是用分号分隔：

```
var x = 5 + 6;
var y = x * 10;
```

### JavaScript 关键字

JavaScript 关键字用于标识要执行的操作。

和其他任何编程语言一样，JavaScript 保留了一些关键字为自己所用。

var 关键字告诉浏览器创建一个新的变量：

```
var x = 5 + 6;
var y = x * 10;
```

JavaScript 同样保留了一些关键字，这些关键字在当前的语言版本中并没有使用，但在以后 JavaScript 扩展中会用到。

```
以下是 JavaScript 中最重要的保留字（按字母顺序）：

abstract	else	instanceof	super
boolean	enum	int	switch
break	export	interface	synchronized
byte	extends	let	this
case	false	long	throw
catch	final	native	throws
char	finally	new	transient
class	float	null	true
const	for	package	try
continue	function	private	typeof
debugger	goto	protected	var
default	if	public	void
delete	implements	return	volatile
do	import	short	while
double	in	static	with
```



### JavaScript 注释

不是所有的 JavaScript 语句都是"命令"。双斜杠 **//** 后的内容将会被浏览器忽略：



### JavaScript 函数

JavaScript 语句可以写在函数内，函数可以重复引用：

```
引用一个函数 = 调用函数(执行函数内的语句)。

function myFunction(a, b) {
   	return a * b;                                // 返回 a 乘以 b 的结果
}


```







# 数据类型(work)

> 基本数据类型
>
> - 字符串 string
> - 数值型 int float (近似数) 
> - 布尔型（boolean）Fales  True =逻辑运算符（&& || ！多个条件链接起来）
>
> 复合数据类型
>
> - 对象
> - 数组
>
> 其他数据类型
>
> - 函数
> - null 为假
> - Undefined 未定义的  返回NaN =1/0。infinity无穷大；空字符串；为假
>
> 数据类型的转换
>
> - 隐式数据类型
> - 显式数据类型



数据类型 就是我可以了解到的是描述数据的类型

js基本的数据类型 ：数字类型，字符串型，布尔型，undefined，null
对象类型 数组 

### JS保存数据类型(work)

包括number、string、boolean、undefined、object、function。

### 1.typeof类型的

typeof 是一个一元运算，放在一个运算数之前，运算数可以是原始数据类型，也可以是引用复杂类型。

它返回值是一个用来表示表达式的数据类型的字符串。

```javascript
typeof 的格式
typeof   expression ;
expression 参数是需要查找类型信息的任意表达式。

 typeof一般测试基本类型（Undefined、Boolean、null、Number、String)，
 对引用类型返回object（Function引用类型返回Function）
 
 	//原始数据类型(string,number,boolean,undefined)
	//原始数据值是一种没有额外属性和方法的单一简单数据值。
	var a="abc";
	var b=10;
	var c=true;
	var d;
	var e=null;
	alert("a 	"+typeof a);//string
	alert("b 	"+typeof b);//number
	alert("c 	"+typeof c);//boolean
	alert("d 	"+typeof d);//undefined
	alert("e 	"+typeof e);//object

	//复杂类型（object，function）
	var obj1=new Array();
	var obj2=new Date(); 
 	var obj3=new Number();
	var obj4=new String(); 
	var obj5=new Function();
	var obj6=new Boolean();
	alert("obj1  "+typeof(obj1));//object
	alert("obj2  "+typeof(obj2));//object
	alert("obj3  "+typeof(obj3));//object
	alert("obj4  "+typeof(obj4));//object
	alert("obj5  "+typeof(obj5));//function
	alert("obj6  "+typeof(obj6));//object
```

### 2.instanceof运算符

因为typeof遇到null,数组,对象时都会返回object类型，所以当我们要判断

一个对象具体是否为一个数组时或者判断某个变量是否为某个对象的实例,

则要选择使用另一个语法instanceof，instanceof返回的是一个布尔值。

```javascript
instanceof的格式
expression instanceof class 表达式运算符类
expression  必选项。任意对象表达式。
class　　必选项。任意已定义的对象类。

//instanceof 运算符与 typeof 运算符相似，用于识别正在处理的对象的类型。
//与 typeof 方法不同的是，instanceof 方法要求开发者明确地确认对象为某特定类型。
var a = {};
alert(a instanceof Object);  //true
var b = [];
alert(b instanceof Array);  //true

//需要注意的是，instanceof只能用来判断对象和函数，不能用来判断字符串和数字等，如：
var b = '123';
alert(b instanceof String);  //false
alert(typeof b);  //string

var c = new String("123");
alert(c instanceof String);  //true
alert(typeof c);  //object

//另外，用instanceof可以判断变量是否为数组：
var arr = [1,2,3]; 
alert(arr instanceof Array);   // true
```







### 1、数字类型（Number）

只有一种数字类型，数字 可以是小数 ，也可以的整数
以0开头 默认使用8进制来表示我的这个数字
以0x开头 默认使用16进制来表述我的这个数字
如果以-开头 默认以负数
如果我带有e：以科学计数法来解析我的这个数字

​	

### 2、字符串型（string）

字符串是存储字符的变量，用来表示文本的数据类型，程序中的字符串是包含单引号/双引号的，由单引号来界定我双引号中包含的字符串 反过来
es6模板字符串("`")

### 3、布尔类型（boolean）

一般是用在流程控制语句中，字符串和数字类型都是无穷多个，然而我们的布尔数据类型只有两个：true 和 false
这两个个值一般用于说明某个事物是真或者假
js一般用布尔类型来比较所得到的结果

### 4、null（空）

null
关键字null是一个特殊的值，它表示变量为空值，用来定义空的或者是不存在的引用。
如果试图去引用一个没有定义的值，就会返回一个null。
这里注意一点：null并不等于"" 或者0

### 5、undefined（未定义）

这个值表示变量不含有值，没有定义的值，或者被定义了一个不存在的属性值

​	

### ！null和undefined区别：

null它表示一个变量被赋予一个空值，而undefined是表示变量还没有被赋值

### 五、运算符

用于执行程序代码运算，会针对一个以上操作数来进行

```
1、算术运算符
+   -   *   /   %  ++  --
字符串拼接使用“+”

2、比较运算符

<
>
==
！=
<=
>=
=== 全等于：将数值以及数据类型一并比较
！==不全等于：将数值以及数据类型一并比较

3、赋值运算符
=
+= 

-=
*=
/=
%=
a=a+2;==>a+=2
a=a-2;==>a-=2
a=a*2;==>a*=2
a=a/2;==>a/=2
a=a%2;==>a%=2	

4、逻辑运算符
 &&  全真为真
||  一个为真就是真

！  取反

逻辑短路

5、三元运算符（三目运算符）
表达式1?表达式2:表达式3

当我的表达式1成立时  执行表达式2  否则执行表达式3
```

​	



​	

### 六、数据类型间转换

### 1、显示数据类型转换

​	1.1转数字类型：

### 1.Number()：

可以将任意类型的参数转换为数字类型，遵循以下规则：
​	1、如果它是一个布尔值true和false将被分别转成1和0；
​	2、如果它是以个数字，返回它本身
​	3、如果是null，返回0；
​	4、如果是undefined，返回NaN
​	5、如果是一个字符串：
​		1）如果这个字符串只包含数字，则直接将它转成10进制数字（忽略前面的0）
​		2）如果有有效浮点格式，将它转成一个浮点数值
​		3）如果是空字符串,转换为0
​		4）如果以上都不符合==>NaN

### 2.parseInt(string,num):

可以解析一个字符串，返回一个整数

1）忽略字符串前面所有的空格，直到找到第一个非空字符为止
2）如果第一个字符不是数字或者“-” 直接返回NaN
3）如果第一个字符是数字，它解析到遇到的第一个不是数字的字符为止



4）如果上面解析完结果是以0开头，就将它当成一个八进制来解析
		5）如果以0x开头，则当成十六进制来解析。
		6）如果我指定了num参数，那么 它就以num进制来解析

### 3.转字符串类型：

​		1.String():将任意的一个类型的值转换为字符串，遵循一下下规则：
​		1）如果是null，==>"null"
​		2)如果是undefined ==>"undefined"

toFied(num):可以把Number类型四舍五入为指定小数位的字符串。
		返回的字符串，num保留小数位
	
Boolean():如果这个值是空字符串（""）、数字零（0）、undefined或者null 会返回false，否则返回true
!空格并不是空字符串
		

# 隐式数据转换（work）

js的数据类型非常弱的，在使用算术运算符的时候,运算符两边的数据类型可以是任意的  这是因为js的引擎它在代码运行之前偷偷把数据类型进行转换 ，这种转换我们称之为隐式转换
	

小类型向大类型转换

### 一、自动类型转换也叫“隐式类型转换”。



```
小类型向大类型的转换会自动完成，不需要程序员编写额外的代码，由jvm负责。

自动类型转换的规则：符号位会自动扩展，负数补1，正数补0

自动类型转换包含以下情况：
  
  1.byte->short->int->   long->double->

	2.int和char类型的数据在某些情况下可以自动相互转换。
	
	### 二、

int类型为32位，最高位为符号位，其余31位为尾数。

long类型为64位，最高位为符号位，其余63位为尾数。

 ps：尾数：精度值，用来存放数据。

int类型转换成long类型后，因为是负数，所以符号位补了32位1。

 小类型向大类型转型一般情况下是安全的。----------

当小类型的精度高于大类型时要注意精度丢失的隐患。

### 三、

int类型为32位，最高位为符号位，其余31位为尾数，float类型为也是32位，但是尾数是23位。

int类型存放了一个28位的数，而flaot类型只能承载23位，转换后精度丢失最后一位的数据。

当小类型的精度（尾数）高于大类型时，要注意精度丢失问题。
```



​         

#### 小练习：

```javascript
  <script type="text/javascript">
   
    var a='7'
    var b=3
    var c = 2
    alert(a+b)
    console.log(a-b-c)   //2
    console.log(a+b+c)	//732
    console.log(b+c+a)	//57
  </script>
```





### 流程控制语句:

```

if语句
if(条件){
	函数体
}
------------
if else语句
if(条件){
	函数体1
}else{
	函数体2
}
--------------
if.....else if......else语句
if(条件1){
	
}else if(条件2){
	
}else if(条件n){
	
}else{
	
}

------------
switch语句:多分支语句

switch(变量){
	case a:
	.....
	break;
	case b:
	.....
	break;
	case c:
	...
	break;
	........
	default:
		....
		break;
}
```

​	

### 循环结构：

>1、while循环：先判断条件 当条件成立 再执行
>while(循环成立条件){
>	....
>}
>
>2do...while循环:不论条件成不成立 先执行一遍 再判断
>do{
>	.....
>}while(循环成立条件)
>
>3、for循环
>4、for in循环
>
>continue：
>跳过当前循环，直接进入循环的下一个步骤
>
>break:
>结束循环





# 3.JavaScript 函数

------

函数是由事件驱动的或者当它被调用时执行的可重复使用的代码块。

```javascript 
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>测试实例</title>
<script>
function myFunction()
{
    alert("Hello World!");
}
</script>
</head>
 
<body>
<button onclick="myFunction()">点我</button>
</body>
</html>

结果： 出现一个。点我
输出hello world
```



------

## JavaScript 函数语法

函数就是包裹在花括号中的代码块，前面使用了关键词 function：

```
function *functionname*()
{
    *// 执行代码*
}
```

当调用该函数时，会执行函数内的代码。

可以在某事件发生时直接调用函数（比如当用户点击按钮时），并且可由 JavaScript 在任何位置进行调用。

JavaScript 对大小写敏感。关键词 function 必须是小写的，并且必须以与函数名称相同的大小写来调用函数。

## 调用带参数的函数

在调用函数时，您可以向其传递值，这些值被称为参数。

这些参数可以在函数中使用。

```
您可以发送任意多的参数，由逗号 (,) 分隔：

myFunction(*argument1,argument2*)

当您声明函数时，请把参数作为变量来声明： 

function myFunction(*var1*,*var2*)
{
*代码*
}

```

变量和参数必须以一致的顺序出现。第一个变量就是第一个被传递的参数的给定的值，以此类推。

### 实例

```javascript
<p>点击这个按钮，来调用带参数的函数。</p>
<button onclick="myFunction('Harry Potter','Wizard')">点击这里</button>
<script>
function myFunction(name,job){
    alert("Welcome " + name + ", the " + job);
}
</script>
--------------------------
<!DOCTYPE html>
<html>	
<head> 
<meta charset="utf-8"> 
<title>菜鸟教程(runoob.com)</title> 
</head>
<body>
		//这儿--
</body>
</html>

结果：
点击这个按钮，来调用带参数的函数。  --》 点击这里
Welcome Harry Potter, the Wizard
```

### 带有返回值的函数

有时，我们会希望函数将值返回调用它的地方。

通过使用 return 语句就可以实现。

在使用 return 语句时，函数会停止执行，并返回指定的值。

### 语法

```javascript
function myFunction()
{
    var x=5;
    return x;
}

上面的函数会返回值 5。

注意整个 JavaScript 并不会停止执行，仅仅是函数。JavaScript 将继续执行代码，从调用函数的地方。
函数调用将被返回值取代：
var myVar=myFunction();

myVar 变量的值是 5，也就是函数 "myFunction()" 所返回的值。
即使不把它保存为变量，您也可以使用返回值：

document.getElementById("demo").innerHTML=myFunction();
"demo" 元素的 innerHTML 将成为 5，也就是函数 "myFunction()" 所返回的值。
```

您可以使返回值基于传递到函数中的参数：

# 实例  = 调用函数 

```javascript
计算两个数字的乘积，并返回结果：

function myFunction(a,b)
{
    return a*b;
}
 
document.getElementById("demo").innerHTML=myFunction(4,3);
"demo" 元素的 innerHTML 将是：
12
```



在您仅仅希望退出函数时 ，也可使用 return 语句。返回值是可选的：

```javascript
function myFunction(a,b)
{
    if (a>b)
    {
        return;
    }
    x=a+b
}

function myFunction(a,b) {if (a>b) {  return;  }   x=a+b }

```

如果 a 大于 b，则上面的代码将退出函数，并不会计算 a 和 b 的总和。

------

## 局部 JavaScript 变量

在 JavaScript 函数内部声明的变量（使用 var）是*局部*变量，所以只能在函数内部访问它。（该变量的作用域是局部的）。

您可以在不同的函数中使用名称相同的局部变量，因为只有声明过该变量的函数才能识别出该变量。

只要函数运行完毕，本地变量就会被删除。

------

## 全局 JavaScript 变量

在函数外声明的变量是*全局*变量，网页上的所有脚本和函数都能访问它。

------

## JavaScript 变量的生存期

JavaScript 变量的生命期从它们被声明的时间开始。

局部变量会在函数运行以后被删除。

全局变量会在页面关闭后被删除。

------

## 向未声明的 JavaScript 变量分配值

如果您把值赋给尚未声明的变量，该变量将被自动作为 window 的一个属性。

这条语句：

carname="Volvo";

将声明 window 的一个属性 carname。

非严格模式下给未声明变量赋值创建的全局变量，是全局对象的可配置属性，可以删除。

```javascript
var var1 = 1; // 不可配置全局属性
var2 = 2; // 没有使用 var 声明，可配置全局属性

console.log(this.var1); // 1
console.log(window.var1); // 1

delete var1; // false 无法删除
console.log(var1); //1

delete var2; 
console.log(delete var2); // true
console.log(var2); // 已经删除 报错变量未定义
```





# 函数 - 闭包

------

JavaScript 变量可以是局部变量或全局变量。

私有变量可以用到闭包。

------

## 全局变量

函数可以访问由函数内部定义的变量，如：

### 实例

```
function myFunction() {     var a = 4;     return a * a; }

function myFunction() {
    var a = 4;
    return a * a;
}
```

函数也可以访问函数外部定义的变量

```javascript
var a = 4;
function myFunction() {
    return a * a;
}
//----------------------
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>菜鸟教程(runoob.com)</title>
</head>
<body>

<p>函数可以访问定义在函数外的变量：</p>
<button type="button" onclick="myFunction()">点我</button>
<p id="demo"></p>
<script>
var a = 4;
function myFunction() {
	document.getElementById("demo").innerHTML = a * a;
} 
</script>

</body>
</html>
```

后面一个实例中， **a** 是一个 **全局** 变量。 

在web页面中全局变量属于 window 对象。

全局变量可应用于页面上的所有脚本。

在第一个实例中， **a** 是一个 **局部** 变量。

局部变量只能用于定义它函数内部。对于其他的函数或脚本代码是不可用的。

全局和局部变量即便名称相同，它们也是两个不同的变量。修改其中一个，不会影响另一个的值。 

**注意**： 变量声明时如果不使用 **var** 关键字，那么它就是一个全局变量，即便它在函数内定义。

### 变量生命周期

全局变量的作用域是全局性的，即在整个JavaScript程序中，全局变量处处都在。

而在函数内部声明的变量，只在函数内部起作用。这些变量是局部变量，作用域是局部性的；函数的参数也是局部性的，只在函数内部起作用。

------

### 计数器困境

设想下如果你想统计一些数值，且该计数器在所有函数中都是可用的。

你可以使用全局变量，函数设置计数器递增：

### 实例

```
var counter = 0;   function add() {    return counter += 1; }  
add(); add(); add();   
// 计数器现在为 3
```

计数器数值在执行 add() 函数时发生变化。

但问题来了，页面上的任何脚本都能改变计数器，即便没有调用 add() 函数。

如果我在函数内声明计数器，如果没有调用函数将无法修改计数器的值：

### 对比实例

```
function add() {     var counter = 0;     return counter += 1; }  
add(); add(); add();   
// 本意是想输出 3, 但事与愿违，输出的都是 1 !
```

以上代码将无法正确输出，每次我调用 add() 函数，计数器都会设置为 1。

**JavaScript 内嵌函数可以解决该问题。**

------

#### JavaScript 内嵌函数

所有函数都能访问全局变量。   

实际上，在 JavaScript 中，所有函数都能访问它们上一层的作用域。

JavaScript 支持嵌套函数。嵌套函数可以访问上一层的函数变量。 

该实例中，内嵌函数 **plus()** 可以访问父函数的 **counter** 变量：

#### 实例

```
function add() {
    var counter = 0;
    function plus() {counter += 1;}
    plus();    
    return counter; 
}
```

如果我们能在外部访问  **plus()** 函数，这样就能解决计数器的困境。

我们同样需要确保 **counter = 0** 只执行一次。

**我们需要闭包。**

------

## JavaScript 闭包(自我调用)

还记得函数自我调用吗？该函数会做什么？

#### 实例

```
var add = (function () {
    var counter = 0;
    return function () {return counter += 1;}
})();
 
add();
add();
add();
 
// 计数器为 3
```

#### 实例解析

```javascript
变量 add 指定了函数自我调用的返回字值。 
自我调用函数只执行一次。设置计数器为 0。并返回函数表达式。
add变量可以作为一个函数使用。非常棒的部分是它可以访问函数上一层作用域的计数器。 
这个叫作 JavaScript **闭包。**它使得函数拥有私有变量变成可能。
计数器受匿名函数的作用域保护，只能通过 add 方法修改。

//闭包是一种保护私有变量的机制，在函数执行时形成私有的作用域，保护里面的私有变量不受外界干扰。
//直观的说就是形成一个不销毁的栈环境。
```







#  正则表达式

正则表达式是构成搜索模式的字符序列。

该搜索模式可用于文本搜索和文本替换操作。

正则表达式（英语：Regular Expression，在代码中常简写为regex、regexp或RE）使用单个字符串来描述、匹配一系列符合某个句法规则的字符串搜索模式。

搜索模式可用于文本搜索和文本替换。



#### 正则表达式通常用于两个字符串方法 : search() 和 replace()。

**search() 方法** 用于检索字符串中指定的子字符串，或检索与正则表达式相匹配的子字符串，并返回子串的起始位置。

**replace() 方法** 用于在字符串中用一些字符替换另一些字符，或替换一个与正则表达式匹配的子串。

## 什么是正则表达式？

正则表达式是构成*搜索模式（search pattern）*的字符序列。

正则表达式可以是单字符，或者更复杂的模式；可用于执行所有类型的*文本搜索*和*文本替换*操作。

#### 语法

```
/pattern/modifiers;
```

#### 实例

```
var patt = /w3school/i;

### 例子解释：

/w3school/i 是一个正则表达式。

w3school 是模式（pattern）（在搜索中使用）。

i 是修饰符（把搜索修改为大小写不敏感）。
```



#### 使用字符串方法

search() 方法使用表达式来搜索匹配，然后返回匹配的位置。

replace() 方法返回模式被替换处修改后的字符串。

#### 使用字符串方法 search() 来处理字符串

search() 方法也接受字符串作为搜索参数。字符串参数将被转换为正则表达式：

```
### 实例

使用字符串来执行对 "W3school" 的搜索：

var str = "Visit W3School!";
var n = str.search("W3School"); 
```

#### 在字符串方法 search() 中使用正则表达式

使用正则表达式执行搜索字符串中 "w3school" 的大小写不敏感的搜索：

```
var str = "Visit W3School";
var n = str.search(/w3school/i); 

n 中的结果将是：6
```

#### 使用字符串方法 replace() 处理字符串

replace() 也接受字符串作为搜索参数：

```
var str = "Visit Microsoft!";
var res = str.replace("Microsoft", "W3School"); 

## 在字符串方法 replace() 中使用正则表达式

使用大小写不明的正则表达式以 W3school 来替换字符串中的 Microsoft：

var str = "Visit Microsoft!";
var res = str.replace(/microsoft/i, "W3School"); 


res 的结果将是：Visit W3School!
```



#### 正则表达式修饰符

*修饰符*可用于大小写不敏感的更全局的搜素：

| 修饰符 | 描述                                                     |      |
| :----- | :------------------------------------------------------- | ---- |
| i      | 执行对大小写不敏感的匹配。                               |      |
| g      | 执行全局匹配（查找所有匹配而非在找到第一个匹配后停止）。 |      |
| m      | 执行多行匹配。                                           |      |

#### 正则表达式模式

*括号*用于查找一定范围的字符串：

| 表达式 | 描述                       |      |
| :----- | :------------------------- | ---- |
| [abc]  | 查找方括号之间的任何字符。 |      |
| [0-9]  | 查找任何从 0 至 9 的数字。 |      |
| (x\|y) | 查找由 \| 分隔的任何选项。 |      |

*元字符（Metacharacter）*是拥有特殊含义的字符：

| 元字符 | 描述                                        |      |
| :----- | :------------------------------------------ | ---- |
| \d     | 查找数字。                                  |      |
| \s     | 查找空白字符。                              |      |
| \b     | 匹配单词边界。                              |      |
| \uxxxx | 查找以十六进制数 xxxx 规定的 Unicode 字符。 |      |

*Quantifiers* 定义量词：

| 量词 | 描述                                |      |
| :--- | :---------------------------------- | ---- |
| n+   | 匹配任何包含至少一个 n 的字符串。   |      |
| n*   | 匹配任何包含零个或多个 n 的字符串。 |      |
| n?   | 匹配任何包含零个或一个 n 的字符串。 |      |

#### 使用 RegExp 对象

在 JavaScript 中，RegExp 对象是带有预定义属性和方法的正则表达式对象。

#### 使用 test()

test() 是一个正则表达式方法。

它通过模式来搜索字符串，然后根据结果返回 true 或 false。

下面的例子搜索字符串中的字符 "e"：

#### 实例

```
var patt = /e/;
patt.test("The best things in life are free!"); 

由于字符串中有一个 "e"，以上代码的输出将是：true


您不必首先把正则表达式放入变量中。上面的两行可缩短为一行：
/e/.test("The best things in life are free!");

```

## 使用 exec()

exec() 方法是一个正则表达式方法。

它通过指定的模式（pattern）搜索字符串，并返回已找到的文本。

如果未找到匹配，则返回 null

```
下面的例子搜索字符串中的字符 "e"：

### 实例


/e/.exec("The best things in life are free!");
由于字符串中有一个 "e"，以上代码的输出将是：e



```



# 作用域

------

作用域是可访问变量的集合。

------

## JavaScript 作用域

在 JavaScript 中, 对象和函数同样也是变量。

**在 JavaScript 中, 作用域为可访问变量，对象，函数的集合。**

JavaScript 函数作用域: 作用域在函数内修改。

------

## 1.JavaScript 局部作用域

变量在函数内声明，变量为局部作用域。

局部变量：只能在函数内部访问。

#### 实例

```javascript
// 此处不能调用 carName 变量
function myFunction() {
    var carName = "Volvo";
    // 函数内可调用 carName 变量
}



<!DOCTYPE html>
<html>
<head> 
<meta charset="utf-8"> 
<title>菜(runoob.com)</title> 
</head>
<body>

<p>局部变量在声明的函数外不可以访问。</p>
<p id="demo"></p>
<script>
myFunction();
document.getElementById("demo").innerHTML = "carName 的类型是：" +  typeof carName;

function myFunction() 
{
    var carName = "Volvo";
}
</script>

</body>
</html>

//jieguo:
//局部变量在声明的函数外不可以访问。
//carName 的类型是：undefined
```

因为局部变量只作用于函数内，所以不同的函数可以使用相同名称的变量。

局部变量在函数开始执行时创建，函数执行完后局部变量会自动销毁。

------

## 2.JavaScript 全局变量

变量在函数外定义，即为全局变量。

全局变量有 **全局作用域**: 网页中所有脚本和函数均可使用。 

#### 实例

```
var carName = " Volvo";
 
// 此处可调用 carName 变量
function myFunction() {
    // 函数内可调用 carName 变量
}
```



如果变量在函数内没有声明（没有使用 var 关键字），该变量为全局变量。

以下实例中 carName 在函数内，但是为全局变量。

#### 实例

````
// 此处可调用 carName 变量
 
function myFunction() {
    carName = "Volvo";
    // 此处可调用 carName 变量
}
````



------

## 3.JavaScript 变量生命周期

JavaScript 变量生命周期在它声明时初始化。

局部变量在函数执行完毕后销毁。

全局变量在页面关闭后销毁。

------

#### 函数参数

函数参数只在函数内起作用，是局部变量。

------

#### HTML 中的全局变量

在 HTML 中, 全局变量是 window 对象: 所有数据变量都属于 window 对象。

#### 实例

```
//此处可使用 window.carName
 
function myFunction() {
    carName = "Volvo";
}
```





# 4.html DOM

属性、文本操作，css操作，对象与数组，面向对象编程

```
ECMAScript规定核心的语法:bom dom
BOM（browser object model）：浏览器对象模型
```

## 2.DOM总结

#### 1. DOM基本介绍

DOM 是 Document Object Model 文档对象模型

- HTML DOM
- XML DOM

#### 2. HTML DOM 对象参考

- 2.1 document 对象

- 属性 ….

- 方法 见手册

- 2.2 form 对象

- 2.3 image 对象

- 2.4 anchor 对象

- 2.5 base 对象

- 2.6 canvas 对象

- 2.7 Event 对象

- 2.8 input 系列对象

- 2.9 select 对象

- 2.10 option 对象

- 2.11 style 对象

- 2.12 table 对象

- 2.13 tableRow 对象

- 2.14 tableCell 对象 ~~~


- 3. XML DOM 对象

------

### 节点操作 (XML DOM)

#### XML DOM 节点

#### 1.节点介绍

- 1.1 什么是节点 node HTML文档中 所有的组成部分 都称之为节点
  - document 文档
  - element 元素
  - attr 属性
  - text 文本
  - comment 注释
- 1.2 节点树 子节点 父节点 同辈节点 后代节点 先辈节点
- 1.3 节点的访问
  - 得到节点
    - document 直接 document
    - element getId/getTagName..
    - attr element.getAttributeNode(‘attrname’)
    - text 子节点
    - comment 子节点
  - 获取子节点 childNodes
  - 获取子元素节点 children
  - 获取第一个子节点 firstChild
  - 获取最后一个子节点 lastChild
  - 获取父节点 parentNode
  - 获取父元素节点 parentElement
  - 获取前一个节点 previousSibling
  - 获取后一个节点 nextSibling
- 1.4 节点属性 nodeName documnet: #document element: 标签名 attr: 属性名 text: #text comment: #comment nodeValue document: null element: null attr: 属性值 text: 文本内容 注释: 注释内容 nodeType document: 9 element: 1 attr: 2 text: 3 commnet: 8

#### 2.节点操作

2.1 获取节点 element: ID/TAGNAME/子节点/父节点/同辈 attr: element.getAttributeNode() 属性节点 element.getAttribute() 属性值 element.attr 属性值

2.2 改变节点(改变节点的值) nodeValue 2.3 删除节点 2.4 替换节点 2.5 插入节点 2.6 创建节点 2.7 克隆节点

#### 3. XML 对象

- node
- nodeList
- document
- element
- attr
- text
- comment

#### 4. HTMLElement(**元素**)对象

```javascript
className   类名

scrollLeft  滚动条至 左边界像素
scrollTop   滚动条至 上边界像素

offsetLeft  距离已定位父元素的 左偏移量
offsetTop   距离已定位父元素的 上偏移量

innerHTML   元素内部的内容(不含标签)
innerText   元素内部所有的文本内容
outerHTML   元素的内容(含标签)

offsetWidth  盒子模型,实际的宽: 内容+内边距+边框
offsetHeight  盒子模型,实际的高: 内容+内边距+边框

clientWidth  宽 + 内边距
clientHeight 高 + 内边距

scrollWidth  宽 + 内边距 + 计算里面元素的大小
scrollHeight 高 + 内边距 + 计算里面元素的大小

document.documentElement.clientHeight  视口高度
document.documentElement.scrollHeight  文档高度
```

### PS. 补充

- PS1. DOM 元素对象的 属性和方法 http://www.runoob.com/jsref/dom-obj-all.html
- PS2. MDN文档
  - Mozilla 开发者社区(MDN): https://developer.mozilla.org/zh-CN/
  - JavaScript MDN文档 https://developer.mozilla.org/zh-CN/docs/Web/JavaScript





## 2.DOM树

#### DOM节点：元素节点/属性节点/文本节点

### js操作节点（增删改查）

#### 一、获取节点：

##### 1、通过id获取

document.getElementById("id")
节点.getElementById("id值")
！返回的是一个具体的节点

##### 2、通过标签名来获取节点

getElementsByTagName("div")
！返回的是一个节点数组,即使只有一个

##### 3、通过标签的Name值来获取

getElementsByName("标签的name值")
!返回的是一个节点数组

##### 4、通过class值来获取节点

getElementsByClassName("类名")
!返回的是一个节点数组

##### *5、querySelector('选择器')//根据我选择器的结果集返回第一个

##### *6、querySelectorAll('选择器')//根据我选择器的结果集返回

!!!getElementsByClassName在IE9以下无效的

##### 7、获取节点.parentNode-->获取到节点的父节点

##### 8、获取节点.children-->获取到节点的子节点集合

​     获取节点.childNodes-->获取到节点的子节点集合（带有前后两个空白的文本节点）

#### 二、创建插入节点

1、document.createElement("div")//创建一个元素节点
2、document.createTextNode("文本文本")//创建一个文本节点

##### 被插入的节点

.appendChild(创建的节点)//在节点后面添加

##### 父节点

.insertBefore(创建的节点，被插入的节点)//在已知父节点的某个孩子前面添加内容

##### 改变文本内容：

选中的元素.innerText='';//直接将HTML代码当做字符来处理
选中的元素.innerHTML='';//可以识别HTML代码
删除：直接设置为空（""）

##### 替换节点：

父节点.replaceChild(新节点,老节点)

##### 克隆(复制节点)

选中的元素.cloneNode(true/false):
当clone参数为true的时候：选中元素里面所有懂得内容克隆
当clone参数为false的时候：选中元素本身克隆

##### 删除节点：

父节点.removeChild(子节点)	

##### 节点的属性操作

```
如何来获取属性：
	选中的元素.getAttribute("属性名")
更改属性：
	选中的元素.setAttribute("属性名","新的属性值")
新增属性
	选中的元素.setAttribute("原本没有的属性名","属性值")
删除属性
	选中的元素.removeAttribute("属性名");
```

# DOM中事件流-冒泡(work)

冒泡事件；捕获事件；阻止事件防止，在内部解决，不会在外部出问题！

window -> document -> body -> div -> (text) 捕获过程

 -> (text文本 ) -> div -> body -> document-> window  冒泡过程



![冒泡/捕获](/images/冒泡/捕获)

```
DOM中的事件流的三个机制

事件流:
页面触发一个事件时，会按照一定的顺序来响应事件，事件的响应过程为事件流
就我个人理解就是网页对点击事件的排序顺序就是事件流
```

```
事件流的起源：就是在浏览器发展到第四代的时候，浏览器开发团队遇到一个问题：页面的哪一部分会拥有某个特定的事件？要明白这个问题问的是什么，可以想象画在一张纸上的一组同心圆。如果你把手指放在圆心上，那么你的手指指向的不是一个圆，而是纸上的所有圆。也就是说如果单击了页面的某个按钮，同时也单击了按钮的容器元素，甚至单击了整个页面。
```

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>事件流</title>
    <style type="text/css">
        #content{width: 150px;height: 150px;background-color: red;}
        #btn{width: 80px;height: 80px;background-color: green;}
    </style>
</head>
<body>
    <div id="content">content
        <div id="btn">button</div>
    </div>

    <script type="text/javascript">
        var content = document.getElementById("content");
        var btn = document.getElementById('btn');
        btn.onclick = function(){
            alert("btn");
        };
        content.onclick = function(){
            alert("content");
        };
        document.onclick = function(){
            alert("document");
        }
    </script>
</body>
</html>
```

```
以上实例和我们阐述了 事件流基本的运行机制 
也就是 从最外的document 页面区域往btn区域执行在达到目标阶段时依次向最外面进行冒泡
```



- #### DOM事件流存在三个阶段: 事件捕获阶段,处于目标阶段,事件冒泡阶段

  #### 1. 什么是事件捕获

  ```
  通俗的理解就是，当鼠标点击或者触发dom事件时，浏览器会从根节点开始由外到内进行事件传播，即点击了子元素，如果父元素通过事件捕获方式注册了对应的事件的话，会先触发父元素绑定的事件。
  ```

  #### 2. 什么是事件冒泡
  
  ```
与事件捕获恰恰相反，事件冒泡顺序是由内到外进行事件传播，直到根节点。
  ```

  #### 3. 在达到目标阶段的情况下 实际上我们的目标阶段的事件被执行了两次

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Document</title>
    <style type="text/css">
    #wrapDiv, #innerP, #textSpan{
        margin: 5px;padding: 5px;box-sizing: border-box;cursor: default;
    }
    #wrapDiv{
        width: 300px;height: 300px;border: indianred 3px solid;
    }
    #innerP{
        width: 200px;height: 200px;border: hotpink 3px solid;
    }
    #textSpan{
        display: block;width: 100px;height: 100px;border: orange 3px solid;
    }
    </style>
</head>
<body>
     <div id="wrapDiv">wrapDiv
        <p id="innerP">innerP
            <span id="textSpan">textSpan</span>
        </p>
    </div>
    <script>
    var wrapDiv = document.getElementById("wrapDiv");
    var innerP = document.getElementById("innerP");
    var textSpan = document.getElementById("textSpan");

    // 捕获阶段绑定事件
    window.addEventListener("click", function(e){
        console.log("window 捕获", e.target.nodeName, e.currentTarget.nodeName);
    }, true);

    document.addEventListener("click", function(e){
        console.log("document 捕获", e.target.nodeName, e.currentTarget.nodeName);
    }, true);

    document.documentElement.addEventListener("click", function(e){
        console.log("documentElement 捕获", e.target.nodeName, e.currentTarget.nodeName);
    }, true);

    document.body.addEventListener("click", function(e){
        console.log("body 捕获", e.target.nodeName, e.currentTarget.nodeName);
    }, true);

    wrapDiv.addEventListener("click", function(e){
        console.log("wrapDiv 捕获", e.target.nodeName, e.currentTarget.nodeName);
    }, true);

    innerP.addEventListener("click", function(e){
        console.log("innerP 捕获", e.target.nodeName, e.currentTarget.nodeName);
    }, true);

    textSpan.addEventListener("click", function(e){
        console.log("textSpan 捕获", e.target.nodeName, e.currentTarget.nodeName);
    }, true);

    // 冒泡阶段绑定的事件
    window.addEventListener("click", function(e){
        console.log("window 冒泡", e.target.nodeName, e.currentTarget.nodeName);
    }, false);

    document.addEventListener("click", function(e){
        console.log("document 冒泡", e.target.nodeName, e.currentTarget.nodeName);
    }, false);

    document.documentElement.addEventListener("click", function(e){
        console.log("documentElement 冒泡", e.target.nodeName, e.currentTarget.nodeName);
    }, false);

    document.body.addEventListener("click", function(e){
        console.log("body 冒泡", e.target.nodeName, e.currentTarget.nodeName);
    }, false);

    wrapDiv.addEventListener("click", function(e){
        console.log("wrapDiv 冒泡", e.target.nodeName, e.currentTarget.nodeName);
    }, false);

    innerP.addEventListener("click", function(e){
        console.log("innerP 冒泡", e.target.nodeName, e.currentTarget.nodeName);
    }, false);

    textSpan.addEventListener("click", function(e){
        console.log("textSpan 冒泡", e.target.nodeName, e.currentTarget.nodeName);
    }, false);
</script>
</body>
</html>


```

```
从上面所画的事件传播的过程能够看出来，当点击鼠标后，会先发生事件的捕获

　　· 捕获阶段：首先window会获捕获到事件，之后document、documentElement、body会捕获到，再之后就是在body中DOM元素一层一层的捕获到事件，有wrapDiv、innerP。

　　· 目标阶段：真正点击的元素textSpan的事件发生了两次，因为在上面的JavaScript代码中，textSapn既在捕获阶段绑定了事件，又在冒泡阶段绑定了事件，所以发生了两次。但是这里有一点是需要注意，在目标阶段并不一定先发生在捕获阶段所绑定的事件，而是先绑定的事件发生，一会会解释一下。

　　· 冒泡阶段：会和捕获阶段相反的步骤将事件一步一步的冒泡到window

上述代码中的两个属性：e.target和e.currentTarget

　　target和currentTarget都是event上面的属性，target是真正发生事件的DOM元素，而currentTarget是当前事件发生在哪个DOM元素上。(监听器触发事件的节点)
　　
　　
　　

　　可以结合控制台打印出来的信息理解下，目标阶段也就是 target == currentTarget的时候。我没有打印它们两个因为太长了，所以打印了它们的nodeName，但是由于window没有nodeName这个属性，所以是undefined。
```





##### 那可能有一个疑问，我们不用addEventListener绑定的事件会发生在哪个阶段呢，我们来一个测试，顺便再演示一下我在上面的目标阶段所说的目标阶段并不一定先发生捕获阶段所绑定的事件是怎么一回事。

```html
<script>
    var wrapDiv = document.getElementById("wrapDiv");
    var innerP = document.getElementById("innerP");
    var textSpan = document.getElementById("textSpan");

    // 测试直接绑定的事件到底发生在哪个阶段
    wrapDiv.onclick = function(){
        console.log("wrapDiv onclick 测试直接绑定的事件到底发生在哪个阶段")
    };

    // 捕获阶段绑定事件
    window.addEventListener("click", function(e){
        console.log("window 捕获", e.target.nodeName, e.currentTarget.nodeName);
    }, true);

    document.addEventListener("click", function(e){
        console.log("document 捕获", e.target.nodeName, e.currentTarget.nodeName);
    }, true);

    document.documentElement.addEventListener("click", function(e){
        console.log("documentElement 捕获", e.target.nodeName, e.currentTarget.nodeName);
    }, true);

    document.body.addEventListener("click", function(e){
        console.log("body 捕获", e.target.nodeName, e.currentTarget.nodeName);
    }, true);

    wrapDiv.addEventListener("click", function(e){
        console.log("wrapDiv 捕获", e.target.nodeName, e.currentTarget.nodeName);
    }, true);

    innerP.addEventListener("click", function(e){
        console.log("innerP 捕获", e.target.nodeName, e.currentTarget.nodeName);
    }, true);

    textSpan.addEventListener("click", function(){
        console.log("textSpan 冒泡 在捕获之前绑定的")
    }, false);

    textSpan.onclick = function(){
        console.log("textSpan onclick")
    };

    textSpan.addEventListener("click", function(e){
        console.log("textSpan 捕获", e.target.nodeName, e.currentTarget.nodeName);
    }, true);

    // 冒泡阶段绑定的事件
    window.addEventListener("click", function(e){
        console.log("window 冒泡", e.target.nodeName, e.currentTarget.nodeName);
    }, false);

    document.addEventListener("click", function(e){
        console.log("document 冒泡", e.target.nodeName, e.currentTarget.nodeName);
    }, false);

    document.documentElement.addEventListener("click", function(e){
        console.log("documentElement 冒泡", e.target.nodeName, e.currentTarget.nodeName);
    }, false);

    document.body.addEventListener("click", function(e){
        console.log("body 冒泡", e.target.nodeName, e.currentTarget.nodeName);
    }, false);

    wrapDiv.addEventListener("click", function(e){
        console.log("wrapDiv 冒泡", e.target.nodeName, e.currentTarget.nodeName);
    }, false);

    innerP.addEventListener("click", function(e){
        console.log("innerP 冒泡", e.target.nodeName, e.currentTarget.nodeName);
    }, false);

    textSpan.addEventListener("click", function(e){
        console.log("textSpan 冒泡", e.target.nodeName, e.currentTarget.nodeName);
    }, false);
</script>
```



```
　　· textSpan是被点击的元素，也就是目标元素，所有在textSpan上绑定的事件都会发生在目标阶段，在绑定捕获代码之前写了绑定的冒泡阶段的代码，所以在目标元素上就不会遵守先发生捕获后发生冒泡这一规则，而是先绑定的事件先发生。[在目标元素上就不会遵守先发生捕获后发生冒泡这一规则，而是先绑定的事件先发生。]
　　· 由于wrapDiv不是目标元素，所以它上面绑定的事件会遵守先发生捕获后发生冒泡的规则。所以很明显用onclick直接绑定的事件发生在了冒泡阶段。
```



#### 4. 如何解决冒泡事件带来的影响呢

```
在支持addEventListener()的浏览器中，可以调用事件对象的stopPropagation()方法以阻止事件的继续传播。如果在同一对象上定义了其他处理程序，剩下的处理程序将依旧被调用，但调用stopPropagation()之后任何其他对象上的事件处理程序将不会被调用。不仅可以阻止事件在冒泡阶段的传播，还能阻止事件在捕获阶段的传播。

　　IE9之前的IE不支持stopPropagation()方法，而是设置事件对象cancelBubble属性为true来实现阻止事件进一步传播。
　　
　　
```



```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Document</title>
    <style type="text/css">
    #wrapDiv, #innerP, #textSpan{
        margin: 5px;padding: 5px;box-sizing: border-box;cursor: default;
    }
    #wrapDiv{
        width: 300px;height: 300px;border: indianred 3px solid;
    }
    #innerP{
        width: 200px;height: 200px;border: hotpink 3px solid;
    }
    #textSpan{
        display: block;width: 100px;height: 100px;border: orange 3px solid;
    }
    </style>
</head>
<body>
     <div id="wrapDiv">wrapDiv
        <p id="innerP">innerP
            <span id="textSpan">textSpan</span>
        </p>
    </div>
<script>
    var wrapDiv = document.getElementById("wrapDiv");
    var innerP = document.getElementById("innerP");
    var textSpan = document.getElementById("textSpan");

    // 测试直接绑定的事件到底发生在哪个阶段
    wrapDiv.onclick = function(){
        console.log("wrapDiv onclick 测试直接绑定的事件到底发生在哪个阶段")
    };

    // 捕获阶段绑定事件
    window.addEventListener("click", function(e){
        console.log("window 捕获", e.target.nodeName, e.currentTarget.nodeName);
    }, true);

    document.addEventListener("click", function(e){
        console.log("document 捕获", e.target.nodeName, e.currentTarget.nodeName);
    }, true);

    document.documentElement.addEventListener("click", function(e){
        console.log("documentElement 捕获", e.target.nodeName, e.currentTarget.nodeName);
    }, true);

    document.body.addEventListener("click", function(e){
        console.log("body 捕获", e.target.nodeName, e.currentTarget.nodeName);
    }, true);

    wrapDiv.addEventListener("click", function(e){
        console.log("wrapDiv 捕获", e.target.nodeName, e.currentTarget.nodeName);
        // 在捕获阶段阻止事件的传播
        e.stopPropagation();
    }, true);

    innerP.addEventListener("click", function(e){
        console.log("innerP 捕获", e.target.nodeName, e.currentTarget.nodeName);
    }, true);

    textSpan.addEventListener("click", function(){
        console.log("textSpan 冒泡 在捕获之前绑定的")
    }, false);

    textSpan.onclick = function(){
        console.log("textSpan onclick")
    };

    textSpan.addEventListener("click", function(e){
        console.log("textSpan 捕获", e.target.nodeName, e.currentTarget.nodeName);
    }, true);

    // 冒泡阶段绑定的事件
    window.addEventListener("click", function(e){
        console.log("window 冒泡", e.target.nodeName, e.currentTarget.nodeName);
    }, false);

    document.addEventListener("click", function(e){
        console.log("document 冒泡", e.target.nodeName, e.currentTarget.nodeName);
    }, false);

    document.documentElement.addEventListener("click", function(e){
        console.log("documentElement 冒泡", e.target.nodeName, e.currentTarget.nodeName);
    }, false);

    document.body.addEventListener("click", function(e){
        console.log("body 冒泡", e.target.nodeName, e.currentTarget.nodeName);
    }, false);

    wrapDiv.addEventListener("click", function(e){
        console.log("wrapDiv 冒泡", e.target.nodeName, e.currentTarget.nodeName);
         // 在冒泡阶段阻止事件的传播
        // e.stopPropagation();
    }, false);

    innerP.addEventListener("click", function(e){
        console.log("innerP 冒泡", e.target.nodeName, e.currentTarget.nodeName);
    }, false);

    textSpan.addEventListener("click", function(e){
        console.log("textSpan 冒泡", e.target.nodeName, e.currentTarget.nodeName);
    }, false);
</script>

```



```
结果:
　实际上我们点击的是textSpan，但是由于在捕获阶段事件就被阻止了传播，所以在textSpan上绑定的事件根本就没有发生，冒泡阶段绑定的事件自然也不会发生，因为阻止事件在捕获阶段传播的特性，e.stopPropagation()很少用到在捕获阶段去阻止事件的传播，大家就以为e.stopPropagation()只能阻止事件在冒泡阶段传播。
```

#### 5.阻止事件的默认行为***

e.preventDefault()可以阻止事件的默认行为发生，默认行为是指：点击a标签就转跳到其他页面、拖拽一个图片到浏览器会自动打开、点击表单的提交按钮会提交表单等等，因为有的时候我们并不希望发生这些事情，所以需要阻止默认行为。

　　IE9之前的IE中，可以通过设置事件对象的returnValue属性为false达到同样的效果。

```js
function cancelHandler(event){
    var event=event||window.event;//兼容IE
    
    //取消事件相关的默认行为
    if(event.preventDefault)    //标准技术
        event.preventDefault();
    if(event.returnValue)    //兼容IE9之前的IE
        event.returnValue=false;
    return false;    //用于处理使用对象属性注册的处理程序
}
```



#### 6. 事件委托***

在JavaScript中，添加到页面上的事件处理程序数量将直接关系到页面的整体运行性能。导致这一问题的原因是多方面的。首先，每个函数都是对象，都会占用内存；内存中的对象越多，性能就越差。其次，必须事先指定所有事件处理程序而导致的DOM访问次数，会延迟整个页面的交互就绪时间。

　　对“事件处理程序过多”问题的解决方案就是事件委托。事件委托利用了事件冒泡，只指定一个事件处理程序，就可以管理某一类型的所有事件。例如，click事件会一直冒泡到document层次。也就是说，我们可以为整个页面指定一个onclick事件处理程序，而不必给每个可单击的元素分别添加事件处理程序。

```html
<ul id="color-list">
    <li>red</li>
    <li>yellow</li>
    <li>blue</li>
    <li>green</li>
    <li>black</li>
    <li>white</li>
</ul>
```

```html
　　如果点击页面中的li元素，然后输出li当中的颜色，我们通常会这样写:
　　(function(){
    var color_list = document.getElementById('color-list');
    var colors = color_list.getElementsByTagName('li');
    for(var i=0;i<colors.length;i++){
        colors[i].addEventListener('click',showColor,false);
    };
    function showColor(e){
        var x = e.target;
        alert("The color is " + x.innerHTML);
    };
})();

```

```html
利用事件流的特性，我们只绑定一个事件处理函数也可以完成
(function(){
    var color_list = document.getElementById('color-list');
    color_list.addEventListener('click',showColor,false);
    function showColor(e){
        var x = e.target;
        if(x.nodeName.toLowerCase() === 'li'){
            alert('The color is ' + x.innerHTML);
        }
    }
})();
```

#### 7. 使用事件冒泡还是事件捕获呢

```
冒泡还是捕获？

　　对于事件代理来说，在事件捕获或者事件冒泡阶段处理并没有明显的优劣之分，但是由于事件冒泡的事件流模型被所有主流的浏览器兼容，从兼容性角度来说还是建议大家使用事件冒泡模型。

 

```

#### 事件委托还有一个好处

```html
事件委托还有一个好处就是添加进来的元素也能绑定事件：

没有使用事件委托：


<body>
 <ul id="thl">
   <li>001</li>
   <li>002</li>
   <li>003</li>
</ul>
<button onclick="fun()">touch</button>

<script>
    var thl= document.getElementById('thl');
    var aLi = thl.getElementsByTagName('li');
    for (var i = 0; i < aLi.length; i++) {
    　　aLi[i].onclick = fn;
    }
    
    function fn (){
      console.log(this.innerHTML);
    }

    function fun(){
        var node=document.createElement("li");
        var textnode=document.createTextNode("maomaoliang");
        node.appendChild(textnode);
        document.getElementById("thl").appendChild(node);
    }
</script>
</body>
```

```html
使用了事件委托
<script>
    var thl= document.getElementById('thl');
    thl.onclick = function(ev) {
        ev = ev || event;
        //兼容处理
        var target = ev.target || ev.srcElement;
    　　//找到li元素
        if (target.nodeName.toLowerCase() == 'li') {
              console.log(target.innerHTML);
         }
    };

    function fun(){
        var node=document.createElement("li");
        var textnode=document.createTextNode("maomaoliang");
        node.appendChild(textnode);
        document.getElementById("thl").appendChild(node);
    }
</script>
```







# 5.浏览器BOM

### 1. 什么是BOM

```
ECMAScript规定核心的语法:bom dom
Browser Object Model  浏览器对象模型
```

### 2. JavaScript 对象层次

#### 2.1 对象种类

- 自定义对象 Object

- 内置对象 A/S/B/N/D/M/R/G

- BOM 浏览器对象模型

- DOM Document Object Model 文档对象模型 ~~~

  #### 2.2 对象树 (倒树状结构)

```
                     window
                        |
history   location   document screen   navigator
                        |
                    doc    html
                            |
                    head   body
                     |       |
                title...   div span p h4 li  ul...
```

### 3. BOM 对象

#### 3.1 window

- 描述整个浏览器窗口的对象

- 它是JS中所有对象的根对象

- 使用window的属性或方法,可以省略window的调用

- 自定义对象 / 变量 / 函数

- 属性: 见手册

- 方法: clearInterval() 取消由 setInterval() 设置的 timeout。 clearTimeout() 取消由 setTimeout() 方法设置的 timeout。 setInterval() 按照指定的周期（以毫秒计）来调用函数或计算表达式。 setTimeout() 在指定的毫秒数后调用函数或计算表达式。

  alert() 警告框 prompt() 输入框 confirm() 确认框

  open() 打开新窗口 close() 关闭自己打开过的窗口 print() 打印

  scrollTo() 滚到哪去 scrollBy() 滚过少

#### 3.2 history 历史

length长度

back() forward() go() 后退,前进,去

#### 3.3 location位置

- 属性
- 方法

#### 3.4 screen屏幕

#### 3.5 navigator导航器





# JavaScript 事件

#### 1. 事件的绑定

- 事件作为 元素的属性

  ```
    <button event="JS CODE"></button>
  ```

- 事件作为 元素对象的属性

  ```
    element.event = function(){}
    element.event = funName;
  ```

- 事件监听(标准)

  ```
    非IE:
        addEventListener('事件名字', funName, false);
    IE:
        attachEvent('事件名字', funName);
  ```

  

  #### 2. 解除绑定

- 第1种和第2种的绑定方式

  ```
    重写覆盖属性为null 或 空的function(){}
    element.event = null
    element.event = function() {}
  ```

- 监听方式

  ```
    非IE:
        removeEventListener('事件名字', funName, false);
    IE:
        detachEvent('事件名字', funName);
  ```

#### 3. 给一组元素绑定事件和this的使用

- 循环绑定事件,获取触发事件的元素对象时,需要使用this
- 元素内部绑定事件时传入this.表示该元素对象自己

#### 4. 闭包 closure

- 在循环绑定事件时,将循环变量保留下来,就必须使用闭包

- 用一组元素去控制另一组元素时 请使用闭包

- 语法:

  ```
    for (...) {
        (function(i,x,y){
            element.event = function (){
                // i,x,y 值皆可用
            }
        })(i,x,y);
    }
  ```

#### 5. 常用事件

#### 5.1 鼠标事件

```
- onclick 单击触发
- ondblclick 双击触发
- oncontextmenu 右击触发/return false阻止系统菜单
- onmouseover 鼠标指向触发
- onmouseout 鼠标移开触发
- onmousedown 鼠标按下触发
- onmouseup 鼠标松开触发
- onmousemove 鼠标移动触发
```



#### 5.2 键盘事件

```
- onkeydown 按下按键触发
- onkeyup 松开按键触发
- onkeypress 按下并松开触发(JS高级事件) 不是所有的按键都能触发,无输出的按键是无法触发 (方向键/shift/ctrl/alt/fn/tab/大小写切换)
```



#### 5.3 表单事件

```
- onsubmit 表单被提交时触发
- onreset 表单被重置时触发
- onfocus 获取焦点时触发
- onblur 失去焦点时触发
```

#### 5.4 框架/对象事件

#### 5.5 其他事件

#### 6. event事件对象

- 6.1 获取 `var e = e || window.event;`

- 6.2 属性

  ```
    e.x       鼠标X坐标
    e.y       鼠标Y坐标
    e.button  检测鼠标按键 0左键/1中键/2右键
    e.offsetX 鼠标相对于 触发事件元素的x坐标
    e.offsetY 鼠标相对于 触发事件元素的y坐标
    e.keyCode 按键键码
  ```

### 7. 常用HTML元素属性

```
    innerHTML   双标签之间的文本

    当前元素 相对与body 或已定位的父元素的 偏移量
    offsetTop
    offsetLeft

    当前元素 左边缘或顶边缘 滚过的像素值
    scrollTop
    scrollLeft

    className   当前元素的class属性值
    tagName     当前元素的标签名
```

------



# js对象及数组

### js对象的分类：

### 内置对象

js已经提供好的对象，这些对象它有自己的方法和属性。如：
Number，String，Boolean，Date，Math，Array，window，location......



### 自定义对象

```javascript
1、如何来定义对象：
	1)语法：var obj={};
	2)使用我们的new关键字来创建
		var obj=new Object()//创建一个空对象
		var arr = new Array()//创建一个空的数组对象
		var time = new Date()//创建一个初始化的日期对象
	3)通过构造函数的形式来创建对象
		var obj = new Test();
		function Test(num1,num2){
			this.number1 = num1;
			this.number2 = num2
		}
4)通过Object.create()创建对象
		var obj = Object.create(null)
		var obj = Object.create({"name":"tom","age"："3"})
```





### 2、对象的属性

​	1、对象.属性名 = 属性值
​	2、对象属性值可以是任何一种js的数据类型 包括对象

### 3、获取对象的属性

​	1、对象.属性名
​	2、对象[属性名]

### 4、遍历对象（for in循环）

​	for(var 变量  in 对象){
​		//  属性名：变量
​		//  属性值: 对象[变量]
​	}

### 二、数组

1、数组内可以存放任意数据类型的数据（本质上它也是对象）
2、数组元素不赋值的情况下 值为undefined
3、如果数组打印的时候，元素不赋值""
4、访问数组范围之外的元素，不会出现越界的问题，undefined
5、定义数组大小，照样可以添加更多元素

### 定义数组的方法：

```
1、var arr=[]//定义一个空数组
2、var arr=[10,20,{"name":"tomy","age":19},0.1,"string",true,["aaa","bbb"]]//定义的同时赋值
3、var arr=new Array();//定义一个空数组
4、var arr = new Array(10,20,{"name":"tomy","age":19},0.1,"string",true,["aaa","bbb"])//定义的同时赋值
5、var arr=new Array(10)//定义一个长度为10的数组

赋值：
数组名[下标] = 值

取值：
数组名[下标]

更改值：
数组名[下标] = 值

数组的分类：
索引数组：下标是数字
关联数组：下标是可以是自定义的字符
```





​	

### 一维数组

### 二维数组:数组里面的元素还是数组

​	var arr = [["id","aaa",10],[1,1,2,3],[1,1,1]]
​	

### 循环二维数组

var arr = [["id","aaa",10],[1,1,2,3],[["a","b","c"],1,1]]
		

### 多维数组

```javascript
js 操作数组的api
！1）concat():连接两个或更多的数组的方法(不修改原数组)
	var arr1 = [1,2,3];
	var arr2 = [7,8,9];
	var newArr = arr1.concat(arr2)
！2）join()：将数组转成字符串，并通过指定的字符分割(未指定默认使用逗号“，”)
	var arr=[1,2,3]
	var str=arr.join("")
3）toString():吧数组转成字符串然后通过,隔开
	var arr=["a","b","c","d"];
	var string = arr.toString()
	console.log(string)
！4）slice():从已有的数组中返回指定的元素
	语法：
	var string = arr.slice(start,end)//start==>开始位置下标   end==>结束位置下标
	var Arr = [1,2,3,4,5,6,7,8,9,10]
	var subArr = Arr.slice(2,4)
	console.log(Arr)
5）splice():删除 插入 会修改原数组
	var arr=[]
	语法：var temp = arr.splice(num1,num2)
	arr:被切割数组
	temp：切割完获取数组元素的数组
	num1：切割开始的下标
	num2：切割多少位

var del = [1,2,3,4,5,6,7,8,9]
		var delected = del.splice(3,5)
		console.log(delected)
		console.log(del)
!6）push：向数组的末尾添加一个或多个的新元素
		var arr=[1,2,3,4,5,6,7,8,9]
		arr.push(10)

!7)	pop:删除并返回最后一个元素(直接修改原数组)
	var arr=[1,2,3,4,5,6,7,8,9]
	var a = arr.pop()
!8) shift:删除并返回第一个元素
	var arr=[1,2,3,4,5,6,7,8,9]
	var a = arr.shift()
!9) sort:排序
	var arr=[9,1,3,6,7,2,8,5,4]
	var a = arr.sort()
10）reverse:颠倒的数组顺序
	var arr=[1,2,3,4,5,6,7,8,9]
	var a = arr.reverse()
```






# 6.AJAX(js)

## 1.Ajax概念

**AJAX 是一种在无需重新加载整个网页的情况下，能够更新部分网页的技术。**

AJAX = 异步 JavaScript + XML。

```
xml可扩展标记语言，标准通用标记语言的子集，是一种用于标记电子文件使其具有结构性的标记语言。
```

AJAX 是一种用于创建快速动态网页的技术。

通过在后台与服务器进行少量数据交换，AJAX 可以使网页实现异步更新。这意味着可以在不重新加载整个网页的情况下，对网页的某部分进行更新。

传统的网页（不使用 AJAX）如果需要更新内容，必需重载整个网页面。



## 2.参数

- ### 1-type

  类型：String

  默认值: “GET”)。请求方式 (“POST” 或 “GET”)， 默认为 “GET”。注意：其它 HTTP 请求方法，如 PUT 和 DELETE 也可以使用，但仅部分浏览器支持。

- ### 2-url

  类型：String

  默认值: 当前页地址。发送请求的地址。

- ### 3-dataType

  类型：String

  预期服务器返回的数据类型。如果不指定，jQuery 将自动根据 HTTP 包 MIME 信息来智能判断，比如 XML MIME 类型就被识别为 XML。

  在 1.4 中，JSON 就会生成一个 JavaScript 对象，而 script 则会执行这个脚本。随后服务器端返回的数据会根据这个值解析后，传递给回调函数。可用值:

  - “xml”: 返回 XML 文档，可用 jQuery 处理。
  - “html”: 返回纯文本 HTML 信息；包含的 script 标签会在插入 dom 时执行。
  - “script”: 返回纯文本 JavaScript 代码。不会自动缓存结果。除非设置了 “cache” 参数。注意：在远程请求时(不在同一个域下)，所有 POST 请求都将转为 GET 请求。（因为将使用 DOM 的 script标签来加载）
  - “json”: 返回 JSON 数据 。
  - “jsonp”: JSONP 格式。使用 JSONP 形式调用函数时，如 “myurl?callback=?” jQuery 将自动替换 ? 为正确的函数名，以执行回调函数。
  - “text”: 返回纯文本字符串

- ### 4-data

  类型：String

  发送到服务器的数据。将自动转换为请求字符串格式。GET 请求中将附加在 URL 后。查看 processData 选项说明以禁止此自动转换。必须为 Key/Value 格式。如果为数组，jQuery 将自动为不同值对应同一个名称。如 {foo:[“bar1”, “bar2”]} 转换为 ‘&foo=bar1&foo=bar2’。

- ### 5-success

  类型：Function

  请求成功后的回调函数。

  参数：由服务器返回，并根据 dataType 参数进行处理后的数据；描述状态的字符串。

  这是一个 Ajax 事件。

  

  

  ### 6-error

  类型：Function

  默认值: 自动判断 (xml 或 html)。请求失败时调用此函数。

  有以下三个参数：XMLHttpRequest 对象、错误信息、（可选）捕获的异常对象。

  如果发生了错误，错误信息（第二个参数）除了得到 null 之外，还可能是 “timeout”, “error”, “notmodified” 和 “parsererror”。

  这是一个 Ajax 事件。

  

  举例说明一些错误原因：

  **1. dataType错误**

  类型错误：后台返回的dataType类型和前台写的不一致会跳入error

  格式错误：jquery1.4之后对json的格式要求非常严格，json格式错误也会跳入error.{“test”:1} 注意格式

  有时，在不需要返回值的情况下，扔按模板格式，设置了dataType:”json”,参数；这时候，ajax传值正确时，出现200返回成功状态下报错的特殊情况。

  ### 2.async请求同步异步问题

   async默认是true(异步请求),如果想一个Ajax执行完后再执行另一个Ajax, 需要把async=false

   例如，你用post请求传值到另一个页面后台，但是页面一加载你的ajax就已经执行过了，传值接收是在后台才完成的，这时候就请求不到数据，所以可以考虑把ajax请求改为同步试试。

  ### 3. data不能不写

  data为空也一定要传”{}”；不然返回的是xml格式的。并提示parsererror. data:”{}”

  parsererror的异常和Header 类型也有关系。及编码header(‘Content-type: text/html; **charset=utf8**’);

  ### 4. 传递的参数

   必须是ajax支持的编码格式

  ### 5.URL路径问题

   路径不能有中文

## 3.考题

```javascript
请求的url:user.php
发送方式:post
发送数据:id为userid的文本框值
返回数据:json格式
请求成功:将返回数据写入id为username的文本框中
请求失败:弹出文本“操作失败”


$.ajax({
	type:”POST”,
​	url:”user.php”,
​	dateType:”json”,
​	date:{“id”:$(“#userid”).val()};
​	success:function(msg){
​	$(“#username”).val(msg);
​	},
​	error:function(msg){
​	alert(“操作失败”);
​	}
})
```





# ajax请求五步（work）

```
小结：
	1.了解js面试题 大概内容
	2.了解ajax大致 似乎用方法
```

```javascript
原生ajax请求的五个步骤
//第一步，创建XMLHttpRequest对象
var xmlHttp = new XMLHttpRequest();
function CommentAll() {
    //第二步，注册回调函数
    xmlHttp.onreadystatechange =callback1;
    //{
    //    if (xmlHttp.readyState == 4)
    //        if (xmlHttp.status == 200) {
    //            var responseText = xmlHttp.responseText;

    //        }
    //}
    //第三步，配置请求信息，open(),get
    //get请求下参数加在url后，.ashx?methodName = GetAllComment&str1=str1&str2=str2
    xmlHttp.open("post", "/ashx/myzhuye/Detail.ashx?methodName=GetAllComment", true);

    //post请求下需要配置请求头信息
    //xmlHttp.setRequestHeader("Content-Type", "application/x-www-form-urlencoded");

    //第四步，发送请求,post请求下，要传递的参数放这
    xmlHttp.send("methodName = GetAllComment&str1=str1&str2=str2");//"

}
//第五步，创建回调函数
function callback1() {
    if (xmlHttp.readyState == 4)
        if (xmlHttp.status == 200) {
            //取得返回的数据
            var data = xmlHttp.responseText;
            //json字符串转为json格式
            data = eval(data);
            $.each(data,
                function(i, v) {
                    alert(v);
                });       
        }
}



//后台方法
 private  void GetAllComment(HttpContext context)
        {

            //Params可以取得get与post方式传递过来的值。
            string methodName = context.Request.Params["methodName"];

            //QueryString只能取得get方式传递过来的值。
            string str1 = context.Request.Form["str1"];

            //取得httpRequest传来的值，包括get与post方式
            string str2 = context.Request["str2"];

            List<string> comments = new List<string>();

            comments.Add(methodName);

            comments.Add(str1);

            comments.Add(str2);


            //ajax接受的是json类型，需要把返回的数据转给json格式
            string commentsJson = new JavaScriptSerializer().Serialize(comments);
            context.Response.Write(commentsJson);
        }
```







# 7.JS继承（work）

JS是面向对象的弱类型语言，继承也是其非常强大的特性之一。

##### 继承 是面向对象软件技术当中的一个概念，与多态、抽象共为面向对象的三个基本特征。 

##### 继承可以使得子类具有父类的属性和方法或者重新定义、追加属性和方法等。

##### 主要分为四种: 原型继承、 构造函数继承、 组合继承以及 寄生继承

```
既然要实现继承，那么首先我们得有一个父类，代码如下：
// 定义一个动物类
function Animal (name) {
  // 属性
  this.name = name || 'Animal';
  // 实例方法
  this.sleep = function(){
    console.log(this.name + '正在睡觉！');
  }
}
// 原型方法
Animal.prototype.eat = function(food) {
  console.log(this.name + '正在吃：' + food);
};



```

##### 先提供一个父类

```
//父类
function Person(name) {
	this.name = name;
	this.sum = function(){
		alert(this.name);
	}
}
Person.prototype.age = 10; //给构造函数添加了原型属性 
```

##### 原型链继承

```
function Per(){
	this.name = "ker";
}
Per.prototype = new Person();
var per1 = new Per();
//instanceof 判断元素是否在另一个元素的原型链上
//per1 继承了Person的属性 返回true
console.log(per1 instanceof Person);//true
```

### 1、原型(链)继承（3、4两大致命缺陷）

**核心：** 将父类的实例作为子类的原型  

##### 原型和构造函数的关系：

优点：父类新增原型方法/原型属性，子类都能访问到

缺点：继承过来的属性的值都是一样的了，只能对调用对象的属性进行重新赋值

```javascript
function Cat(){ 
}
Cat.prototype = new Animal();
Cat.prototype.name = 'cat';

//　Test Code
var cat = new Cat();
console.log(cat.name);
console.log(cat.eat('fish'));
console.log(cat.sleep());
console.log(cat instanceof Animal); //true 
console.log(cat instanceof Cat); //true
```

### 特点：

```


1. 非常纯粹的继承关系，实例是子类的实例，也是父类的实例
2. 父类新增原型方法/原型属性，子类都能访问到
3. 简单，易于实现

缺点：

1. 要想为子类新增属性和方法，必须要在`new Animal()`这样的语句之后执行，不能放到构造器中
2. 无法实现多继承
3. 来自原型对象的引用属性是所有实例共享的（详细请看附录代码： 示例1）
4. 创建子类实例时，无法向父类构造函传参

缺点1中描述有误：可以在Cat构造函数中，为Cat实例增加实例属性。如果要新增原型属性和方法，则必须放在new Animal()这样的语句之后执行。
--------------------
特点:(小老弟)
实例可继承的属性有: 实例的构造函数的属性
父类构造函数属性
父类原型的属性

缺点：
新实例无法向父类构造函数传参
继承单一
所有新实例都会共享父类实例的属性
```



### 2、构造继承



```
function Con(){
	Person.call(this,"jer");
	this.age = 12;
}
var con1 = new Con();
console.log(con1.name);
console.log(con1.age);
console.log(con1 instanceof Person);//false
```

- 重点: 用.call()或.apply() 将父类构造函数引入子类函数

**核心：**使用父类的构造函数来增强子类实例，等于是复制父类的实例属性给子类（没用到原型）

##### 借用构造函数:构造函数名字.call(当前对象,属性,属性,属性....); 解决了属性继承,并且值不重复的问题

优点：可以实现多继承（call多个父类对象）

缺点：无法继承父类方法

```javascript
function Cat(name){
  Animal.call(this);
  this.name = name || 'Tom';
}

// Test Code
var cat = new Cat();
console.log(cat.name);
console.log(cat.sleep());
console.log(cat instanceof Animal); // false
console.log(cat instanceof Cat); // true
```

```
特点：

1. 解决了1中，子类实例共享父类引用属性的问题
2. 创建子类实例时，可以向父类传递参数
3. 可以实现多继承（call多个父类对象）

缺点：

1. 实例并不是父类的实例，只是子类的实例
2. 只能继承父类的实例属性和方法，不能继承原型属性/方法
3. 无法实现函数复用，每个子类都有父类实例函数的副本，影响性能

- 特点:(小老弟)
  - 只继承了父类构造函数的属性，没有继承父类原型的属性
  - 解决了原型链继承缺点
  - 可以继承多个构造函数属性(call 多个)
  - 在子实例中可向父实例传参
- 缺点
  - 只能继承父类构造函数的属性
  - 无法实现构造函数的复用 (每次用每次都有重新调用)
```





### 3、组合继承★★★★（仅仅多消耗了一点内存）

##### 组合继承(组合原型链继承和借用构造函数继承)

```
function SubType(name) {
	Person.call(this,name);//构造函数继承
}
SubType.prototype = new Person();//原型链继承
var sub = new SubType("ger");
console.log(sub.name);
console.log(sub.age);
```

- 重点: 结合了两种模式的优点，传参和复用

##### 简单来说：就是原型继承和构造函数继承的组合

优点：既可以多继承还可以继承父类的方法

缺点：要生成两个实例，比前两种要占内存

**核心：**通过调用父类构造，继承父类的属性并保留传参的优点，然后通过将父类实例作为子类原型，实现函数复用

```javascript
function Cat(name){
  Animal.call(this);
  this.name = name || 'Tom';
}
Cat.prototype = new Animal();

// Test Code
var cat = new Cat();
console.log(cat.name);
console.log(cat.sleep());
console.log(cat instanceof Animal); // true
console.log(cat instanceof Cat); // true
```

### 特点：

```
1. 弥补了方式2的缺陷，可以继承实例属性/方法，也可以继承原型属性/方法
2. 既是子类的实例，也是父类的实例
3. 不存在引用属性共享问题
4. 可传参
5. 函数可复用

缺点：
1. 调用了两次父类构造函数，生成了两份实例（子类实例将子类原型上的那份屏蔽了）
---------------



- 特点
  - 可以继承父类原型上的属性，可以传参，可复用
  - 每个新实例引入的构造函数属性是私有的
- 缺点：
  - 调用了两次父类构造函数（耗内存），子类的构造函数会代替原型上的构造函数


```





### 4、寄生组合继承★★★★（实现复杂，扣掉一颗星）

```javascript
//寄生
function content(obj){
	function F(){}
	F.prototype = obj;
	return new F();
}
var con = content(Person.prototype);
//con实例（F实例）的原型继承了父类函数的原型
//上述就像原型链继承，只不过只继承了原型属性

//组合
function Sub(){
	Person.call(this);
}//继承了父类构造函数的属性解决了组合式两次调用构造函数属性的缺点

Sub.prototype = con;
con.constructor = Sub;//修复实例
var sub1 = new Sub();
//Sub实例就继承了构造函数属性，父类实例，con的函数属性

----------------------------------------------------------------------------------
//不同写法
function F(){};
F.prototype = Person.prototype;
function Sub(){
	Person.call(this);
}
Sub.prototype = new F();
var sub2 = new Sub();
```

- 重点:修复了组合继承的问题

**核心：**通过寄生方式，砍掉父类的实例属性，这样，在调用两次父类的构造的时候，就不会初始化两次实例方法/属性，避免的组合继承的缺点

##### 其实就是在原型式继承得到对象的基础上，在内部再以某种方式来增强对象，然后返回增强

优点：不限制调用方式，不管是new 子类()还是子类(),返回的对象具有相同的效果

缺点：不能多继承

```javascript
function Cat(name){
  Animal.call(this);
  this.name = name || 'Tom';
}
(function(){
  // 创建一个没有实例方法的类
  var Super = function(){};
  Super.prototype = Animal.prototype;
  //将实例作为子类的原型
  Cat.prototype = new Super();
})();

// Test Code
var cat = new Cat();
console.log(cat.name);
console.log(cat.sleep());
console.log(cat instanceof Animal); // true
console.log(cat instanceof Cat); //true
```

特点：堪称完美

缺点：实现较为复杂

### 5、实例继承（不需要看）

**核心：**为父类实例添加新特性，作为子类实例返回

```
function Cat(name){
  var instance = new Animal();
  instance.name = name || 'Tom';
  return instance;
}

// Test Code
var cat = new Cat();
console.log(cat.name);
console.log(cat.sleep());
console.log(cat instanceof Animal); // true
console.log(cat instanceof Cat); // false
```

 特点：

1. 不限制调用方式，不管是`new 子类()`还是`子类()`,返回的对象具有相同的效果

缺点：

1. 实例是父类的实例，不是子类的实例
2. 不支持多继承

### 6、拷贝继承（★缺点1）不用看

```javascript
function Cat(name){
  var animal = new Animal();
  for(var p in animal){
    Cat.prototype[p] = animal[p];
  }
  Cat.prototype.name = name || 'Tom';
}

// Test Code
var cat = new Cat();
console.log(cat.name);
console.log(cat.sleep());
console.log(cat instanceof Animal); // false
console.log(cat instanceof Cat); // true
```

特点：

1. 支持多继承

缺点：

1. 效率较低，内存占用高（因为要拷贝父类的属性）
2. 无法获取父类不可枚举的方法（不可枚举方法，不能使用for in 访问到）



## 附录代码：

示例一：

```
function Animal (name) {
  // 属性
  this.name = name || 'Animal';
  // 实例方法
  this.sleep = function(){
    console.log(this.name + '正在睡觉！');
  }
  //实例引用属性
  this.features = [];
}
function Cat(name){
}
Cat.prototype = new Animal();

var tom = new Cat('Tom');
var kissy = new Cat('Kissy');

console.log(tom.name); // "Animal"
console.log(kissy.name); // "Animal"
console.log(tom.features); // []
console.log(kissy.features); // []

tom.name = 'Tom-New Name';
tom.features.push('eat');

//针对父类实例值类型成员的更改，不影响
console.log(tom.name); // "Tom-New Name"
console.log(kissy.name); // "Animal"
//针对父类实例引用类型成员的更改，会通过影响其他子类实例
console.log(tom.features); // ['eat']
console.log(kissy.features); // ['eat']
```

原因分析：

```
关键点：属性查找过程

执行tom.features.push，首先找tom对象的实例属性（找不到），
那么去原型对象中找，也就是Animal的实例。发现有，那么就直接在这个对象的
features属性中插入值。
在console.log(kissy.features); 的时候。同上，kissy实例上没有，那么去原型上找。
刚好原型上有，就直接返回，但是注意，这个原型对象中features属性值已经变化了。
```





#  8.jQuery 



## jQuery vs JavaScript 

jQuery 由 John Resig 于 2006 年创建。它旨在处理浏览器不兼容性并简化 HTML DOM 操作、事件处理、动画和 Ajax。

十多年来，jQuery 一直是世界上最受欢迎的 JavaScript 库。

但是，在 JavaScript Version 5（2009）之后，大多数 jQuery 实用程序都可以通过几行标准 JavaScript 来解决：



## DOM 选择器

#### 1.通过 id 来查找 HTML 元素

返回 id="intro" 的元素：

#### jQuery

```
var myElement = $("#id01");
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
<!DOCTYPE html>
<html>
<head>
<script src="/jquery/jquery.min.js"></script>
</head>
<body>

<h1>通过 id 查找 HTML 元素</h1>

<p id="id01">Hello World!</p>
<p id="id02">Hello China!</p>
<p id="id03">Hello Shanghai!</p>

<p id="demo"></p>

        <script>
        $(document).ready(function() {
          var myElements = $("#id03");
          $("#demo").text("段落 id03 的文本是：" + myElements[0].innerHTML);
        });
        </script>

</body>
</html>

//结果：
//通过 id 查找 HTML 元素
Hello World!
Hello China!
Hello Shanghai!
段落 id03 的文本是：Hello Shanghai!


```

#### JavaScript



```
var myElement = document.getElementById("id01");

<!DOCTYPE html>
<html>
<body>

<h1>通过 id 查找 HTML 元素</h1>

<p id="id01">Hello World!</p>
<p id="id02">Hello China!</p>
<p id="id03">Hello Shanghai!</p>

<p id="demo"></p>

        <script>
        var myElement = document.getElementById("id03");
        document.getElementById("demo").innerHTML = "段落 id03 的文本是：" + myElement.innerHTML;
        </script>

</body>
</html>


```





## 2.通过标签名来查找 HTML 元素

返回所有 <p> 元素：

### jQuery

```
var myElements = $("p");
```

### 实例

```
var myElements = document.getElementsByTagName("p");
```

## 3.通过类名来查找 HTML 元素

返回 class="intro" 的所有元素。

### jQuery

```
var myElements = $(".intro");
```

### JavaScript

```
var myElements = document.getElementsByClassName("intro");
```

按类名查找元素在 Internet Explorer 8 和早期版本中不起作用。

## 通过 CSS 选择器查找 HTML 元素

返回包含 class="intro" 的所有 <p> 元素的列表。

### jQuery

```
var myElements = $("p.intro");
```

### JavaScript

```
var myElements = document.querySelectorAll("p.intro");
```

querySelectorAll() 方法在 Internet Explorer 8 和早期版本中不起作用。





## jq-HTML 元素



```
### 1设置文本内容

设置 HTML 元素的内部文本：

jQuery
myElement.text("Hello China!");

JavaScript
myElement.textContent = "Hello China!";


### 2获取文本内容

获取 HTML 元素的内部文本：
 jQuery
var myText = myElement.text();
JavaScript
var myText = myElement.textContent || myElement.innerText;

### 3设置 HTML 内容

设置元素的 HTML 内容：
jQuery
var myElement.html("<p>Hello World</p>");
JavaScript
var myElement.innerHTML = "<p>Hello World</p>";


#### 获取 HTML 内容

获取元素的 HTML 内容：
 jQuery
var content = myElement.html();
JavaScript
var content = myElement.innerHTML;

```





## JavaScript / jQuery CSS 样式

```


隐藏 HTML 元素
隐藏一个 HTML 元素：
jQuery
myElement.hide();
JavaScript
myElement.style.display = "none";


显示 HTML 元素
显示一个 HTML 元素：
jQuery
myElement.show();
JavaScript
myElement.style.display = "";

样式化 HTML 元素
更改 HTML 元素的字体尺寸：
jQuery
myElement.css("font-size","35px");
JavaScript
myElement.style.fontSize = "35px";
```



## javaScript / jQuery HTML DOM

```
删除元素
删除 HTML 元素：
jQuery
$("#id").remove();
JavaScript
element.parentNode.removeChild(element);

获取父元素
返回 HTML 元素的父元素：
jQuery
var myParent = myElement.parent();
JavaScript
var myParent = myElement.parentNode;
```









# 9.Bootstrap

## 什么是 Bootstrap？

Bootstrap 是一个用于快速开发 Web 应用程序和网站的前端框架。Bootstrap 是基于 HTML、CSS、JAVASCRIPT 的。

## 历史

Bootstrap 是由 *Twitter* 的 *Mark Otto* 和 *Jacob Thornton* 开发的。Bootstrap 是 2011 年八月在 GitHub 上发布的开源产品。

## 为什么使用 Bootstrap？

- **移动设备优先**：自 Bootstrap 3 起，框架包含了贯穿于整个库的移动设备优先的样式。

- 浏览器支持

  ：所有的主流浏览器都支持 Bootstrap。

- **容易上手**：只要您具备 HTML 和 CSS 的基础知识，您就可以开始学习 Bootstrap。

- 响应式设计

  ：Bootstrap 的响应式 CSS 能够自适应于台式机、平板电脑和手机。

  Bootstrap 响应式设计

- 它为开发人员创建接口提供了一个简洁统一的解决方案。

- 它包含了功能强大的内置组件，易于定制。

- 它还提供了基于 Web 的定制。

- 它是开源的。

## Bootstrap 包的内容

- **基本结构**：Bootstrap 提供了一个带有网格系统、链接样式、背景的基本结构。这将在 **Bootstrap 基本结构** 部分详细讲解。

- **CSS**：Bootstrap 自带以下特性：全局的 CSS 设置、定义基本的 HTML 元素样式、可扩展的 class，以及一个先进的网格系统。这将在 **Bootstrap CSS** 部分详细讲解。

- **组件**：Bootstrap 包含了十几个可重用的组件，用于创建图像、下拉菜单、导航、警告框、弹出框等等。这将在 **布局组件** 部分详细讲解。

- JavaScript 插件

  ：Bootstrap 包含了十几个自定义的 jQuery 插件。您可以直接包含所有的插件，也可以逐个包含这些插件。这将在

   

  Bootstrap 插件

  

  

- 定制

  ：您可以定制 Bootstrap 的组件、LESS 变量和 jQuery 插件来得到您自己的版本。

  

------

## 在线实例

本站的 Bootstrap 教程包含了上百个实例。

你可以使用我们的在线编辑器在线编辑代码，并点击运行按钮查看结果。

## Bootstrap 实例



---------------------------------------------

<div class="container">
  <div class="jumbotron">
    <h1>我的第一个 Bootstrap 页面</h1>
    <p>重置窗口大小，查看响应式效果！</p> 
  </div>
  <div class="row">
    <div class="col-sm-4">
      <h3>Column 1</h3>
      <p>学的不仅是技术，更是梦想！</p>
      <p>再牛逼的梦想,也抵不住你傻逼似的坚持！</p>
    </div>
    <div class="col-sm-4">
      <h3>Column 2</h3>
      <p>学的不仅是技术，更是梦想！</p>
      <p>再牛逼的梦想,也抵不住你傻逼似的坚持！</p>
    </div>
    <div class="col-sm-4">
      <h3>Column 3</h3> 
      <p>学的不仅是技术，更是梦想！</p>
      <p>再牛逼的梦想,也抵不住你傻逼似的坚持！</p>
    </div>
  </div>
</div>



```html
<div class="container">
  <div class="jumbotron">
    <h1>我的第一个 Bootstrap 页面</h1>
    <p>重置窗口大小，查看响应式效果！</p> 
  </div>
  <div class="row">
    <div class="col-sm-4">
      <h3>Column 1</h3>
      <p>学的不仅是技术，更是梦想！</p>
      <p>再牛逼的梦想,也抵不住你傻逼似的坚持！</p>
    </div>
    <div class="col-sm-4">
      <h3>Column 2</h3>
      <p>学的不仅是技术，更是梦想！</p>
      <p>再牛逼的梦想,也抵不住你傻逼似的坚持！</p>
    </div>
    <div class="col-sm-4">
      <h3>Column 3</h3> 
      <p>学的不仅是技术，更是梦想！</p>
      <p>再牛逼的梦想,也抵不住你傻逼似的坚持！</p>
    </div>
  </div>
</div>
```



## -------------------

## Bootstrap 实例2

<div class="table-responsive">          
 <table class="table table-striped table-bordered">
   <thead>
     <tr>
       <th>#</th>
       <th>Name</th>
       <th>Street</th>
     </tr>
   </thead>
   <tbody>
     <tr>
       <td>1</td>
       <td>Anna Awesome</td>
       <td>Broome Street</td>
     </tr>
     <tr>
       <td>2</td>
       <td>Debbie Dallas</td>
       <td>Houston Street</td>
     </tr>
     <tr>
       <td>3</td>
       <td>John Doe</td>
       <td>Madison Street</td>
     </tr>
   </tbody>
 </table>
</div>













# 10.JSON 教程

------

JSON: **J**ava**S**cript **O**bject **N**otation(JavaScript 对象表示法)

JSON 是存储和交换文本信息的语法。类似 XML。

JSON 比 XML 更小、更快，更易解析。

##  JSON ？

- JSON 指的是 JavaScript 对象表示法（**J**ava**S**cript **O**bject **N**otation）
- JSON 是轻量级的文本数据交换格式
- JSON 独立于语言：JSON 使用 Javascript语法来描述数据对象，但是 JSON 仍然独立于语言和平台。JSON 解析器和 JSON 库支持许多不同的编程语言。 目前非常多的动态（PHP，JSP，.NET）编程语言都支持JSON。
- JSON 具有自我描述性，更易理解

------

## JSON - 转换为 JavaScript 对象

JSON 文本格式在语法上与创建 JavaScript 对象的代码相同。

由于这种相似性，无需解析器，JavaScript 程序能够使用内建的 eval() 函数，用 JSON 数据来生成原生的 JavaScript 对象。









### JSON - 简介



```html
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>菜鸟教程(runoob.com)</title>
</head>
<body>
<h2>JavaScript 创建 JSON 对象</h2>
<p>
网站名称: <span id="jname"></span><br /> 
网站地址: <span id="jurl"></span><br /> 
网站 slogan: <span id="jslogan"></span><br /> 
</p>
<script>
var JSONObject= {
    "name":"菜鸟教程",
    "url":"www.runoob.com", 
    "slogan":"学的不仅是技术，更是梦想！"
};
document.getElementById("jname").innerHTML=JSONObject.name 
document.getElementById("jurl").innerHTML=JSONObject.url 
document.getElementById("jslogan").innerHTML=JSONObject.slogan
</script>
 
</body>
</html>
```





与 XML 相同之处

- JSON 是纯文本
- JSON 具有"自我描述性"（人类可读）
- JSON 具有层级结构（值中存在值）
- JSON 可通过 JavaScript 进行解析
- JSON 数据可使用 AJAX 进行传输

------

## 与 XML 不同之处

- 没有结束标签
- 更短
- 读写的速度更快
- 能够使用内建的 JavaScript eval() 方法进行解析
- 使用数组
- 不使用保留字

------

## 为什么使用 JSON？

对于 AJAX 应用程序来说，JSON 比 XML 更快更易使用：

#### 使用 XML

- 读取 XML 文档
- 使用 XML DOM 来循环遍历文档
- 读取值并存储在变量中

#### 使用 JSON

- 读取 JSON 字符串
- 用 eval() 处理 JSON 字符串





# == & ===



==：运算符称作相等，用来检测两个操作数是否相等，这里的相等定义的非常宽松，可以允许进行类型转换
===：用来检测两个操作数是否严格相等
1、对于string,number等基础类型，==和===是有区别的
不同类型间比较，==之比较“转化成同一类型后的值”看“值”是否相等；

##### ===如果类型不同，其结果就是不等

同类型比较，直接进行“值”比较，两者结果一样

2、对于Array,Object等高级类型，==和===是没有区别的

3、基础类型与高级类型，==和===是有区别的

对于==，将高级转化为基础类型，进行“值”比较，因为类型不同，===结果为false

