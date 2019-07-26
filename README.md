>>2018/04/16
# 每天都要有Get的感觉
## Scala的学习之路， 加油 ！！！

### Part1
**1、学习Scala的原因**:
```
Spark是新一代内存级大数据计算框架，是大数据的重要内容
Spark就是使用Scala编写的。因此为了更好的学习Spark，需要掌握Scala这门语言

Scala是Scalable Language的简写， 十一么多范式(范式/编程方式[面向对象/函数式编程]的编程语言)

Spark的兴起带动了Scala语言的发展

Pizza和Scala极大地推动了Java编程语言的发展
jdk5.0的泛型,for循环增强,自动类型转换等都是从Pizza引入的新特性。
jdk8.0的类型推断, Lambda表达式就是从Scala引入的特性。 
```

### Part2
**2、java/scala/jvm的关系**
```
java代码 > javac编译器 > 得到.class字节码文件 > 将字节码文件放到JVM(JVM for windows / linux / unix)上运行 > 跨平台
Scala能使用Java的部分语法
Scala有自己特有的语法
Scala增加了函数式编程 / 偏函数 / 函数的柯里化 / 高阶函数 / 将函数作为参数传递
Scala对Java的类进行了包装
Scala代码 > Scalac编译器 > 得到.class字节码文件 > 将字节码文件放到JVM中运 > 跨平台
```

### Part3
**Scala**

### Part4
**Scala的特点:**
```
Scala是一门以Java虚拟机(JVM)为运行环境并将 面向对象 和 函数式编程 的最佳特性结合在一起的静态类型编程语言
1）Scala是一门多范式(multi-paradigm)的编程语言, Scala支持面向对象和函数式编程
2）Scala源代码(.scala)会被编译成Java字节码(.class),然后运行于JVM之上, 并可以调用现有的Java类库，实现两种语言的无缝对接
3）Scala单作为一门语言来看，非常的简洁高效 (舍弃了三元运算 ++ -- 等)
4）Scala的设计者式参考了Java的设计思想，可以说Scala是源于Java
```

### Part5
**Windows下搭建Scala开发环境**
```
1-Scala运行需要Java运行时库， 安装Scala需要首先安装JVM虚拟机并配置好环境变量, 推荐安装JDK1.8
2-http://www.scala-lang.org 不同系统选择不同版本
```

### Part6
**Linux下搭建Scala开发环境**
```
scala
```

### Part7
**Scala的开发工具**
```
IEDA(推荐)
Eclipse

默认情况下, Scala不支持Scala的开发, 需要在IDEA中安装Scala插件
```

### Part8
**Scala快速开发入门**

### Part9
**IDEA开发Scala入门**
```
IDEA创建maven项目, 项目中添加上Scala的SDK包,一般在本地安装了Scala, 将安装环境配置到IDEA中就可以了

```

### Part10
**Java模拟Scala运行流程机制**
```

```

### Part11
**Scala程序开发注意事项(重点)**
```
1 - Scala源文件以".scala"为扩展名
2 - Scala程序的执行入口时main()函数
3 - Scala语言严格区分大小写
4 - Scala犯方法由一条条语句构成, 每个语句后不需要分号(Scala语言会在每行后面自动加分号), 体现了Scala的简洁性
5 - 如果在同一行有多条语句, 除了最后一条语句不需要分号， 其他行语句需要分号

```
**Scala语言转义字符(escape char)**
```
1 - \t  : 一个制表符, 实现对齐的功能      println("name\tage")
2 - \n  : 换行符                      println("name\nage")
3 - \\  : 一个\                      println("C:\\xx")
4 - \"  : 一个"                      println("name\"age\"")
5 - \r  : 一个回车                    println("name\r age")
```

**Scala语言输出的三种方式**
``` scala
1 - 字符串通过 + 号连接 (似Java)
2 - printf用法 (似C)  字符串通过%传值  (%s-String %d-十进制)
3 - 字符串通过$引用 (似PHP)
```

