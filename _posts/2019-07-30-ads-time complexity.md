---
layout: post
title: "《数据结构与算法》的学习-时间复杂度py3和c"
date: 2019-08-23
tag: ads
---









dataStructure-algorithm（已经讲过）

## 算法效率的度量方法

**1.事后统计方法**

这种方法主要是通过设计好的测试程序和数据，利用计算机计时器对不同算法编制的程序的运行时间进行比较，从而确定算法效率的高低。

**2.事前分析估算方法**

在计算机程序编写前，依据统计方法对算法进行估算。

经过总结，我们发现一个高级语言编写的程序在计算机上运行时所消耗的时间取决于下列因素：

1. 算法采用的策略，方案
2. 编译产生的代码质量
3. 问题的输入规模
4. 机器执行指令的速度

> >由此可见，抛开这些与计算机硬件、软件有关的因素，一个程序的运行时间依赖于算法的好坏和问题的输入规模。（所谓的问题输入规模是指输入量的多少）





## 算法的空间复杂度 

```
算法的空间复杂度 约为占用内存
   是程序运行从开始到结束所需的存储量。  
问题实例的特征 : 
    与问题的具体实例有关的量。
    
    例如，对一组特定个数的元素进行排序，对该组元素的排序是排序问题的一个实例。元素的个数可视为该实例的特征。


程序运行所需的存储空间包括两部分：
（1）固定部分  这部分空间与所处理数据的大小和个数无关，或者称与问题的实例的特征无关。主要包括程序代码、常量、简单变量、定长成分的结构变量所占的空间。
（2）可变部分  这部分空间大小与算法在某次执行中处理的特定数据的大小和规模有关。例如，分别为100个元素的两个数组相加，与分别为10个元素的两个数组相加，所需的存储空间显然是不同的。    

```





## 算法的时间复杂度 

```c++

算法的时间复杂度	
   是程序运行从开始到结束所需的时间。  
程序步  
        一个程序步是指在语法上或语义上有意义的程序段，该程序段的执行时间与问题实例的特征无关。
        
算法时间复杂度的本质是算法的执行时间，也就是算法中所有语句的频度之和。语句频度就是语句的执行次数，它与算法求解问题的规模大小息息相关。

运行时间与时间复杂度：
运行时间随着输入量增大而增大，复杂度越高，运行时间增加速度越快。
一般计算的时候认为计算机1s可以进行10^9次运算，那么输入数量当n=1000时，复杂度n^3的程序需要运行1s。而复杂度log n 的只需要极少的时间（不到1毫秒）
```

##  渐近时间复杂度 

```c++
（一） 大O记号 
如果存在两个正常数c 和 n0，使得对所有的n，n> n0 ，有
f(n)<= cg(n) 则有 f(n)=O(g(n))。
即函数f(n)当n充分大时上有界，且 g(n)是它的一个上界，也称f(n)的阶不高于g(n)的阶。


渐近时间复杂性：
   使用大O记号表示的算法的时间复杂性，称为算法的渐近时间复杂性。  

在大O记号下，可用程序步来估计算法的执行时间。
    很多情况下，可以通过考察一个算法中的关键操作（关键操作被认为是一个程序步）的执行次数来计算算法的渐近时间复杂性。

---渐进和时间复杂的区别
假设对于给定的算法，目前问题规模为n，则语句频度可以表示成一个关于问题规模的函数 T(n)，那么算法时间复杂度也就可以用T(n)表示，其含义是算法在输入规模为n时的运行时间。
当问题规模很大时，精确的计算T(n)是很难实现而且也是没有必要的。对于算法时间性能的分析无需非要得到时间复杂度T(n)的精确值，它的变化趋势和规律也能清楚地反映算法的时间耗费。基于此，引入了渐进时间复杂度作为时间性能分析的依据，它的含义就是：在问题规模 n趋于无穷大时算法时间复杂度T(n)的渐进上界，即函数 T(n)的数量级(阶)。

算法时间复杂度和渐进算法时间复杂度:
在实际的算法分析过程中是不予区分的，渐进时间复杂度可以简称为时间复杂度，记为T(n)=O(f(n))。其中，通过统计算法中基本操作重复执行的次数就可近似地得到算法的执行效率，用O(n)表示，称为时间复杂度。    
```



常见的渐近时间复杂性从小到大排列有：
O(1)< O(log2 n) < O(n)< O(nlog2 n)< O(n2)< O(n**3)<o(2^n)











大O表示法中都是以logn/log2  = 以log2为底数

![O表示法](/images/posts/dataStructure/O表示法.png)