### Part12
**Scala源码查看关联**
``` scala
在使用Scala过程中, 为了搞清楚Scala底层机制, 需要查看源码:
1 - 查看源码, 选择要查看的方法或者类, 输入ctrl + b   (将鼠标指针放到要查看的方法或类上, 输入ctrl + b)
2 - 关联源码, 将Attach Source指定到Scala的源代码解压路径下即可

```
### Part13
**注释(_comment_)**
```text
用于注释说明解释程序的文字就是注释, 注释提高了代码的可阅读性
注释是一个程序员必须要具有的良好编码习惯，将自己的思想通过注释先整理出来，再用代码去体现
Scala中的注释类型:
1 - 单行注释
2 - 多行注释
3 - 文档注释
    scaladoc -d 文档存放路径 类名称  (最好是直接切换到当前类的路径下)
    scaladoc -d E:\test\doc HelloScala.scala

```

### part14
**Scala规范的代码风格**
```text
正确的缩进和空白
1 - 使用一次tab操作, 实现缩进，默认整体向右移动, 使用shift+tab整体左移
2 - 使用ctrl + alt + l 格式化代码
3 - 运算符的两边习惯性加一个空格
4 - 一行代码最长不要超过80个字符，超过则使用换行展示，尽量保持格式优雅

```
**scala官方编程指南**
```text

```