![O表示法](../images/posts/dataStructure/O表示法.png)



```
Are we out of Numbers?	我们的人数不够了吗?
Get a number randomly from the available numbers	从可用的数字中随机抽取一个数字
Does it conflict?	冲突吗?
Use it!	使用它!
go forward 1 square	向前走1平方
Replenish this squares numbers and go back 1 square	补充这个平方数，回到1
Remove from available numbers for this square	从此方块的可用号码中移除
```



```flow
st=>start: 开始:>https://fibncci.github.io
e=>end

op1=>operation: 从可用的数字中随机抽取一个数字1|past
op2=>operation: 使用他2|current
sub1=>subroutine: 使用它2|current
op3=>operation: 补充这个平方数，回到1|current
op4=>operation: 从此方块的可用号码中移除|current
op5=>operation: 向前走1的平方

cond1=>condition: 我们的人数不够了吗?
cond2=>condition: 对吗？

io1=>inputoutput: 继续循环

st->cond1


cond1(yes)->op3->io1->
cond1(no)->op1->cond2

cond2(no)->sub1->op5
cond2(yes)->op4
```





## 时间复杂度

**算法的时间复杂度，用来度量算法的运行时间，记作: T(n) = O(f(n))。它表示随着 输入大小n 的增大，算法执行需要的时间的增长速度可以用 f(n) 来描述。**

f(n) 的增长速度是大于或者等于 T(n) 的，即T(n) = O(f(n))，所以我们可以用 f(n) 的增长速度来度量 T(n) 的增长速度，所以我们说这个算法的时间复杂度是 O(f(n))。



## 计算时间复杂度

```python

# 这个方法需要执行 2 次运算
def void():
    for i  in range(1):
        print('hello,worid',end='') #需要执行1次
    return 0                 # #需要执行1次
void() #hello,worid 0




```

```c
int aFunc(void) {
    printf("Hello, World!\n");      //  需要执行 1 次
    return 0;       // 需要执行 1 次
}
--------------
#include <stdio.h>
int main(int argc, char const *argv[])
{
        printf("hello，world\n");
        return 0;
}
```



```
# 这个方法需要执行 2n+1 次运算

def aFun(n):
    for i in range(n):     #需要执行n次
        print('hello,worid',end='') #需要执行n次
    return 0;   #需要执行1次
aFun(4)

# hello,woridhello,woridhello,woridhello,worid
# 0
```



```c
int aFunc(int n) {
    for(int i = 0; i<n; i++) {         // 需要执行 (n + 1) 次
        printf("Hello, World!\n");      // 需要执行 n 次
    }
    return 0;       // 需要执行 1 次
}
```



```
比如
f(n) 的增长速度是大于或者等于 T(n) 的，即T(n) = O(f(n))，所以我们可以用 f(n) 的增长速度来度量 T(n) 的增长速度，所以我们说这个算法的时间复杂度是 O(f(n))。

比如
T(n) = n^3 + n^2 + 29，此时时间复杂度为 O(n^3)。

比如
T(n) = 3n^3，此时时间复杂度为 O(n^3)。
```

**综合起来：如果一个算法的执行次数是 T(n)，那么只保留最高次项，同时忽略最高项的系数后得到函数 f(n)，此时算法的时间复杂度就是 O(f(n))。为了方便描述，下文称此为 大O推导法。**

**时间复杂度分析的基本策略是：从内向外分析，从最深层开始分析。如果遇到函数调用，要深入函数进行分析。**







## 例1.单循环O(n)

```python
# 单循环 O(n×m) ,循环体的时间复杂度为 O(n),循环次数为 m
# 时间复杂度为 O(n × 1)，即 O(n)

def aFun(n):
    for i in range(n): # 循环次数为 n
        print('hi') #循环体时间复杂度为 O(1)
aFun(3)

# hi
# hi
# hi
```

```c
void aFunc(int n) {
    for(int i = 0; i < n; i++) {         // 循环次数为 n
        printf("Hello, World!\n");      // 循环体时间复杂度为 O(1)
    }
}

#include <stdio.h>
int main(int argc, char const *argv[])
{

for(int i = 0;i<3;i++){
        printf("nihao\n" );
}
return 0;
}


```





## 例2.多循环 O(n^2)

```
# 多循环 ：循环体的时间复杂度为 O(n)，各个循环的循环次数分别是a, b, c...，
# 则这个循环的时间复杂度为 O(n×a×b×c...)。分析的时候应该由里向外分析这些循环。
# 时间复杂度为 O(n × n × 1)，即 O(n^2)

def aFun(n):
    for i in range(n):#循环次数为 n
        for j in range(n):#循环次数为 n
            print('hi',end=',');#循环体时间复杂度为 O(1)
aFun(3)
#hi,hi,hi,hi,hi,hi,hi,hi,hi,

```