### Part15 / 16 /17
**Scala变量**
```
变量是程序的基本组成单位,变量相当于内存中一个数据存储控件的表示, 你可以把变量看做是一个房间的门牌号，
通过门牌号我们可以找到房间, 而通过变量名可以访问到变量

声明/定义(指声明的同时给变量赋值)变量的关键字:
val: 不可变类型, 没有线程安全问题(推荐使用), 效率较高
var: 可变类型
再Scala中小数默认为Double类型，整数默认为Int类型
isInstanceOf判断数据类型

val | var 变量名 [:变量类型] = 变量值
注意:
1 - 声明变量时，类型可以省略(编译器自动推导,即类型推导)
2 - 类型确定后，就不能修改，说明Scala是强数据类型语言
3 - 再声明/定义一个变量时，可以使用var或者val来修饰, var修饰的变量可改变, val修饰的变量不能改变
4 - val修饰的变量再编译后，等同于加上final
5 - var修饰的对象引用可以改变,val修饰的则不可以改变, 但对象的状态(值)却是可以改变的。
6 - 声明变量时, 需要初始值

程序中 + 号的使用  (同Java)
1 - 当左右两边都是数值型时, 则做加法运算
2 - 当左右两边有一方为字符串, 则做拼接运算

```
**Scala数据类型**
```
1 - Scala与Java有着相同的数据类型,再Scala中数据类型都是对象, 也就是说Scala没有Java中的原生类型
2 - Scala数据类型分为两大类AnyVal(值类型) 和 AnyRef(引用类型), 注意: 不管是AnyVal还是AnyRef都是对象
3 - 相对于Java的类型系统, Scala要更复杂, 也正是这些复杂多变的类型系统才让面向对象编程和函数式编程完美的融合在一起
```
![Image](https://github.com/ReturnTears/allst-scala/blob/master/cimg/Scala_data_type.png)
```text
对上图的解释如下:
1 - 在Scala中有一个根类型, Any是所有类型的父类
2 - Scala中一切皆为对象,分为两大类型AnyVal(值类型),AnyRef(引用类型), 它们都是Any的子类型
3 - Null类型是Scala的特别类型,他只是一个值null, 它是bottom class, 是所有AnyRef类型的子类型
4 - Nothing类型也是bottom class, 它是所有类型的子类型, 在开发中可以将Nothing类型的值返回给任意变量或者函数, 在抛出异常时使用较多
5 - 在Scala中仍然遵守低精度向高精度的值自动转换(implicit conversion)隐式转换

```

### Part18  / 19
**Scala数据类型列表**
```
数据类型          |           描述
----            |           ----
Byte            |           8位有符号补码整数。整数区间为-128 ~ 127           -2的7次方 ~ 2的7次方 - 1
Short           |           16位有符号补码整数。整数区间为-32768 ~ 32767
Int             |           32位有符号补码整数。整数区间为-2147483648 ~ 2147483647
Long            |           64位有符号补码整数。整数区间为-9223372036864775808 ~ 9223372036854775807
Float           |           32位，IEEE754标准的单精度浮点数
Double          |           64位，IEEE754标准的双精度浮点数
Char            |           16位无符号Unicode，区间值为U+0000到U+FFFF
String          |           无符序列
Boolean         |           true或false
Unit            |           表示无值，和其他语言中void等同。用作不返回任何结果的方法的结果类型，Unit是一个实例值，写成()
Null            |           null
Nothing         |           Nothing类型在Scala的类层级的最低端，它是任何其他类型的子类型
Any             |           Any是所有其他类的超类
AnyRef          |           AnyRef类是Scala里所有引用类reference class的基类
```

补充:
最高位为符号为 **[0 1]**
·0表示整数
·1表示负数

**整数的使用细节:**
```
1 - Scala个整数类型有固定的表示范围和字段长度, 不受具体的OS的影响, 以保证Scala程序的可移植性性
2 - scala的整型 **常量/字面量** 默认为Int型， 声明Long型 常量/字面量 须后面加"l"或者“L”
3 - Scala程序中变量常声明为Int型, 除非不足以表示大数, 才使用Long
```
**浮点数使用细节:**
```
1 - 与整型类似,Scala浮点数类型也有固定的表示范围和字段长度,不受具体OS的影响
2 - Scala的浮点数类型**常量**为Double型, 声明Float型常量,须后加'f'或'F'
3 - 浮点型常量有两种表示方式:
    十进制数形式:5.12     512.0f  .512 (必须有小数点)
    科学计数法形式:5.12e2 = 5.12 × 10^2  5.12E-2 = 5.12 ÷ 10^2
4 - 通常情况下,应该使用Double型,因此他比Float型更精确(Float大致精确到小数点后7位)
```

### Part20
**字符类型(Char)**
```
字符类型可以表示单格字符,字符类型是Char,16位无符号Unicode(Unicode编码包含了assci码)字符(2个字节),区间值为U+0000到U+FFFF

字符类型使用细节:
1 - 字符常量是使用单引号('')括起来的单格字符; var c1 = 'a'
2 - Scala也允许使用转义字符'\'来将其后的字符转变为特殊字符型常量
3 - 可以直接给Char赋一个整数,然后输出时,回按照对应的Unicode字符输出['\u0061' 97]
4 - Char类型是可以进行运算的,详单与一个整数,因为它都对应有Unicode码

```
**注意:**
```
当把一个计算的结果赋值一个变量,则编译器会进行类型转换及判断(即会查看范围+类型)
当把一个字面量赋值一个变量,则编译器会进行数值范围判断
```

### Part21
**布尔类型:Boolean**
```
基本介绍:
1 - 布尔类型也叫Boolean类型, Boolean类型数据只允许取值true和false
2 - Boolean类型占1个字节
3 - Boolean类型适用于逻辑运算, 一般用于程序流程控制
> if条件控制语句
> while循环控制语句
> do-while循环控制语句
> for循环控制语句

```

**Unit类型 Null类型 Nothing类型**
```
使用细节和注意事项:
1 - Null类型只有一个实例对象,null,类似于Java的null引用.null可以赋值给任意引用类型(AnyRef),但是不能赋值给值类型(AnyVal)
2 - Unit类型用来标识过程,也就是没有明确返回值的函数.由此可见,unit类似于Java的void.Unit只有一个实例,(),这个实例也没有实质的意义
3 - Nothing,可以作为没有正常返回值的方法的返回值类型,非常直观的告诉你这个方法不会正常返回,而且由于Nothing是其他任意类型的子类,他还能跟要求返回值的方法兼容
```

### Zuoye Page
```text
1 - 在Scala REPL(Read evaluateion print loop)中,计算3的平方根,然会再对该值求平方, 这个结果和3相差多少?
    scala> var a = 3
    a: Int = 3
    
    scala> import scala.math
    import scala.math
    
    scala> val b = math.sqrt(a)
    b: Double = 1.7320508075688772
    
    scala> val c = b * b
    c: Double = 2.9999999999999996
    
    scala> val d = c - a
    d: Double = -4.440892098500626E-16
    
2 - Scala语言的sdk是什么?
    开发工具包

3 - Scala环境变量配置及其作用
    注意Windows和LInux下的环境配置区别
    作用是方便开发和使用

4 - Scala程序的编写,编译,运行各个步骤是什么? 能否一步执行?
    
    
5 - Scala程序编写的规则
    同Java, 可以不带分号

6 - 简述: 在配置环境\编译\运行各个步骤中常见错误
    

7 - 如何检测一个变量是val还是var?  
    思路:分别定义一个val和var变量, 重新赋值成功的是var变量, 不能重新赋值的是val变量
    isInstanceOf


8 - Scala允许你用数字去乘一个字符串,去REPL中试一下"crazy" * 3? 这个步骤做什么?再Scaladoc中如何找到这个操作?
    scala> val e = "crezy"
    e: String = crezy
    
    scala> e * 3
    res0: String = crezycrezycrezy

9 - 10 max 2的含义是什么? max方法定义下那个类下?
    scala> 10 max 2
    res1: Int = 10
    或者
    scala> 10.max(2)
    返回两个数的最大值
    max方法定义在RichInt, Int
    
10 - length计算2的1024次方(使用BigInt计算)
    scala> val a = BigInt(2)
    a: scala.math.BigInt = 2
    
    scala> a.pow(1024)
    res0: scala.math.BigInt = 179769313486231590772930519078902473361797697894230657273430081157732675805500963132708477322407536021120113879871393357658789768814416622492847430639474124377767893424865485276302219601246094119453082952085005768838150682342462881473913110540827237163350510684586298239947245938479716304835356329624224137216

11 - 在Scala中如何获取字符串"Hello"的首字符和尾字符
    Java,JavaScript可以使用substring
    scala> val b = "Hello"
    b: String = Hello
    
    scala> b.take(1)
    res1: String = H
    
    scala> "Hello"(0)
    res4: Char = H
    
    scala> b.reverse.take(1)
    res2: String = o
    
    scala> b.takeRight(1)
    res3: String = o

```

### Part24
**值类型转换**
```
自动类型转换细节说明:
1 - 有多种类型的数据混合运算时,系统首先会自动将所有数据转换成容量最大的那种数据类型,然后在进行计算
2 - 当我们把精度(容量)大的数据类型赋值给精度(容量)小的数据类型时就会报错,反之,就会进行自动类型转换
3 - (byte,short)和char之间不会相互转换,(byte和short可以)
4 - byte,short,char它们三者可以计算,在计算时首先转换为int类型
5 - 自动提升原则, 表达式结果的类型自动提升为操作数中最大的类型
```
**高级隐式转换和隐式函数**
```
todo
```
**强制类型转换**
```
自动类型转换的逆过程,将容量大的数据类型转换为容量小的数据类型,使用时需要加上强制类型转换函数,
但可能造成精度降低或溢出, 格外注意
强制类型转换细节说明:
1 - 当进行数据的从大到小,就需要使用强制类型转换
2 - 强制符号只针对于最近的操作数有效,往往会使用小括号提升优先级
    val num1:Int = 10 * 3.5.toInt + 6 * 1.5.toInt   // 36
    val num2:Int = (10 * 3.5 + 6 * 1.5).toInt       // 44
3 - Char类型可以保持int的常量值,但不能保存Int的变量值,需要强转
4 - Byte和Short类型在进行运算时,当作int类型处理
```

### 快捷键  shortcut key
```text
格式化文档:
1 - ctrl + alt + l  格式化代码

```

### REPL常用命令
```text
:q  -  退出Scala REPL

```