```c
void aFunc(int n) {
    for(int i = 0; i < n; i++) {         // 循环次数为 n
        for(int j = 0; j < n; j++) {       // 循环次数为 n
            printf("Hello, World!\n");      // 循环体时间复杂度为 O(1)
        }
    }
}
```



## 3顺序执行 O(n^2)

```
# 对于顺序执行 的语句或者算法，总的时间复杂度 等于 其中最大的时间复杂度
# 时间复杂度为 max(  O(n^2), O(n)  )
# 即 O(n^2)。
def aFun(n):
    #第一部分时间复杂度为 O(n^2)
    for i in range(n):
        for j in range(n):
               
            print('hhe',end='')
    for j in range(n): #第二部分时间复杂度为 O(n)
        print('ss')

aFun(3)

# hhehhehhehhehhehhehhehhehhess
# ss
# ss
```



```c
void aFunc(int n) {
    // 第一部分时间复杂度为 O(n^2)
    for(int i = 0; i < n; i++) {
        for(int j = 0; j < n; j++) {
            printf("Hello, World!\n");
        }
    }
    // 第二部分时间复杂度为 O(n)
    for(int j = 0; j < n; j++) {
        printf("Hello, World!\n");
    }
}
```





## 4条件判断O(n^2)

```
# 条件判断语句，总的时间复杂度等于其中 时间复杂度最大的路径 的时间复杂度。
# 时间复杂度为 max(O(n^2), O(n))，即 O(n^2)
# 时间复杂度分析的基本策略是：
# 从内向外分析，从最深层开始分析。如果遇到函数调用，要深入函数进行分析。
def aFun(n):
    if n> 0:
        for i in range(n):
            for j in range(n):
                print('cc',end = ',')
    else:
        for j in range(n):
            print('ddd',end= '.')
aFun(2)

# cc,cc,cc,cc,
```





```c
void aFunc(int n) {
    if (n >= 0) {
        // 第一条路径时间复杂度为 O(n^2)
        for(int i = 0; i < n; i++) {
            for(int j = 0; j < n; j++) {
                printf("输入数据大于等于零\n");
            }
        }
    } else {
        // 第二条路径时间复杂度为 O(n)
        for(int j = 0; j < n; j++) {
            printf("输入数据小于零\n");
        }
    }
}
```



##  例1. O(log n) 

```python
# 假设循环次数为 t，则循环条件满足 2^t < n。
# 可以得出，执行次数t = log(2)(n)，即 T(n) = log(2)(n)，
# 可见时间复杂度为 O(log(2)(n))，即 O(log n)。
def aFun(n):
    count= 0
    for i in range(2,n):
        i *= 2
        #i=i*2
        print('哦哦哦',end= '')
        count += 1
    print(count)    
    
print(aFun(8))

# 哦哦哦哦哦哦哦哦哦哦哦哦哦哦哦哦哦哦6 None


#二分法的基本思想如下：假设数据是按升序排序的,对于给定值x,从序列的中间位置开始比较,如果当前位置值等于x,则查找成功；若x小于当前位置值,则在数列的前半段中查找；若x大于当前位置值则在数列的后半段中继续查找,...
```



```c
void aFunc(int n) {
    for (int i = 2; i < n; i++) {
        i *= 2;
        printf("%i\n", i);
    }
}
```





## 例2.指数级别O(2^n)-fib

```python
# 1  1 2 3 5 8 13
# T(0) = T(1) = 1，同时 T(n) = T(n - 1) + T(n - 2) + 1，
# 这里的 1 是其中的加法算一次执行。
# 显然 T(n) = T(n - 1) + T(n - 2) 是一个斐波那契数列，
# 通过归纳证明法可以证明，当 n >= 1 时 T(n) < (5/3)^n，
# 同时当 n > 4 时 T(n) >= (3/2)^n。

# 所以该方法的时间复杂度可以表示为 O((5/3)^n)，简化后为 O(2^n)。
# 可见这个方法所需的运行时间是以指数的速度增长的。
# 如果大家感兴趣，可以试下分别用 1，10，100 的输入大小来测试下算法的运行时间，
# 相信大家会感受到时间复杂度的无穷魅力。



def aFun(n):
    if n  <= 1 :
        return 1
        
    return aFun(n-1)+aFun(n-2)

print(aFun(1))  #1
print(aFun(10)) # 89
print(aFun(32)) #35245
# print(aFun(100))
# aFun(1000)
1
89
3524578
```

**c**

```c
long aFunc(int n) {
    if (n <= 1) {
        return 1;
    } else {
        return aFunc(n - 1) + aFunc(n - 2);
    }
}
```

**py**

```python
%%time 
def fibonacci_num(n):
    if n ==1:
        return 1
    if n ==2 :
        return 1
    return fibonacci_num(n-1)+fibonacci_num(n-2)
print(fibonacci_num(40))

#102334155
#CPU times: user 21.6 s, sys: 31.1 ms, total: 21.6 s
#Wall time: 21.7 s(我的电脑32g)（使用 系统  全部时间）

#102334155
#CPU times: user 25.8 s, sys: 8.2 ms, total: 25.9 s
#Wall time: 25.9 s（天池16g）
```

```python
%%time 

def fibonacci_num(n):
    if n == 1:
        return 1 
    if n==2 :
        return 1
    a = 1
    b= 1
    for i in range(n-2):
        b= a+b 
        
        a = b-a
        
    return b 
print(fibonacci_num(40))

# 102334155
# CPU times: user 123 µs, sys: 17 µs, total: 140 µs
# Wall time: 100 µs = 0.0001s
```



fibonacci数列5种求解方法：

1.$$a^n$$减治法

 n为偶数： r = $a^{\frac{n}{2}}$

n为奇数： n-1为偶数 r = $$a^{\frac{n-1}{2}}$$ 每次减半 $a^n$的 O(lgn) =n



2.求解通项公式：

f(n) =f(n-1)+ f(n-2)   ;  $x^2$ =x+1 ==>{$x_1$= $\frac{1+\sqrt{5}}{2}$  ;$x_2$= $\frac{1-\sqrt{5}}{2}$}

$f_n$ = $a_1x_1^n+a_2x_2^n$   ==> 
$$
\begin{cases}
f(0)= 0\\
f(1)=1\\
\end{cases}
$$
$\begin{cases} a_1 = \frac{1}{\sqrt{5}}\\  a_2 = -\frac{1}{\sqrt{5}}\\ \end{cases}$ ==>$ f_n$ = $\frac{1}{\sqrt{5}}[(\frac{1+\sqrt{5}}{2})^n-(\frac{1-\sqrt{5}}{2})^n]$ 



3.查表法：空间换时间

return return[n]===>O[1]

4.正推O[n]

a[n] =0 ;  a[1] = 1

for  a[n] = a [i-1]+a[i+1]

5.递归法

f(45) 跑死机 

```python
%%time 
def fibonacci_num(n):
    if n ==1:
        return 1
    if n ==2 :
        return 1
    return fibonacci_num(n-1)+fibonacci_num(n-2)
print(fibonacci_num(45))
1134903170
CPU times: user 3min 54s, sys: 307 ms, total: 3min 55s
Wall time: 3min 55s
```



## CPU时间

进程时间也称CPU时间，用以度量进程使用的中央处理器资源。进程时间以时钟嘀嗒计算，

实际时间（Real），实际时间指实际流逝的时间；

用户时间和系统时间 指特定进程使用的CPU时间：用户CPU时间（User），系统CPU时间（Sys）

- real time是从进行开始执行到完成所经历的墙上时钟时间（wall clock）时间，包括其他进程使用的时间片（time slice）和本进程耗费在阻塞（如等待I/O操作完成）上的时间。
- user time是进程执行用户态代码（内核外）耗费的CPU时间，仅统计该进程执行时实际使用的CPU时间，而不计入其他进程使用的时间片和本进程阻塞的时间
- sys time 是该进程在内核态运行所耗费的CPU时间，即内核执行系统调用所使用的CPU时间



CPU总时间（user + sys）是CPU执行用户进程操作和内核（代表用户进程执行）系统调用所耗时间的总和，即该进程（包括线程和子进程）所使用的实际CPU时间。若程序循环遍历数组，则增加用户CPU时间；若程序执行exec或fork等系统调用，则增加系统CPU时间。



在多核处理器机器上，若进程含有多个线程或通过fork调用创建子进程，则实际时间可能小于CPU总时间，因为不同线程或进程可并行执行，但其时间会计入主进程的CPU总时间。若程序在某段时间处于等待状态而并未执行，则实际时间可能大于CPU总时间：

1. real < CPU  表明进程为计算密集型（CPU bound），利用多核处理器的并行执行优势
2. real ≈ CPU  表明进程为计算密集型，未并行执行
3. real > CPU  表明进程为I/O密集型 （I/O bound），多核并行执行优势并不明显