

#  Java基础





## 一：Java语言概述

#### 文章目录

•01、 软件开发介绍••1.1、常用的DOS命令•02、计算机编程语言介绍•03、 Java语言概述••3.1、Java简史•3.2、Java技术体系平台•04、 Java程序运行机制及运行过程••4.1、Java两种核心机制•05、Java语言的环境搭建•06、 开发体验—HelloWorld•07、 常见问题及解决方法•08、 注释(comment)•09、小结第一个程序

## 01、 软件开发介绍

•软件开发软件，即一系列按照特定顺序组织的计算机数据和指令的集合。**软件有系统软件和应用软件之分**。•人机交互方式•**图形化界面**(Graphical User Interface `GUI`)这种方式简单直观，使用者易于接受，容易上手操作。•**命令行方式**(Command Line Interface `CLI`)：需要有一个控制台，输入特定的指令，让计算机完成一些操作。较为麻烦，需要记录住一些命令。

> **Pascal之父Nicklaus Wirth：“Algorithms+DataStructures=Programs”**

### 1.1、常用的DOS命令

•⊞+R，一起按下，输入cmd，可以打开dos界面。•dir :列出当前目录下的文件以及文件夹•md:创建目录•rd :删除目录•cd:进入指定目录•cd… : 退回到上一级目录•cd:退回到根目录•del :删除文件•exit : 退出dos 命令行•补充：echo javase>1.doc•常用快捷键•← →：移动光标•↑↓：调阅历史操作命令•Delete和Backspace：删除字符•注意：在输入dos命令时，要是用英文输入，所有标点符号都是英文。

## 02、计算机编程语言介绍

•什么是计算机语言•语言：是人与人之间用于沟通的一种方式。•例如：中国人与中国人用普通话沟通。而中国人要和英国人交流，就要学习英语。•计算机语言：人与计算机交流的方式。•如果人要与计算机交流，那么就要学习计算机语言。计算机语言有很多种。如：C ,C++,Java,PHP,Kotlin，Python，Scala等。•第一代语言•机器语言：指令以二进制代码形式存在。•第二代语言•汇编语言：使用助记符表示一条机器指令。•第三代语言：高级语言•C、Pascal、Fortran面向过程的语言•C++面向过程/面向对象•Java跨平台的纯面向对象的语言•.NET跨语言的平台•Python、Scala…•面向过程：例如张三打篮球，他打篮球的全部过程(拿球、传球、投篮……)。•面向对象：人的对象，人的运动的动作，运动的器械这三个对象，实例化一个张三的对象，对象有一个打篮球的动作，器械是篮球。•面向对象能更好的在抽象的层面分析问题，在程序实现跨越极大的赋予之前的代码。这些是面向过程编程极难实现的。

## 03、 Java语言概述

•是**SUN**(Stanford University Network，斯坦福大学网络公司) **1995年**推出的一门高级编程语言。•是一种面向Internet的编程语言。Java一开始富有吸引力是因为Java程序可以在Web浏览器中运行。这些Java程序被称为Java小程序（applet）。applet使用现代的图形用户界面与Web用户进行交互。applet内嵌在HTML代码中。•随着Java技术在web方面的不断成熟，已经成为Web应用程序的首选开发语言。**后台开发：Java、PHP、Python、Go、Node.js**

### 3.1、Java简史

•1991年Green项目，开发语言最初命名为Oak (橡树)•1994年，开发组意识到Oak 非常适合于互联网•1996年，发布JDK 1.0，约8.3万个网页应用Java技术来制作•1997年，发布JDK 1.1，JavaOne会议召开，创当时全球同类会议规模之最•1998年，发布JDK 1.2，同年发布企业平台J2EE•1999年，Java分成J2SE、J2EE和J2ME，JSP/Servlet技术诞生•2004年，发布里程碑式版本：**JDK 1.5，为突出此版本的重要性，更名为JDK 5.0**•2005年，J2SE -> JavaSE，J2EE -> JavaEE，J2ME -> JavaME•2009年，Oracle公司收购SUN，交易价格74亿美元•2011年，发布JDK 7.0•**2014年，发布JDK 8.0，是继JDK 5.0以来变化最大的版本**•2017年，发布JDK 9.0，最大限度实现模块化•2018年3月，发布JDK 10.0，版本号也称为18.3•2018年9月，发布JDK 11.0，版本号也称为18.9•2019年3月20日，Java SE 12 发布。Java 12是短期支持版本。•2019年9月23日，Java SE 13发布，此版本中添加了“文本块”，文本块是一个多行字符串文字，避免对大多数转义序列的需要，以可预测的方式自动格式化字符串，并在需要时让开发人员控制格式。

### 3.2、Java技术体系平台

> 1、**JavaSE(Java Standard Edition)标准版**

支持面向桌面级应用（如Windows下的应用程序）的Java平台，提供了完整的Java核心API，此版本以前称为J2SE

> 2、**JavaEE(Java Enterprise Edition)企业版**

是为开发企业环境下的应用程序提供的一套解决方案。该技术体系中包含的技术如:Servlet 、Jsp等，主要针对于Web应用程序开发。版本以前称为J2EE

> 3、Java ME(Java Micro Edition)小型版

支持Java程序运行在移动终端（手机、PDA）上的平台，对Java API有所精简，并加入了针对移动终端的支持，此版本以前称为J2ME

> 4、Java Card

支持一些Java小程序（Applets）运行在小内存设备（如智能卡）上的平台

> 5、从Java的应用领域来分，Java语言的应用方向主要表现在以下几个方面：

•企业级应用：主要指复杂的大企业的软件系统、各种类型的网站。Java的安全机制以及它的跨平台的优势，使它在分布式系统领域开发中有广泛应用。应用领域包括金融、电信、交通、电子商务等。•Android平台应用：Android应用程序使用Java语言编写。Android开发水平的高低很大程度上取决于Java语言核心能力是否扎实。•大数据平台开发：各类框架有Hadoop，spark，storm，flink等，就这类技术生态圈来讲，还有各种中间件如flume，kafka，sqoop等等，这些框架以及工具大多数是用Java编写而成，但提供诸如Java，scala，Python，R等各种语言API供编程。•移动领域应用：主要表现在消费和嵌入式领域，是指在各种小型设备上的应用，包括手机、PDA、机顶盒、汽车通信设备等。

> Java主要特性

•Java语言是易学的。Java语言的语法与C语言和C++语言很接近，使得大多数程序员很容易学习和使用Java。•Java语言是强制面向对象的。Java语言提供类、接口和继承等原语，为了简单起见，只支持类之间的单继承，但支持接口之间的多继承，并支持类与接口之间的实现机制（关键字为implements）。•Java语言是分布式的。Java语言支持Internet应用的开发，在基本的Java应用编程接口中有一个网络应用编程接口（java net），它提供了用于网络应用编程的类库，包括URL、URLConnection、Socket、ServerSocket等。Java的RMI（远程方法激活）机制也是开发分布式应用的重要手段。•Java语言是健壮的。Java的强类型机制、异常处理、垃圾的自动收集等是Java程序健壮性的重要保证。对指针的丢弃是Java的明智选择。•Java语言是安全的。Java通常被用在网络环境中，为此，Java提供了一个安全机制以防恶意代码的攻击。如：安全防范机制（类ClassLoader），如分配不同的名字空间以防替代本地的同名类、字节代码检查。•Java语言是体系结构中立的。Java程序（后缀为java的文件）在Java平台上被编译为体系结构中立的字节码格式（后缀为class的文件），然后可以在实现这个Java平台的任何系统中运行。•Java语言是解释型的。如前所述，Java程序在Java平台上被编译为字节码格式，然后可以在实现这个Java平台的任何系统的解释器中运行。先编译后解释。•Java是性能略高的。与那些解释型的高级脚本语言相比，Java的性能还是较优的。•Java语言是原生支持多线程的。在Java语言中，线程是一种特殊的对象，它必须由Thread类或其子（孙）类来创建。

## 04、 Java程序运行机制及运行过程

•特点一：面向对象•两个基本概念：类、对象•**三大特性：封装、继承、多态**•特点二：健壮性•吸收了C/C++语言的优点，但去掉了其影响程序健壮性的部分（如指针、内存的申请与释放等），提供了一个相对安全的内存管理和访问机制•特点三：跨平台性•跨平台性：通过Java语言编写的应用程序在不同的系统平台上都可以运行。“Write once , Run Anywhere”•原理：只要在需要运行java 应用程序的操作系统上，先安装一个Java虚拟机(JVM Java Virtual Machine) 即可。由JVM来负责Java程序在该系统中的运行。

### 4.1、Java两种核心机制

> 1、Java虚拟机(Java VirtalMachine)

•JVM是一个虚拟的计算机，具有指令集并使用不同的存储区域。负责执行指令，管理数据、内存、寄存器。•对于不同的平台，有不同的虚拟机。•只有某平台提供了对应的java虚拟机，java程序才可在此平台运行。[外链图片转存失败,源站可能有防盗链机制,建议将图片保存下来直接上传

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/769975360ad2e28fee20163e9f6ba156.png#pic_center)在这里插入图片描述

•Java虚拟机机制屏蔽了底层运行平台的差别，实现了“一次编译，到处运行”。[外链图片转存失败,源站可能有防盗在这里插入!链机制,建描述]议将图片上https://传(imblog-dnimg.cn/img_convert/UEET6e8896a45811378ed13d38b7df66.png#pic_center344)(#pic_center)]



![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/5be62acd969e53f64d5334050b0d98ca.png#pic_center)在这里插入图片描述

> 2、垃圾收集机制(Garbage Collection)

•不再使用的内存空间应回收——垃圾回收。•在C/C++等语言中，由程序员负责回收无用内存。•Java 语言消除了程序员回收无用内存空间的责任：它提供一种系统级线程跟踪存储空间的分配情况。并在JVM空闲时，检查并释放那些可被释放的存储空间。•垃圾回收在Java程序运行过程中自动进行，程序员无法精确控制和干预。

**Java程序还会出现内存泄漏和内存溢出问题吗？Yes!**

## 05、Java语言的环境搭建

> 1、明确什么是JDK, JRE

•JDK(Java Development Kit Java开发工具包)•JDK是提供给Java开发人员使用的，其中包含了java的开发工具，也**包括了JRE。**所以安装了JDK，就不用在单独安装JRE了。其中的开发工具：编译工具(javac.exe) 打包工具(jar.exe)等。•JRE(Java Runtime Environment Java运行环境)•包括Java虚拟机(JVM Java Virtual Machine)和Java程序所需的核心类库等，**如果想要运行一个开发好的Java程序，计算机中只需要安装JRE即可。**

> 2、**简单而言，使用JDK的开发工具完成的java程序，交给JRE去运行。**

![null](https://i-blog.csdnimg.cn/blog_migrate/99164fd4afe6cb528b0e692530b5c921.png)

![null](https://i-blog.csdnimg.cn/blog_migrate/aea336a2f695f01c3160c477d13311f0.png)

•**JDK = JRE + 开发工具集（例如Javac编译工具等）**•**JRE = JVM + Java SE标准类库**

> 3、**官方网址：**

•下载JDK：www.oracle.com•java.sun.com•安装JDK1.傻瓜式安装，下一步即可。2.**建议：安装路径不要有中文或者空格等特殊符号。**3.如果操作系统是64位的，软件尽量选择支持64位的（除非软件本身不区分）。4.当提示安装JRE 时，正常在JDK安装时已经装过了，但是为了后续使用Eclipse等开发工具不报错，建议也根据提示安装JRE。

> 4、配置环境变量

•**path**：windows系统执行命令时要搜寻的路径。•在dos命令行中敲入javac，出现错误提示：

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/06cb918dec481e39307082ac9360fa8f.png#pic_center)在这里插入图片描述

•错误原因：当前执行的程序在当前目录下如果不存在，windows系统会在系统中已有的一个名为path的环境变量指定的目录中查找。如果仍未找到，会出现以上的错误提示。所以进入到jdk安装路径\bin目录下，执行javac，会看到javac参数提示信息。![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/b18ab9061c0433ab6fcdd06fd7d18748.png#pic_center)在这里插入图片描述



> 5、**每次执行java 的工具都要进入到bin目录下，非常麻烦。可不可以在任何目录下都可以执行java的工具呢？**

•根据windows系统在查找可执行程序的原理，可以将java工具所在路径定义到path 环境变量中，让系统帮我们去找运行执行的程序。•配置方法：•我的电脑–属性–高级系统设置–环境变量•编辑path 环境变量，在变量值开始处加上java工具所在目录，后面用“; ”和其他值分隔开即可。•打开DOS命令行，任意目录下敲入javac。如果出现javac的参数信息，配置成功。•注：具体操作流程，参看https://www.yuque.com/nizhegechouloudetuboshu/library/rc1889

![null](https://i-blog.csdnimg.cn/blog_migrate/8ccf1ae7b4fec49ab69f708d244cec7c.png)



> 6、验证是否成功

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/2d8d5aed4fc0109728448266030b674a.png#pic_center)在这里插入图片描述

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/3aa96b45b29542b18f03d04a4c9be7e8.png#pic_center)在这里插入图片描述

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/cc64f82dc759cc751c565c7eb84de221.png#pic_center)在这里插入图片描述

> 7、选择合适的文本编辑器或IDE 开发

•eclipse——https://www.eclipse.org/downloads/packages/•IDEA——https://www.jetbrains.com/idea/download/•官网太慢，备用地址：链接：https://pan.baidu.com/s/1rnBuCPKCyunCTyNKoRY7YA，提取码：4x3d•安装步骤：https://www.yuque.com/nizhegechouloudetuboshu/library/rc1889。

## 06、 开发体验—HelloWorld

> 1、步骤：

1.将Java 代码**编写**到扩展名为.java 的文件中。

•选择最简单的编辑器：记事本。•敲入代码class Test{}将文件保存成Test.java，这个文件是存放java代码的文件，称为源文件。

> 2、**第一个Java程序**

```java
public class Test {

    public static void main(String[] args) {
    
        System.out.println("hello world");
    
    }

}    
```

> 1、通过javac命令对该java 文件进行**编译**。

![图片](https://i-blog.csdnimg.cn/blog_migrate/f869971602ea860780932e7ae0f57fb1.png)图片

•有了java源文件，通过编译器将其编译成JVM可以识别的字节码文件。•在该源文件目录下，通过javac编译工具对Test.java文件进行编译。•如果程序没有错误，没有任何提示，但在当前目录下会出现一个Test.class文件，该文件称为字节码文件，也是可以执行的java的程序。

> 2、通过java 命令对生成的class 文件进行**运行**。

•有了可执行的java程序(Test.class字节码文件)•通过运行工具java.exe对字节码文件进行执行。

![null](https://i-blog.csdnimg.cn/blog_migrate/becc6cc6be05988a91935c1aaba108a3.png)

•出现提示：缺少一个名称为main的方法。
![null](https://i-blog.csdnimg.cn/blog_migrate/60957de14b9445c330317306cd3675ef.png)•因为一个程序的执行需要一个起始点或者入口，所以在Test类中的加入**public static void main(String[] args){}**•对修改后的Test.java源文件需要重新编译，生成新的class文件后，再进行执行。•发现没有编译失败，但也没有任何效果，因为并没有告诉JVM要帮我们做什么事情，也就是没有可以具体执行的语句。•想要和JVM来个互动，只要在main方法中加入一句System.out.println(“Hello World");因为程序进行改动，所以再重新编译，运行即可。
![null](https://i-blog.csdnimg.cn/blog_migrate/15506368463c34344803b27d206acb8c.png)



## 07、 常见问题及解决方法

> 1、问题1

![null](https://i-blog.csdnimg.cn/blog_migrate/ef0b387109a10e9f2120ba6182bccafa.png)

•源文件名不存在或者写错•当前路径错误•后缀名隐藏问题

> 2、问题2

![null](https://i-blog.csdnimg.cn/blog_migrate/c4653f4e5e92aedefcb7b33ed94d3134.png)

•类文件名写错，尤其文件名与类名不一致时，要小心•类文件不在当前路径下，或者不在classpath指定路径下

> 3、问题3

![null](https://i-blog.csdnimg.cn/blog_migrate/9328b3af802198b81e9a7e99ddf8959b.png)

•声明为public的类应与文件名一致，否知编译失败

> 4、问题4

![null](https://i-blog.csdnimg.cn/blog_migrate/ae4467d30095505381b3526251befa0d.png)

•编译失败，注意错误出现的行数，再到源代码中指定位置改错

总结：学习编程最容易犯的错是**语法错误**。Java要求你必须按照语法规则编写代码。如果你的程序违反了语法规则，例如：忘记了分号、大括号、引号，或者拼错了单词，java编译器都会报语法错误。**尝试着去看懂编译器会报告的错误信息。**

## 08、 注释(comment)

•用于注解说明解释程序的文字就是注释。•Java中的注释类型：•单行注释•**格式：//注释文字**•多行注释•**格式：/\* 注释文字*/**•**注：对于单行和多行注释，被注释的文字，不会被JVM（java虚拟机）解释执行。**
**多行注释里面不允许有多行注释嵌**•**文档注释(java特有)**•**格式**：`/** * @author 指定java程序的作者** * @version 指定源文件的版本** */`**注释内容可以被JDK提供的工具javadoc所解析，生成一套以网页文件形式体现的该程序的说明文档。**

![null](https://i-blog.csdnimg.cn/blog_migrate/010e66c6c95b721d908aa6444b8c1f47.png)

•**提高了代码的阅读性；调试程序的重要方法。**•注释是一个程序员必须要具有的良好编程习惯。•将自己的思想通过注释先整理出来，再用代码去体现。



## 09、小结第一个程序

•Java源文件以“java”为扩展名。源文件的基本组成部分是类（class），如本例中的HelloWorld类。•Java应用程序的执行入口是main()方法。它有固定的书写格式：
**`public static void main(String[] args) {…}`**•Java语言严格区分大小写。•Java方法由一条条语句构成，每个语句以“;”结束。•大括号都是成对出现的，缺一不可。•**一个源文件中最多只能有一个public类。其它类的个数不限，如果源文件包含一个public类，则文件名必须按该类名命名**。



## 二：变量、标识符、保留字、变量

#### 文章目录

•01、关键字与保留字•02、标识符••2.1、什么是标识符（Identifier）•2.2、定义合法标识符规则【重要】•2.3、Java 中的名称命名规范•03、变量••3.1、变量的声明与使用•3.2、基本数据类型••3.2.1、整数类型：byte、short、int、long•3.2.2、浮点类型：float、double•3.2.3、字符类型：char•3.3.4、布尔类型：boolean•3.3、基本数据类型转换•3.3、字符串类型：String•3.4、强制类型转换•04、进制••4.1、进制与进制间的转换•4.2、二进制•4.3、进制间转化•其他

## 01、关键字与保留字

> 1、关键字(keyword)的定义和特点

•定义：被 Java 语言赋予了特殊含义，用做专门用途的字符串（单词）•特点：关键字中所有字母都为小写•官方地址： https://docs.oracle.com/javase/tutorial/java/nutsandbolts/\_keywords.html

![null](https://i-blog.csdnimg.cn/blog_migrate/78be6fe8dd9bcf95dcc6043edd3e09aa.png)



![null](https://i-blog.csdnimg.cn/blog_migrate/63b6eafcf4ffbf081d8476a0499809e6.png)

> 2、保留字(reserved word)

Java 保留字：现有 Java 版本尚未使用，但以后版本可能会作为关键字使用。自己命名标识符时要避免使用这些保留字 `goto、const`。

## 02、标识符

### 2.1、什么是标识符（Identifier）

•Java 对各种变量、方法和类等要素命名时使用的字符序列称为标识符•技巧：凡是自己可以起名字的地方都叫标识符。

### 2.2、定义合法标识符规则【重要】

1.**由 26 个英文字母大小写，0-9，_或$ 组成**2.**数字不可以开头。**3.**标识符不能包含空格。**4.**不可以使用关键字和保留字，但能包含关键字和保留字。**5.**Java 中严格区分大小写，长度无限制。**

### 2.3、Java 中的名称命名规范

> 1、Java 中的名称命名规范：

•**包名**：多单词组成时**所有字母都小写**：xxxyyyzzz•**类名**、接口名：多单词组成时，**所有单词的首字母大写：**XxxYyyZzz•**变量名**、方法名：多单词组成时，**第一个单词首字母小写，第二个单词开始每个单词首字母大写：xxxYyyZzz**•**常量名**：**所有字母都大写。多单词时每个单词用下划线连接：XXX_YYY_ZZZ**

> 2、注意点

•注意 1：在起名字时，为了提高阅读性，要尽量有意义，“见名知意”。•注意 2：java 采用 unicode 字符集，因此标识符也可以使用汉字声明，但是不建议使用。•更多细节详见《代码整洁之道》

## 03、变量

### 3.1、变量的声明与使用

> 1、变量的概念：

•内存中的一个存储区域；•该区域的数据可以在同一类型范围内不断变化；•变量是程序中最基本的存储单元。包含**变量类型、变量名和存储的值。**

> 2、变量的作用：

•用于在内存中保存数据。

> 3、使用变量注意：

•Java 中每个变量必须先声明，后使用；•使用变量名来访问这块区域的数据；•变量的作用域：其定义所在的一对{ }内；•变量只有在其作用域内才有效；•同一个作用域内，不能定义重名的变量；

> 4、声明变量

•语法：<数据类型> <变量名称>•例如：int var;

> 5、变量的赋值

•语法：<变量名称> = <值>•例如：var = 10;

> 6、声明和赋值变量

•语法：<数据类型><变量名>= <初始化值>•例如：int var = 10

> 7、补充：变量的分类-按声明的位置的不同

•在方法体外，类体内声明的变量称为**成员变量**。•在方法体内部声明的变量称为**局部变量**。

![null](https://i-blog.csdnimg.cn/blog_migrate/29865b778f39a47e8e2c32fbc1cf7b0a.png)



> 8、注意：二者在初始化值方面的异同:

•同：都有生命周期•异：局部变量除形参外，需显式初始化。

### 3.2、基本数据类型

> 2、变量的分类-按数据类型

对于每一种数据都定义了明确的具体数据类型（强类型语言），在内存中分配了不同大小的内存空间。

![null](https://i-blog.csdnimg.cn/blog_migrate/e1c471200c6a0f35af578c9246ccd5e7.png)

#### 3.2.1、整数类型：byte、short、int、long

•Java 各整数类型有固定的表数范围和字段长度，不受具体 OS 的影响，以保证 java 程序的可移植性。•**java 的整型常量默认为 int 型，声明 long 型常量须后加‘l’或‘L’**•java 程序中变量通常声明为 int 型，除非不足以表示较大的数，才使用 long

| 类型  | 占用存储空间 | 表数范围               |
| ----- | ------------ | ---------------------- |
| byte  | 1字节=8bit位 | -128 ~ 127             |
| short | 2字节        | -2^15~ 2^15-1          |
| int   | 4字节        | -2^31~ 2^31-1 (约21亿) |
| long  | 8字节        | -2^63~ 2^63-1          |

•1MB = 1024KB 1KB= 1024B B= byte ? bit?•**bit: 计算机中的最小存储单位。byte:计算机中基本存储单元。**

```java
/*
Java定义的数据类型

一、变量按照数据类型来分：
    基本数据类型：
        整型：byte \ short \ int \ long
        浮点型：float \ double
        字符型：char
        布尔型：boolean

    引用数据类型：
        类：class
        接口：interface
        数组：array

二、变量在类中声明的位置：
        成员变量 vs 局部变量
*/
class VariableTest1{
    public static void main(String[] args) {
        //1. 整型：byte(1字节=8bit) short(2字节） \ int (4字节）\ long(8字节)
        //① byte范围：-128 ~ 127

        byte b1 = 12;
        byte b2 = -128;
    //    b2 = 128; //编译不通过
        System.out.println(b1);
        System.out.println(b2);

        // ② 声明long型变量，必须以“1”或“L”结尾
        short s1 = 128;
        int i1 = 12345;
        long l1 = 345678586;
        System.out.println(l1);
    }
}
```

#### 3.2.2、浮点类型：float、double

•与整数类型类似，Java 浮点类型也有固定的表数范围和字段长度，不受具体操作系统的影响。•浮点型常量有两种表示形式：•十进制数形式：如：5.12 512.0f .512 (必须有小数点）•科学计数法形式:如：5.12e2 512E2 100E-2•float:单精度，尾数可以精确到7位有效数字。很多情况下，精度很难满足需求。•double:双精度，精度是float的两倍。通常采用此类型。•**Java 的浮点型常量默认为double型，声明float型常量，须后加‘f’或‘F’。**

| 类型         | 占用存储空间 | 表数范围               |
| ------------ | ------------ | ---------------------- |
| 单精度float  | 4字节        | -3.403E38 ~ 3.403E38   |
| 双精度double | 8字节        | -1.798E308 ~ 1.798E308 |

#### 3.2.3、字符类型：char

•char 型数据用来表示通常意义上“字符”(2字节)•Java中的所有字符都使用Unicode编码，故一个字符可以存储一个字母，一个汉字，或其他书面语的一个字符。•字符型变量的三种表现形式：•字符常量是用单引号(‘ ’)括起来的单个字符。例如：char c1 = ‘a’; char c2 = ‘中’; char c3 = ‘9’;•Java中还允许使用转义字符‘\’来将其后的字符转变为特殊字符型常量。例如：char c3 = ‘\n’; //’\n’表示换行符•直接使用Unicode值来表示字符型常量：‘\uXXXX’。其中，XXXX代表一个十六进制整数。如：\u000a 表示\n。•char类型是可以进行运算的。因为它都对应有Unicode码。

```java
/*
Java定义的数据类型

一、变量按照数据类型来分：

    基本数据类型：
        整型：byte \ short \ int \ long
        浮点型：float \ double
        字符型：char
        布尔型：boolean

    引用数据类型：
        类：class
        接口：interface
        数组：array

二、变量在类中声明的位置：
        成员变量 vs 局部变量
*/
class VariableTest1{
    public static void main(String[] args) {
        //2. 浮点型：float(4字节) \ double(8字节)
        //① 浮点型，表示带小数点的数值
        //② float表示数值的范围比long还大

        double d1 = 12.3;
        System.out.println(d1 +1);
        
        //定义float类型变量时，变量要以"f" 或"F"结尾
        float f1 = 12.3F;
        System.out.println(f1);

        //② 通常，定义浮点型变量时，使用double变量

        //3. 字符型：char(1字符=2字节)
        //① 定义char型变量，通常使用一对'' 
        char c1 = 'a';
        //编译不通过
        //c1 = 'AB';
        System.out.println(c1);

        char c2 = '1';
        char c3 = '中';
        char c4 = '&';
        System.out.println(c2);
        System.out.println(c3);
        System.out.println(c4);

        //② 表示方式：1.声明一个字符；2.转义字符；3.直接使用Unicode值来表示字符型常量
        char c5 = '\n';    //换行符
        c5 = '\t';    //制表符
        System.out.print("hello" + c5);
        System.out.println("world");

        char c6 = '\u0123';
        System.out.println(c6);
        
        char c7 = '\u0043';
        System.out.println(c7);
    }
}
```

> 了解：ASCII 码

•在计算机内部，所有数据都使用二进制表示。每一个二进制位（bit）有0 和1 两种状态，因此8个二进制位就可以组合出256 种状态，这被称为一个字节（byte）。一个字节一共可以用来表示256 种不同的状态，每一个状态对应一个符号，就是256 个符号，从0000000 到11111111。•ASCII码：上个世纪60年代，美国制定了一套字符编码，对英语字符与二进制位之间的关系，做了统一规定。这被称为ASCII码。ASCII码一共规定了128个字符的编码，比如空格“SPACE”是32（二进制00100000），大写的字母A是65（二进制01000001）。这128个符号（包括32个不能打印出来的控制符号），只占用了一个字节的后面7位，最前面的1位统一规定为0。•缺点：•不能表示所有字符。•相同的编码表示的字符不一样：比如，130在法语编码中代表了é，在希伯来语编码中却代表了字母Gimel(ג)。

> 了解：Unicode 编码

•乱码：世界上存在着多种编码方式，同一个二进制数字可以被解释成不同的符号。因此，要想打开一个文本文件，就必须知道它的编码方式，否则用错误的编码方式解读，就会出现乱码。•Unicode：一种编码，将世界上所有的符号都纳入其中。每一个符号都给予一个独一无二的编码，使用Unicode 没有乱码的问题。•Unicode 的缺点：Unicode 只规定了符号的二进制代码，却没有规定这个二进制代码应该如何存储：无法区别Unicode 和ASCII：计算机无法区分三个字节表示一个符号还是分别表示三个符号。另外，我们知道，英文字母只用一个字节表示就够了，如果unicode统一规定，每个符号用三个或四个字节表示，那么每个英文字母前都必然有二到三个字节是0，这对于存储空间来说是极大的浪费。

> 了解：UTF-8

•UTF-8 是在互联网上使用最广的一种Unicode 的实现方式。•UTF-8 是一种变长的编码方式。它可以使用1-6 个字节表示一个符号，根据不同的符号而变化字节长度。•UTF-8的编码规则：•对于单字节的UTF-8编码，该字节的最高位为0，其余7位用来对字符进行编码（等同于ASCII码）。•对于多字节的UTF-8编码，如果编码包含n 个字节，那么第一个字节的前n位为1，第一个字节的第n+1 位为0，该字节的剩余各位用来对字符进行编码。在第一个字节之后的所有的字节，都是最高两位为"10"，其余6位用来对字符进行编码。

#### 3.3.4、布尔类型：boolean

•boolean 类型用来判断逻辑条件，一般用于程序流程控制：•if条件控制语句；•while循环控制语句；•do-while循环控制语句；•for循环控制语句；•boolean类型数据只允许取值true和false，无null。•不可以使用0或非0 的整数替代false和true，这点和C语言不同。•Java虚拟机中没有任何供boolean值专用的字节码指令，Java语言表达所操作的boolean值，在编译之后都使用java虚拟机中的int数据类型来代替：true用1表示，false用0表示。———《java虚拟机规范8版》

```java
class VariableTest1{
    public static void main(String[] args) {
        //4. 布尔型：boolean
        //① 只能取两个值之一：true 、false
        //② 常常在条件判断、循环结构中使用
        boolean bb1 = true;
        System.out.println(bb1);

        boolean isMarried = true;
        if(isMarried){
            System.out.println("禁止入内！");
        }else{
            System.out.println("可以参观！");
        }
    }
}
```

### 3.3、基本数据类型转换

•自动类型转换：容量小的类型自动转换为容量大的数据类型。数据类型按容量大小排序为：

![null](https://i-blog.csdnimg.cn/blog_migrate/3e19215fffda29e8f3de4d28726ac01e.png)

•有多种类型的数据混合运算时，系统首先自动将所有数据转换成容量最大的那种数据类型，然后再进行计算。•**byte,short,char之间不会相互转换，他们三者在计算时首先转换为int类型**。•**boolean类型不能与其它数据类型运算**。•**当把任何基本数据类型的值和字符串(String)进行连接运算时(+)，基本数据类型的值将自动转化为字符串(String)类型**。



```java
/*
基本数据类型之间的运算规则：

前提：这里讨论只是7中基本数据类型变量的运算。不包含boolean类型的。
1. 自动类型提升：
    当容量小的数据类型的变量和容量大的数据类型的变量做运算时，结果自动提升为容量大的数据类型。
    char、byte、short-->int-->long-->float-->double

    特别的：当byte、char、short三种类型的变量做运算时，结果为int类型

2. 强制类型转换：
    
说明：此时容量大小指的是，表示数的范围的大和小。比如：float容量要大于long的容量
*/
class VariableTest2{
    public static void main(String[] args) {
        byte b1 = 2;
        int i1 = 129;
        //编译不通过
//        byte b2 = b1 + i1;
        int i2 = b1 + i1;
        long l1 = b1 + i1;
        System.out.println(i2);
        System.out.println(l1);

        float f = b1 + i1;
        System.out.println(f);
        //***************特别的**************************
        char c1 = 'a';    //97
        int i3 = 10;
        int i4 = c1 + i3;
        System.out.println(i4);

        short s2 = 10;
        //编译错误
//        char c3 = c1 + s2;
        
        byte b2 = 10;
//        char c3 = c1 + b2;    //编译不通过

//        short s3 = b2 + s2;    //编译不通过
        
//        short s4 = b1 + b2;    //编译不通过
    }
}
class VariableTest4{
    public static void main(String[] args){
        //1. 编码情况
        long l = 123456;
        System.out.println(l);
        //编译失败：过大的整数
        //long l1 = 452367894586235;
        long l1 = 452367894586235L;

        //**************************
        //编译失败
//        float f1 = 12.3;
        
        //2. 编码情况2:
        //整型变量，默认类型为int型
        //浮点型变量，默认类型为double型
        byte b = 12;
    //    byte b1 = b + 1;    //编译失败
        
    //    float f1 = b + 12.3;    //编译失败
    }
}
```

### 3.3、字符串类型：String

•**String不是基本数据类型，属于引用数据类型**•使用方式与基本数据类型一致。例如：String str= “abcd”;•一个字符串可以串接另一个字符串，也可以直接串接其他类型的数据。例如：

```java
/*
String类型变量的使用
1. String属于引用数据类型
2. 声明String类型变量时，使用一对""
3. String可以和8种基本数据类型变量做运算，且运算只能是连接运算；+
4. 运算的结果任然是String类型

*/
class StringTest{
    public static void main(String[] args){

        String s1 = "Good Moon!";

        System.out.println(s1);

        String s2 = "a";
        String s3 = "";

//        char c = '';    //编译不通过
        
        //*******************************
        int number = 1001;
        String numberStr = "学号:";
        String info = numberStr + number;    //连接运算
        boolean b1 = true;
        String info1 = info + true;
        System.out.println(info1);
    }
}
```

> 练习1

```java
String str1 = 4; //判断对错：no
String str2 = 3.5f + “”; //判断str2对错：yes
System.out.println(str2); //输出：”3.5”
System.out.println(3+4+“Hello!”); //输出：7Hello!
System.out.println(“Hello!”+3+4); //输出：Hello!34
System.out.println(‘a’+1+“Hello!”); //输出：98Hello!
System.out.println(“Hello”+‘a’+1); //输出：Helloa1
```

### 3.4、强制类型转换

•自动类型转换的逆过程，将容量大的数据类型转换为容量小的数据类型。使用时要加上强制转换符：()，但可能造成精度降低或溢出,格外要注意。•通常，字符串不能直接转换为基本类型，但通过基本类型对应的包装类则可以实现把字符串转换成基本类型。•如：`String a = “43”; inti= Integer.parseInt(a);`•`boolean`类型不可以转换为其它的数据类型。

> 练习2

判断是否能通过编译

```java
short s = 5;
s = s-2; //判断：no
byte b = 3;
b = b + 4;//判断：no
b = (byte)(b+4);//判断：yes
char c = ‘a’;
int i = 5;
float d = .314F;
double result = c+i+d; //判断：yes
byte b = 5;
short s = 3;
short t = s + b;//判断：no
```

## 04、进制

### 4.1、进制与进制间的转换

> 关于进制

•所有数字在计算机底层都以二进制形式存在。•对于整数，有四种表示方式：•二进制(binary)：0,1 ，满2进1.以`0b`或`0B`开头。•十进制(decimal)：0-9 ，满10进1。•八进制(octal)：0-7 ，满8进1. 以数字`0`开头表示。•十六进制(hex)：0-9及A-F，满16进1. 以`0x`或`0X`开头表示。此处的A-F不区分大小写。如：0x21AF +1= 0X21B0

```java
class BinaryTest{
    public static void main(String[] args){

        int num1 = 0b110;
        int num2 = 110;
        int num3 = 0127;
        int num4 = 0x110A;

        System.out.println("num1 = " + num1);
        System.out.println("num2 = " + num2);
        System.out.println("num3 = " + num3);
        System.out.println("num4 = " + num4);
    }
}
```

### 4.2、二进制

•Java整数常量默认是int类型，当用二进制定义整数时，其第32位是符号位；当是long类型时，二进制默认占64位，第64位是符号位•二进制的整数有如下三种形式：•原码：直接将一个数值换成二进制数。最高位是符号位•负数的**反码**：是对**原码按位取反，只是最高位（符号位）确定为1**。•负数的**补码**：其**反码加1**。计算机以二进制补码的形式保存所有的整数。•正数的原码、反码、补码都相同，负数的补码是其反码+1

> 为什么要使用原码、反码、补码表示形式呢？

计算机辨别“符号位”显然会让计算机的基础电路设计变得十分复杂! 于是人们想出了将符号位也参与运算的方法. 我们知道, 根据运算法则减去一个正数等于加上一个负数, 即: 1-1 = 1 + (-1) = 0 , 所以机器可以只有加法而没有减法, 这样计算机运算的设计就更简单了。

![null](https://i-blog.csdnimg.cn/blog_migrate/ad375f0ed6f54befa9abe2d2ccfda3a5.png)

**二进制——》十进制**

![null](https://i-blog.csdnimg.cn/blog_migrate/c826dd534005e5e6edb85cb9222e3ba3.png)

> 原码与反码是帮助推导出补码而存在的！！！

十进制——》二进制

![null](https://i-blog.csdnimg.cn/blog_migrate/47c999cb3b0d6845288e4def0292ecb4.png)

•对于正数来讲：原码、反码、补码是相同的：三码合一。•计算机底层都是使用二进制表示的数值。•**计算机底层都是使用的数值的`补码`保存数据的。**

### 4.3、进制间转化

> 十进制二进制互转

•二进制转成十进制乘以2的幂数•十进制转成二进制除以2取余数

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/03be98e3f56eb1e6a8384983f938d4e8.png)在这里插入图片描述

![在这里插入图片描述](https://i-blog.csdnimg.cn/blog_migrate/cd6870028b6360df06ef6c1a2fc3e970.png#pic_center)在这里插入图片描述

## 三：运算符

#### 文章目录

•01、运算符••1.1、算术运算符•1.2、赋值运算符•1.3、比较运算符•1.4、逻辑运算符•1.5、位运算符•1.6、三元运算符•02、运算符的优先级•其他

## 01、运算符

> 运算符是一种特殊的符号，用以表示数据的运算、赋值和比较等。

•算术运算符•赋值运算符•比较运算符（关系运算符）•逻辑运算符•位运算符•三元运算符

### 1.1、算术运算符

![null](https://i-blog.csdnimg.cn/blog_migrate/a59b954556fde50f321e7e688f442b03.png)

```java
/*
运算符之一：算术运算符
+ - * / % (前)++ (后)++ (前)-- (后)-- 

*/
class Day3Test{
    public static void main(String[] args) {

        //除号：/
        int num1 = 12;
        int num2 = 5;
        int resule1 = num1 / num2;
        System.out.println(resule1);    //2

        int result2 = num1 / num2 * num2;
        System.out.println(result2);

        double result3 = num1 / num2;
        System.out.println(result3);    //2.0

        double result4 = num1 / num2 + 0.0;    //2.0
        double result5 = num1 / (num2 + 0.0);    //2.4
        double result6 = (double)num1 / num2;    //2.4
        double result7 = (double)(num1 / num2);    //2.0
        System.out.println(result5);
        System.out.println(result6);

        // %：取余运算
        //结果的符号与被模数的符号相同
        int m1 = 12;
        int n1 = 5;
        System.out.println("m1 % n1 = " + m1 % n1);

        int m2 = -12;
        int n2 = 5;
        System.out.println("m2 % n2 = " + m2 % n2);

        int m3 = 12;
        int n3 = -5;
        System.out.println("m3 % n3 = " + m3 % n3);

        int m4 = -12;
        int n4 = -5;
        System.out.println("m4 % n4 = " + m4 % n4);

        //(前)++ : 先自增1，后运算
        //(后)++ ：先运算，后自增1
        int a1 = 10;
        int b1 = ++a1;
        System.out.println("a1 = " + a1 + ",b1 = " + b1);

        int a2 = 10;
        int b2 = a2++;
        System.out.println("a2 = " + a2 + ",b2 = " + b2);

        int a3 = 10;
        a3++;    //a3++;
        int b3 = a3;

        //注意点：
        short s1 = 10;
        //s1 = s1 + 1;    //编译失败
//        s1 = (short)(s1 + 1);    //正确的
        s1++;    //自增1不会改变本身变量的数据类型
        System.out.println(s1);

        //问题：
        byte bb1 = 127;
        bb1++;
        System.out.println("bb1 = " + bb1);

        //(前)-- :先自减1，后运算
        //(后)-- ：先运算，后自减1

        int a4 = 10;
        int b4 = a4--;    //int b4 = --a4;
        System.out.println("a4 = " + a4 + ",b4 = " + b4);
    }
}
```

> 算术运算符的注意问题

•如果对负数取模，可以把模数负号忽略不记，如：5%-2=1。但被模数是负数则不可忽略。此外，取模运算的结果不一定总是整数。•对于除号“/”，它的整数除和小数除是有区别的：整数之间做除法时，只保留整数部分而舍弃小数部分。例如：intx=3510;x=x/1000*1000; x的结果是？•“+”除字符串相加功能外，还能把非字符串转换成字符串.例如：System.out.println(“5+5=”+5+5); //打印结果是？5+5=55 ?

```java
/*
练习：随意给出一个三位数的整数，打印显是它的个位数，十位数，百位数的值。
格式如下：
数字xxx的情况如下：
个位数：
十位数：
百位数：

例如：
数字153的情况如下：
个位数：3
十位数：5
百位数：1

*/
class AriExer{
    public static void main(String[] args){
        int num = 187;
        System.out.println("百位数：" + num/100);
        System.out.println("十位数：" + num%100/10);
        System.out.println("个位数：" + num%10);
    }
}
```

### 1.2、赋值运算符

•符号：`=`•当“=”两侧数据类型不一致时，可以使用自动类型转换或使用强制类型转换原则进行处理。•支持连续赋值。•扩展赋值运算符：`+=, -=, *=, /=, %=`

```java
/*
运算符之二：赋值运算符
+= -= *= /= 

*/
class SetValueTest{
    public static void main(String[] args) {
        //赋值符号：=
        int i1 = 10;
        int j1 = 10;

        int i2,j2;
        //连续赋值
        i2 = j2 = 10;

        int i3 = 10,j3 = 20;

        //***********************
        int num1 = 10;
        num1 += 2;    //num1 = num1 + 2;
        System.out.println(num1);    //12
        
        int num2 = 12;
        num2 %= 5;    //num2 = num2 % 5;
        System.out.println(num2);

        short s1 = 10;
        //s1 = s1 + 2;    //编译失败
        s1 += 2;    //结论：不会改变变量本身的数据类型
        System.out.println(s1);

        //开发中，如果希望变量实现+2的操作，有几种方法？？？(int num = 10)
        //方式一：num = num + 2;
        //方式二：num += 2;(推荐)

        //开发中，如果希望变量实现+1的操作，有几种方法？？？(int num = 10)
        //方式一：num = num + 1;
        //方式二：num += 1;
        //方式三：num++;(推荐)
    }
}
class MkFan{
    public static void main(String[] args) {
        //练习1：
        int i = 1;
        i *= 0.1;
        System.out.println(i);//
        i++;
        System.out.println(i);//

        //练习2：
        int m = 2;
        int n1 = 3;
        n1 *= m++; 
        System.out.println("m=" + m);    //3
        System.out.println("n1=" + n1);    //6

        //练习3：
        int n = 10;
        n += (n++) + (++n);
        System.out.println(n);    //32
    }
}
```

### 1.3、比较运算符

![null](https://i-blog.csdnimg.cn/blog_migrate/15e8fa809ae0203f436177f50a3d5cf0.png)

•比较运算符的结果都是`boolean`型，也就是要么是true，要么是false。•比较运算符“`==`”不能误写成“=” 。

```java
/*
运算符之三：比较运算符
==  !=  > < >= <= instanceof

结论：
1.比较运算符的结果是boolean类型
2.区分 == 和 = 

*/
class CompareTest{
    public static void main(String[] args){
        int i = 10;
        int j = 20;
        System.out.println(i==j);    //false
        System.out.println(i = j);    //20

        boolean b1 = true;
        boolean b2 = false;
        System.out.println(b2 == b1);    //false
        System.out.println(b2 = b1);    //true
    }
}
```

### 1.4、逻辑运算符

•`&`—逻辑与•`|` —逻辑或•`！`—逻辑非•`&&` —短路与•`||` —短路或•`^` —逻辑异或

![null](https://i-blog.csdnimg.cn/blog_migrate/4ac147c577ff503527d927df2754201b.png)

•逻辑运算符用于连接布尔型表达式，在Java中不可以写成3<x<6，应该写成x>3 & x<6 。•“`&`”和“`&&`”的区别：•单`&`时，左边无论真假，右边都进行运算；•双`&`时，如果左边为真，右边参与运算，如果左边为假，那么右边不参与运算。•“`|`”和“`||`”的区别同理，`||`表示：当左边为真，右边不参与运算。•异或(`^`)与或( `|` )的不同之处是：当左右都为true时，结果为false。理解：异或，追求的是“异”!

> **练习**

```java
/*
运算符之四：逻辑运算符
& && | || ！ ^

说明：
1. 逻辑与运算符操作的都是boolean类型的变量

*/
class LogicTest{
    public static void main(String[] args){
        //区分& 与 &&
        //相同点1：& 与 && 的运算结果都相同
        //相同点2：当符号左边是true时，二者都会执行符号右边的运算
        //不同点：当符号左边是false时，&继续执行符号
        //开发中，推荐使用&&
        boolean b1 = false;
        int num1 = 10;
        if(b1 & (num1++ > 0)){
            System.out.println("我现在在南京");
        }else{
            System.out.println("我现在在北京");
        }
        System.out.println("num1 = " + num1);

        boolean b2 = false;
        int num2 = 10;
        if(b2 && (num2++ > 0)){
            System.out.println("我现在在南京");
        }else{
            System.out.println("我现在在北京");
        }
        System.out.println("num2 = " + num2);

        //区分：| 与 ||
        //相同点1：| 与 || 的运算结果都相同
        //相同点2：当符号左边是false时，二者都会执行符号右边的运算
        //不同点3：当符号左边是true时，|继续执行符号右边的运算，而||不再执行符号右边的运算
        //开发中，推荐使用||
        boolean b3 = true;
        int num3 = 10;
        if(b3 | (num3++ > 0)){
            System.out.println("我现在在南京");
        }else{
            System.out.println("我现在在北京");
        }
        System.out.println("num3 = " + num3);

        boolean b4 = true;
        int num4 = 10;
        if(b4 || (num4++ > 0)){
            System.out.println("我现在在南京");
        }else{
            System.out.println("我现在在北京");
        }
        System.out.println("num4 = " + num4);
    }
}
class LogoinTest{
    public static void main(String[] args){
        boolean x = true;
        boolean y = false;
        short z = 42;
        //if(y == true)
        if((z++==42)&&(y=true))z++;
        if((x=false)||(++z==45)) z++;
        System.out.println("z=" + z);    //46
    }
}
```

### 1.5、位运算符

> 1、位运算是直接对整数的二进制进行的运算

![null](https://i-blog.csdnimg.cn/blog_migrate/63868aa0c12c9fd8f8cb7ed765085a74.png)

> 2、**注意：无<<<**

```java
/*
运算符之五：位运算符(了解)

结论：
1.位运算符操作的都是整型的数据变量
2.<< : 在一定范围内，每向左移一位，相当于 * 2
  >> : 在一定范围内，每向右移一位，相当于 / 2

面试题：最高效的计算2 * 8 ？    2 << 3 或 8 << 1
*/
class BitTest{
    public static void main(String[] args){
        int i = 21;
//        i = -21;
        System.out.println("i << 2 :" + (i << 2));
        System.out.println("i << 3 :" + (i << 3));
        System.out.println("i << 20 :" + (i << 20));
        System.out.println("i << 27 :" + (i << 27));
        int m = 12;
        int n = 5;
        System.out.println("m & n :" + (m & n));
        System.out.println("m & n :" + (m | n));
        System.out.println("m & n :" + (m ^ n));
        //练习：交换两个变量的值
        int num1 = 10;
        int num2 = 20;

        //方式一：
    //    int tent = num1;
    //    num1 = num2;
    //    num2 = tent;

        //方式二：
        //好处：不用定义临时变量
        //弊端：①相加可能超出存储范围 ② 有局限性：只适用于数值类型
//        num1 = num1 + num2;
//        num2 = num1 - num2;
//        num1 = num1 - num2;

        //方式三：使用位运算
        num1 = num1 ^ num2;
        num2 = num1 ^ num2;
        num1 = num1 ^ num2;

        System.out.println("num1 = " + num1 + ",num2 = " + num2);
    }
}
```

![null](https://i-blog.csdnimg.cn/blog_migrate/5f458d7426848b700ba0b3da54de0c42.png)

![null](https://i-blog.csdnimg.cn/blog_migrate/8fb5ba68c0db18c975ffc6ade6335978.png)

```java
class BitTest{
    public static void main(String[] args){
        //练习：交换两个变量的值
        int num1 = 10;
        int num2 = 20;

        //方式一：
    //    int tent = num1;
    //    num1 = num2;
    //    num2 = tent;

        //方式二：
        //好处：不用定义临时变量
        //弊端：①相加可能超出存储范围 ② 有局限性：只适用于数值类型
//        num1 = num1 + num2;
//        num2 = num1 - num2;
//        num1 = num1 - num2;

        //方式三：使用位运算
        num1 = num1 ^ num2;
        num2 = num1 ^ num2;
        num1 = num1 ^ num2;

        System.out.println("num1 = " + num1 + ",num2 = " + num2);
    }
}
```

### 1.6、三元运算符

![null](https://i-blog.csdnimg.cn/blog_migrate/a7ea7e35aa033110dd0b0f84fa1e422b.png)

```java
/*
运算符之六：三元运算符
1.结构：(条件表达式)？表达式1 : 表达式2
2. 说明
① 条件表达式的结果为boolean类型
② 根据条件表达式真或假，决定执行表达式1，还是表达式2.
  如果表达式为true,则执行表达式1
  如果表达式为false,则执行表达式2
③ 表达式1 和表达式2要求是一致的。
④ 三元运算符是可以嵌套的
3. 凡是可以使用三元运算的地方，都是可以改写if-else。
   反之，则不一定成立！！！
*/
class SanTest{
    public static void main(String[] args) {
        //获取两个整数的最大值
        int m = 12;
        int n = 5;
        int max = (m > n)? m : n;
        System.out.println(max);

        double num = (m > n) ? 2 : 1.0;
        //(m > n) ? 2 : "n大";    //编译错误

        //****************************************
        String str = (m > n) ? "m大" : ((m == n)? "m和n相等" : "n大");
        System.out.println(str);

        //****************************************
        //获取三个数中的最大值
        int n1 = 12;
        int n2 = 30;
        int n3 = -43;

        int max1 = (n1 > n2) ? n1 : n2;
        int max2 = (max1 > n3) ? max1 : n3;
        System.out.println("三个数中的最大值是：" + max2);

        //此方法：pass
        int max3 = (((n1 > n2)? n1 : n2) > n3) ?((n1 > n2) ? n1 : n2) : n3;
        System.out.println("三个数中的最大值是：" + max3);

        //改写成if-else
        if(m > n){
            System.out.println(m);
        }else{
            System.out.println(n);
        }
    }
}
```

## 02、运算符的优先级

•运算符有不同的优先级，所谓优先级就是表达式运算中的运算顺序。如右表，上一行运算符总优先于下一行。•只有单目运算符、三元运算符、赋值运算符是从右向左运算的。

![null](https://i-blog.csdnimg.cn/blog_migrate/9f619d05e2b5eb4c80517342c66aa53c.png)

## 四：程序流程控制

#### 文章目录

•01、 程序流程控概述•02、 顺序结构•03、分支语句••2.1、分支语句1：if-else结构••2.1.1、输入语句•2.2、 分支语句2：switch-case结构•04、循环结构••4.1、for循环•4.2、while循环•4.3、do-while循环•4.4、嵌套循环结构•4.5、break、continue的使用•其他

## 01、 程序流程控概述

流程控制语句是用来控制程序中各语句执行顺序的语句，可以把语句组合成能完成一定功能的小逻辑模块。

其流程控制方式采用结构化程序设计中规定的三种基本流程结构，即：

•顺序结构•分支结构•循环结构

> 1、顺序结构

程序从上到下逐行地执行，中间没有任何判断和跳转。

> 2、分支结构

•根据条件，选择性地执行某段代码。•有`if…else`和`switch-case`两种分支语句。

> 3、循环结构

•根据循环条件，重复性的执行某段代码。•有`while、do…while、for`三种循环语句。•注：JDK1.5提供了`foreach`循环，方便的遍历集合、数组元素。

## 02、 顺序结构

Java中定义成员变量时采用合法的前向引用。如：

![null](https://i-blog.csdnimg.cn/blog_migrate/bbd971ccbf561a6f116011ef12e6e248.png)

## 03、分支语句

### 2.1、分支语句1：if-else结构

![null](https://i-blog.csdnimg.cn/blog_migrate/b3edcdd684abf65f05a4c7fb26b86714.png)

![null](https://i-blog.csdnimg.cn/blog_migrate/926e8d209339012596dcd4c3ee922c6e.png)

> 1、if-else使用说明：

•条件表达式必须是布尔表达式（关系表达式或逻辑表达式）、布尔变量；•语句块只有一条执行语句时，一对{}可以省略，但建议保留；•if-else语句结构，根据需要可以嵌套使用；•当if-else结构是“多选一”时，最后的else是可选的，根据需要可以省略；•当多个条件是“互斥”关系时，条件判断语句及执行语句间顺序无所谓当多个条件是“包含”关系时，“小上大下/ 子上父下”。

> 2、练习

```java
/*
分支结构中的if-else（条件判断结构）
一、三种结构
第一种：
if(条件表达式){
    执行表达式
}
第二种：
if(条件表达式){
    执行表达式1
}else{
    执行表达式2
}
第三种：
if(条件表达式){
    执行表达式1
}else if{
    执行表达式2
}else if(条件表达式){
    执行表达式3
}
...
else{
    执行表达式n
}

*/
class IfTest{
    public static void main(String[] args){
        //举例1
        int heartBeats = 75;
        if(heartBeats < 60 || heartBeats > 100){
            System.out.println("需要进一步做检查");
        }
        System.out.println("检查结束");

        //举例2
        int age = 23;
        if(age < 18){
            System.out.println("你还可以看动画片");
        }else{
            System.out.println("你可以看科技电影了");
        }

        //举例3
        if(age < 0){
            System.out.println("你输入的数据不合适");
        }else if(age < 18){
            System.out.println("你还是个青少年");
        }else if(age < 35){
            System.out.println("你还是个青壮年");
        }else if(age < 60){
            System.out.println("你还是个中年");
        }else if(age < 120){
            System.out.println("你进入老年了");
        }else{
            System.out.println("你成仙了");
        }
    }
}
```

#### 2.1.1、输入语句

```java
/*
如何从键盘获取不同类型的变量，需要使用Scanner类

具体步骤：
1.导包：import java.util.Scanner;
2.Scanner的实例化;
3.调用Scanner类的相关方法，来获取指定的变量。
*/
import java.util.Scanner;

class IFTest{
    public static void main(String[] args){
        //声明一个Scanner
        Scanner scan = new Scanner(System.in);

        int num = scan.nextInt();

        System.out.println(num);
    }
}
/*
如何从键盘获取不同类型的变量，需要使用Scanner类

具体步骤：
1.导包：import java.util.Scanner;
2.Scanner的实例化;
3.调用Scanner类的相关方法，来获取指定的变量。
*/
import java.util.Scanner;

class IFTest{
    public static void main(String[] args){
        //Scanner实例化
        Scanner scan = new Scanner(System.in);

        System.out.println("请输入你的姓名：");
        String name = scan.next();
        System.out.println(name);

        System.out.println("请输入你的年龄：");
        int age = scan.nextInt();
        System.out.println(age);

        System.out.println("请输入你的体重：");
        double weight = scan.nextDouble();
        System.out.println(weight);

        System.out.println("你是否单身？(true/false)");
        boolean isLive = scan.nextBoolean();
        System.out.println(isLive);

        //char型的获取，Scanner没有提供相关方法，只能获取一个字符串
        System.out.println("请输入你的性别：(男/女)");
        String TF = scan.next();
        char TFChar = TF.charAt(0);
        System.out.println(TFChar);
    }
}
```

> 1、练习1

```java
/*
岳小鹏参加Java考试，他和父亲岳不群达成承诺：
如果：成绩为100分时，奖励一辆BMW；
成绩为(80，99]时，奖励一台iphone xs max；
当成绩为[60,80]时，奖励一个iPad；
其它时，什么奖励也没有。
请从键盘输入岳小鹏的期末成绩，并加以判断

说明：
1.else结构是可选的。
2.针对于条件表达式：
    ① 如果多个条件表达式之间的关系是“互斥”关系(或没有交集的关系),哪个判断和执行语句声明在上面还是下面，无所谓；
    ② 如果多个条件表达式之间是有交集的关系，需要根据实际情况，需要考虑实际情况，考虑清楚应该将哪个结构声明在上面。
    ③ 如果多个条件表达式之间有包含的关系，通常情况下，需要将范围小的声明在范围大的上面。否则，范围小的就没机会运行。
*/
import java.util.Scanner;
class IFTest02{
    public static void main(String[] args){
        Scanner scan = new Scanner(System.in);
        System.out.println("请输入岳小鹏的成绩：");
        int score = scan.nextInt();

        if(score == 100){
            System.out.println("奖励一辆BMW");
        }else if(score >80 && score <=99){
            System.out.println("奖励一台iphone xs max");
        }else if(score >= 60 && score <= 80){
            System.out.println("奖励一个iPad");
        }else{
            System.out.println("奖励？学习去！！！");
        }
    }
}
```

> 2、练习2

```java
/*
编写程序：由键盘输入三个整数分别存入变量num1、num2、num3，
对它们进行排序(使用if-else if-else),并且从小到大输出。

*/
import java.util.Scanner;

class Sorting{
    public static void main(String[] args){
        //Scanner实例化
        Scanner scan = new Scanner(System.in);
        System.out.println("请输入第一个整数：");
        int num1 = scan.nextInt();
        System.out.println("请输入第二个整数：");
        int num2 = scan.nextInt();
        System.out.println("请输入第三个整数：");
        int num3 = scan.nextInt();

        int MaxNumber = 0;
        if(num1 >= num2 ){
            if(num3 >= num1){
                System.out.println(num2 + "," + num1 + "," + num3);
            }else if(num3 <= num2){
                System.out.println(num3 + "," + num2 + "," + num1);
            }else{
                System.out.println(num2 + "," + num3 + "," + num1);
            }
        }else{
            if(num3 >= num2){
                System.out.println(num1 + "," + num2 + "," + num3);
            }else if(num3 <= num1){
                System.out.println(num3 + "," + num1 + "," + num2);
            }else{
                System.out.println(num1 + "," + num3 + "," + num2);
            }
        }
    }
}
```

> 3、练习3

```java
/*
我家的狗5岁了，5岁的狗相当于人类多大呢？
其实，狗的前两年每一年相当于人类的10.5岁，之后每增加一年就增加四岁。
那么5岁的狗相当于人类多少年龄呢？应该是：10.5 + 10.5 + 4 + 4 + 4 = 33岁。
如果用户输入负数，请显示一个提示信息。

*/
import java.util.Scanner;

class DogYear{
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        System.out.println("请输入狗的年龄：");
        double Dyear = scan.nextDouble();
        if(Dyear <= 2 &&  Dyear > 0){
            System.out.println("狗的年龄等同于人的：" + Dyear * 10.5);
        }else if(Dyear <= 0){
            System.out.println("你输入的不正确。");
        }else{
            double number = 2 * 10.5 + (Dyear - 2) * 4;
            System.out.println("狗的年龄等同于人的：" + number);
        }        
    }
}
```

> 4、练习4

```java
/*
假设你想开发一个玩彩票的游戏，程序随机地产生一个两位数的彩票，
提示用户输入一个两位数，然后按照下面的规则判定用户是否能赢。
1)如果用户输入的数匹配彩票的实际顺序，奖金10 000美元。
2)如果用户输入的所有数字匹配彩票的所有数字，但顺序不一致，奖金3 000美元。
3)如果用户输入的一个数字仅满足顺序情况下匹配彩票的一个数字，奖金1 000美元。
4)如果用户输入的一个数字仅满足非顺序情况下匹配彩票的一个数字，奖金500美元。
5)如果用户输入的数字没有匹配任何一个数字，则彩票作废。
提示：使用(int)(Math.random() * 90  + 10)产生随机数。
Math.random() : [0,1)  * 90 [0,90) + 10 [10,100)[10,99]

*/
import java.util.Scanner;

class CaiTest{
    public static void main(String[] args){
        //1、随机产生一个两位数
        //System.out.println(Math.random());//产生[0,1)
        int number = (int)(Math.random()*90 + 10);//得到[10,99]，即[10,100)
        //System.out.println(number);
        
        int numberShi = number/10;
        int numberGe = number%10;
        
        //2、用户输入一个两位数
        Scanner input = new Scanner(System.in);
        System.out.print("请输入一个两位数：");
        int guess = input.nextInt();
        
        int guessShi = guess/10;
        int guessGe = guess%10;
        
        if(number == guess){
            System.out.println("奖金10 000美元");
        }else if(numberShi == guessGe && numberGe == guessShi){
            System.out.println("奖金3 000美元");
        }else if(numberShi==guessShi || numberGe == guessGe){
            System.out.println("奖金1 000美元");
        }else if(numberShi==guessGe || numberGe == guessShi){
            System.out.println("奖金500美元");
        }else{
            System.out.println("没中奖");
        }
        
        System.out.println("中奖号码是：" + number);
    }
}
```

> 6、练习5

```java
/*
大家都知道，男大当婚，女大当嫁。
那么女方家长要嫁女儿，当然要提出一定的条件：高：180cm以上；
富：财富1千万以上；帅：是。如果这三个条件同时满足，则：“我一定要嫁给他!!!”
如果三个条件有为真的情况，则：“嫁吧，比上不足，比下有余。”
如果三个条件都不满足，则：“不嫁！”

*/
import java.util.Scanner;

class GaoFuTest{
    public static void main(String[] args){
        Scanner scan = new Scanner(System.in);

        System.out.println("请输入你的身高：(cm)");
        int height = scan.nextInt();
        System.out.println("请输入你的财富：(千万)");
        double weight = scan.nextDouble();
//        System.out.println("请输入你是否帅：(true/false)");
//        boolean isHandSome = scan.nextBoolean();

//        if(height >= 180 && weight >= 1 && isHandSome){
//            System.out.println("我一定要嫁给他!!!");
//        }else if(height >= 180 || weight >= 1 || isHandSome){
//            System.out.println("嫁吧，比上不足，比下有余。");
//        }else{
//            System.out.println("不嫁！");
//        }

        //方式二
        System.out.println("请输入你是否帅: (是or否)");
        String isHandsome = scan.next();

        if(height >= 100 && weight >= 1 && isHandsome.equals("是")){
            System.out.println("我一定要嫁给他!!!");
        }else if(height >= 180 || weight >= 1 || isHandsome.equals("是")){
            System.out.println("嫁吧，比上不足，比下有余。");
        }else{
            System.out.println("不嫁！");
        }
    }
}
```

### 2.2、 分支语句2：switch-case结构

> **注意： switch结构中的表达式，只能是如下的六种数据类型之一：`byte`、`short`、`char`、`int`、`枚举类型`(JDK5.0)、`String类型`(JDK7.0)**
>
> **不能是：long，float，double，boolean**。

![null](https://i-blog.csdnimg.cn/blog_migrate/debdcc45cc385fbc9aecaf97d6ffe973.png)

```java
/*
分支结构之二：switch-case

1.格式
switch(表达式){
case 常量1:
    执行语句1;
    //break;
case 常量2:
    执行语句2;
    //break;

...

default:
    执行语句n:
    //break;
}

2.说明:
① 根据switch表达式中的值，依次匹配各个case中的常量。一旦匹配成功，进入相应case结构中，执行相关语句。
  当调用完执行语句后，则仍然继续向下执行其他case语句，直到遇到break关键字或末尾结束为止。

② break, 可以使用switch-case结构中，表示一旦执行到此关键字，就跳出switch-case结构。

③ switch结构中的表达式，只能是如下的六种数据类型之一：byte、short、char、int、枚举类型(JDK5.0)、String类型(JDK7.0)
④ case 之后之能声明常量。不能声明范围。

⑤ break关键字是可选的。
⑥ default：相当于if-else结构中的else。
            default 结构是可选的，而且位置是灵活的。
*/

class SwitchTest{
    public static void main(String[] args){

        int number = 2;
        switch(number){
        case 0:
            System.out.println("zero");
            break;
        case 1:
            System.out.println("one");
            break;
        case 2:
            System.out.println("twe");
            break;
        case 3:
            System.out.println("three");
            break;
        default:
            System.out.println("other");
            break;
        }

        //*********************************
        //运行报错，不能运行boolean类型
/*        boolean isHandSome = true;
        switch(isHandSome){
        case true:
            System.out.println("可乐吗？？");
            break;
        case false:
            System.out.println("薯条吗？？");
            break;
        default:
            System.out.println("输入有误！！！");
        }
*/
        //*********************************
        String season= "summer";
        switch(season) {
        case"spring":
            System.out.println("春暖花开");
            break;
        case"summer":
            System.out.println("夏日炎炎");
            break;
        case"autumn":
            System.out.println("秋高气爽");
            break;
        case"winter":
            System.out.println("冬雪皑皑");
            break;
        default:
            System.out.println("季节输入有误");
            break;
        }

        //**************************************
        //运行报错
/*        int age = 10;
        switch(age){            
        case age > 18:
            System.out.println("成年了");
            break;
        default:
            System.out.println("未成年");
        }    */
    }
}
```

> 1、练习1

```java
/*
使用switch 把小写类型的char型转为大写。只转换a, b, c, d, e. 其它的输出“other”。
提示：String word = scan.next();  char c = word.charAt(0); switch(c){}
*/
import java.util.Scanner;
class  SwitchCaseTest1{
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        String word = scan.next();  
        char c = word.charAt(0); 
        switch(c){
        case 'a':
            System.out.println("A");
            break;
        case 'b':
            System.out.println("B");
            break;
        case 'c':
            System.out.println("C");
            break;
        case 'd':
            System.out.println("D");
            break;
        case 'e':
            System.out.println("E");
            break;
        default:
            System.out.println("other");
        }
    }
}
```

> 2、练习2

```java
/*
对学生成绩大于60分的，输出“合格”。低于60分的，输出“不合格”。

说明：如果switch-case语句中多个相同语句，可以进行合并。
*/
class  SwitchTest1{
    public static void main(String[] args){
        int score = 78;
        //方案一
        switch(score / 10){
        case 0:
        case 1:
        case 2:
        case 3:
        case 4:
        case 5:
            System.out.println("不合格");
            break;
        case 6:
        case 7:
        case 8:
        case 9:
        case 10:
            System.out.println("合格");
            break;
        }

        //更优的解法
        switch(score /60){
        case 0:
            System.out.println("不及格");
            break;
        case 1:
            System.out.println("合格");
            break;
        }
    }
}
```

> 3、练习3

```java
/*
根据用于指定月份，打印该月份所属的季节。
3,4,5 春季6,7,8 夏季9,10,11 秋季12, 1, 2 冬季

*/
class MonthTest{
    public static void main(String[] args){
        int month = 6;
        switch(month){
        case 12:
        case 1:
        case 2:
            System.out.println("冬季");
            break;
        case 3:
        case 4:
        case 5:
            System.out.println("春季");
            break;
        case 6:
        case 7:
        case 8:
            System.out.println("夏季");
            break;
        case 9:
        case 10:
        case 11:
            System.out.println("秋季");
            break;
        }
    }
}
```

> 4、练习4

```java
/*
编写程序：从键盘上输入2020年的“month”和“day”，
要求通过程序输出输入的日期为2019年的第几天。
2 15 : 31 + 15

5 7: 31 + 28 +31 +30 + 7
...
说明：break在switch-case中是可选的。
*/
import java.util.Scanner;
class DayTest{
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        System.out.println("请输入2020年的month");
        int month = scan.nextInt();
        System.out.println("请输入2020年的day");
        int day = scan.nextInt();

        //定义一个变量来保存天数
        int sumDays = 0;
        switch(month){
        case 12:
            sumDays += 30;
        case 11:
            sumDays += 31;
        case 10:
            sumDays += 30;
        case 9:
            sumDays += 31;
        case 8:
            sumDays += 31;
        case 7:
            sumDays += 30;
        case 6:
            sumDays += 31;
        case 5:
            sumDays += 30;
        case 4:
            sumDays += 31;
        case 3:
            sumDays += 29;
        case 2:
            sumDays += 31;
        case 1:
            sumDays += day;
        }

        System.out.println("2020年" + month + "月" + day + "日是当年的第" + sumDays + "天");
    }
}
```

> 5、练习5

```java
/*
从键盘分别输入年、月、日，判断这一天是当年的第几天注：判断一年是否是闰年的标准：
1）可以被4整除，但不可被100整除或
2）可以被400整除
(year % 4 == 0 && year % 100 != 0) || year %400 == 0)

说明:
1凡是可以使用switch-case的结构,都可以转换为if-else。反之,不成立。
2.我们写分支结构时,当发现既可以使用switch-case,〔(同时,switch中表达式的取值情况不太多),
又可以使用，我们优先选择使用switch-case。原因:switch-case执行效率稍高。

*/
import java.util.Scanner;
class YearDayTest{
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        System.out.println("请输入year");
        int year = scan.nextInt();
        System.out.println("请输入month");
        int month = scan.nextInt();
        System.out.println("请输入day");
        int day = scan.nextInt();

        //定义一个变量来保存天数
        int sumDays = 0;
        switch(month){
        case 12:
            sumDays += 30;
        case 11:
            sumDays += 31;
        case 10:
            sumDays += 30;
        case 9:
            sumDays += 31;
        case 8:
            sumDays += 31;
        case 7:
            sumDays += 30;
        case 6:
            sumDays += 31;
        case 5:
            sumDays += 30;
        case 4:
            sumDays += 31;
        case 3:
            //判断是否为闰年
            if((year % 4 == 0 && year % 100 != 0) || year %400 == 0){
                sumDays += 29;
            }else{
                sumDays += 28;
            }
        case 2:
            sumDays += 31;
        case 1:
            sumDays += day;
        }

        System.out.println(year + "年" + month + "月" + day + "日是当年的第" + sumDays + "天");
    }
}
```

> 6、练习六

```java
/*
编写一个程序，为一个给定的年份找出其对应的中国生肖。
中国的生肖基于12年一个周期，每年用一个动物代表：
rat、ox、tiger、rabbit、dragon、snake、horse、sheep、monkey、rooster、dog、pig。
提示：2019年：猪2019 % 12 == 3
*/
import java.util.Scanner;
class ZodiacSignTest{
    public static void main(String[] args){
        Scanner scan = new Scanner(System.in);
        System.out.println("请输入年份：");
        int year = scan.nextInt();
        switch (year % 12){
        case 1:
            System.out.println("rooster");
            break;
        case 2:
            System.out.println("dog");
            break;
        case 3:
            System.out.println("pig");
            break;
        case 4:
            System.out.println("rat");
            break;
        case 5:
            System.out.println("ox");
            break;
        case 6:
            System.out.println("tiger");
            break;
        case 7:
            System.out.println("rabbit");
            break;
        case 8:
            System.out.println("dragon");
            break;
        case 9:
            System.out.println("snake");
            break;
        case 10:
            System.out.println("horse");
            break;
        case 11:
            System.out.println("sheep");
            break;
        case 12:
            System.out.println("monkey");
            break;
        }
    }
}
```

## 04、循环结构

> 1、循环结构

在某些条件满足的情况下，反复执行特定代码的功能

> 2、循环语句分类

•for 循环•while 循环•do-while 循环

![null](https://i-blog.csdnimg.cn/blog_migrate/24a9a430df3a5c086730db3577371a2c.png)

### 4.1、for循环

```java
语法格式
for(①初始化部分;②循环条件部分;④迭代部分)｛
            ③循环体部分;
｝


执行过程：①-②-③-④-②-③-④-②-③-④-.....-②


说明：
②循环条件部分为boolean类型表达式，当值为false时，退出循环
①初始化部分可以声明多个变量，但必须是同一个类型，用逗号分隔
④可以有多个变量更新，用逗号分隔
```

![null](https://i-blog.csdnimg.cn/blog_migrate/cbf69d7e85933b822f95ad76f62f3740.png)

```java
/*
For循环结构的使用
一、循环结构的四个要素
① 初始化条件
② 循环条件
③ 循环体
④ 迭代条件

二、for循环的结构
for(①;②;④){
    ③
}
*/
class ForTest{
    public static void main(String[] args){
        for(int i=1;i <= 5 ;i++){
            System.out.println("Hello World!");
        }

        //练习：
        int num = 1;
        for(System.out.print('a');num <= 3;System.out.print('c'),num++){
            System.out.print('b');
        }

        //遍历100以内的偶数,获取所有偶数的和,输出偶数的个数
        int sum = 0;    //记录所有偶数的和
        int count = 0;
        for(int i = 1;i <= 100;i++){
            if(i %2 == 0){
                System.out.println(i);
                sum += i;
                count++;
            }
        }
        System.out.println("100以内的偶数的和：" + sum);
        System.out.println("个数为：" + count);
    }
}
```

> 1、练习1

```java
/*
编写程序从1循环到150，并在每行打印一个值，
另外在每个3的倍数行上打印出“foo”,
在每个5的倍数行上打印“biz”,
在每个7的倍数行上打印输出“baz”。

*/
class ForTest1{
    public static void main(String[] args){
        
        for(int i = 1;i <= 150;i++ ){
            System.out.print(i + " ");
            if(i % 3 == 0){
                System.out.print("foo ");
            }
            if(i % 5 == 0){
                System.out.print("biz ");
            }
            if(i % 7 == 0){
                System.out.print("baz ");
            }

            //换行
            System.out.println();
        }
    }
}
```

> 2、练习2

```java
/*
输入两个正整数m和n，求其最大公约数和最小公倍数。
比如：12和20的最大公约数是4，最小公倍数是60。说明：break关键字的使用

*/
import java.util.Scanner;
class GnumberTest{
    public static void main(String[] args){
        Scanner scan = new Scanner(System.in);
        System.out.println("请输入m:");
        int m = scan.nextInt();
        System.out.println("请输入n:");
        int n = scan.nextInt();
        //获取m和n的较大值
        int max = (m > n) ? m : n;
        //获取m和n的最小值
        int min = (m < n) ? m : n;
        
        //求最大公约数
        for(int i = min;i >= 1;i--){
            if(m % i == 0 && n % i == 0){
                System.out.println("m和n的最大公约数：" + i);
                break;
            }
        }

        //求最小公倍数
        for(int i = max;i <= m * n;i++){
            if( i % m == 0 && i % n == 0){
                System.out.println("m和n的最小公倍数是：" + i);
                break;
            }
        }
    }
}
```

> 3、练习3

```java
/*
输出所有的水仙花数，所谓水仙花数是指一个3位数，其各个位上数字立方和等于其本身。
例如：153 = 1*1*1 + 3*3*3 + 5*5*5

*/
class ForTest2{
    public static void main(String[] args){
        for(int i = 100;i <= 999;i++){
            int a = i / 100;    //获取百位
            int b = i % 100 /10;    //获取十位
            int c = i % 10;    //获取个位
            if(a*a*a + b*b*b + c*c*c == i){
                System.out.println("此数值为满足条件的水仙花数:" + i);
            }
        }
    }
}
```

### 4.2、while循环

> 语法格式

```java
①初始化部分
while(②循环条件部分)｛
    ③循环体部分;
    ④迭代部分;
}
```

执行过程：①-②-③-④-②-③-④-②-③-④-…-②

> 说明：

•注意不要忘记声明④迭代部分。否则，循环将不能结束，变成死循环。•for循环和while循环可以相互转换。

```java
public class WhileLoop {
    public static void main(String args[]) {
        int result = 0;
        int i= 1;
        while(i<= 100) {
            result += i;
            i++;
        }
        System.out.println("result="+ result);
    }
}
```

> 1、练习

```java
/*
While循环结构的使用
一、循环结构的四个要素
① 初始化条件
② 循环条件
③ 循环体
④ 迭代条件

二、while循环的结构
①初始化部分
while(②循环条件部分)｛
    ③循环体部分;
    ④迭代部分;
}

执行过程： ① - ② - ③ - ④ - ② -  ③ - ④ - ... - ② 

说明：
1.写while循环千万要小心不要丢了迭代条件。一旦丢了，就可能导致死循环！
2.写程序要避免死循环。
3.能用while循环的，可以用for循环，反之亦然。二者可以相互转换。
区别：for循环和while循环的初始化条件部分的作用范围不同。

算法：有限性。
*/
class WhileTest{
    public static void main(String[] args){
        //遍历100以内的所有偶数
        int i = 1;
        while(i <= 100){
            if(i % 2 == 0){
                System.out.println(i);
            }
            i++;
        }
    }
}
```

### 4.3、do-while循环

```java
do-while循环结构的使用
一、循环结构的四个要素
① 初始化条件
② 循环条件 --->是boolean类型
③ 循环体
④ 迭代条件

二、do-while循环的结构
①
do{
    ③;
    ④;
}while(②);

执行过程：① - ③ - ④ - ② - ① - ③ - ④ - ... - ②
 
说明：do-while循环至少执行一次循环体。
```

> 1、练习1

```java
class DoWhileTest{
    public static void main(String[] args){
        //遍历100以内的所有偶数,并计算所有偶数的和和偶数的个数
        int number = 1;
        int sum = 0;    //记录总和
        int count = 0;    //记录个数
        do{
            if(number % 2 == 0){
                System.out.println(number);
                sum += number;
                count++;
            }
            number++;
        }while(number <= 100);

        System.out.println("总和为：" + sum);
        System.out.println("个数为：" + count);

        //*********************************
        int numb = 10;
        while(numb > 10){
            System.out.println("hello:while");
            numb--;
        }

        int numb2 = 10;
        do{
            System.out.println("hello：do-while");
            numb2--;
        }while(numb2 > 10);
    }
}
```

> 2、练习2

```java
/*
从键盘读入个数不确定的整数，并判断读入的正数和负数的个数，输入为0时结束程序。

说明：
1.不在循环条件部分限制次数的结构：while(true) , for(true)
2.结束循环的几种方式：
    方式一：循环条件部分返回false;
    方式二：在循环体中，执行break;
*/
import java.util.Scanner;
class XunTest{
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        int Positive = 0;    //正数个数
        int Negative = 0;    //负数个数
        while(true){
            int number = scan.nextInt();
            if(number > 0){
                Positive++;
            }else if(number < 0){
                Negative++;
            }else{
                //一旦执行，跳出循环。
                break;
            }    
        }

        System.out.println("正数的个数：" + Positive);
        System.out.println("负数的个数：" + Negative);
    }
}
```

### 4.4、嵌套循环结构

> 1、嵌套循环(多重循环)

•将一个循环放在另一个循环体内，就形成了嵌套循环。其中，for ,while ,do…while均可以作为外层循环或内层循环。•实质上，嵌套循环就是把内层循环当成外层循环的循环体。当只有内层循环的循环条件为false时，才会完全跳出内层循环，才可结束外层的当次循环，开始下一次的循环。•设外层循环次数为m次，内层为n次，则内层循环体实际上需要执行m*n次。

> 2、例题：

1.九九乘法表2.100以内的所有质数

> 3、练习1

```java
/*
嵌套循环的使用
1.嵌套循环：将一个循环结构A声明在另一个循环结构B的循环体中，就构成了嵌套循环

2.
外层循环：循环结构B
内层循环：循环结构A
3.说明
① 内层循环遍历一遍，只相当于外层循环循环体执行了一次
② 假设外层循环需要执行m次，内层循环需要执行n次。此时内层循环的循环体一共执行了m * n次

4.技巧
外层循环控制行数，内层循环控制列数
*/
class  ForForTest{
    public static void main(String[] args) {
        //******
        for(int i = 1;i <= 6;i++){
            System.out.print("*");
        }
        System.out.println();//换行

        /*
        ******
        ******
        ******
        ******
        */
        for(int i = 1;i <= 4;i++){  
            for(int j = 1;j <= 6;j++){  
                System.out.print('*');
            }
            System.out.println();    //换行
        }
        /*
        *
        **
        ***
        ****
        *****
        */
        for(int i = 1;i <= 5;i++){  //控制行数
            for(int j = 1;j <= i;j++){  //控制列数
                System.out.print("*");
            }
            System.out.println();
        }
        /*
        *****
        ****
        ***
        **
        *
        */
        for(int i = 1;i <= 6;i++){
            for(int j = 1;j <= 6-i;j++){
                System.out.print("*");
            }
            System.out.println();
        }

        /*
        *
        **
        ***
        ****
        *****
        ****
        ***
        **
        *
        */
        for(int i = 1;i <= 5;i++){
            for(int j = 1;j <= i;j++){
                System.out.print("*");
            }
            System.out.println();
        }

        for(int i = 1;i <= 5;i++){
            for(int j = 1;j <= 5-i;j++){
                System.out.print("*");
            }
            System.out.println();
        }

        //九九乘法表
        for(int i = 1;i <= 9;i++){
            for(int j = 1;j <= i;j++){
                System.out.print(i + "*" + j + "=" + i*j + " ");
            }
            System.out.println();    //换行
        }

    }
}
```

> 练习2

```java
/*
100以内的所有质数
质数：素数，只能被1和它本身整除的自然数。

最小的质数是：2
*/
class PrimeNuberTest{
    public static void main(String[] args){
        boolean isFlag = true;    //标识是否被除尽，一旦除尽，修改其值。

        for(int i = 2;i <= 100;i++){    //遍历100以内的自然数
            for(int j =2;j < i;j++){    //j:被i去除
                if(i % j == 0){    //i被j除尽
                    isFlag = false;
                }
            }
            if(isFlag == true){
                System.out.println(i);
            }

            //重置isFlag
            isFlag = true;
        }
    }
}
```

> 练习2的优化

```java
/*
100000以内的所有质数
质数：素数，只能被1和它本身整除的自然数。

最小的质数是：2
*/

class PrimeNuberTest{
    public static void main(String[] args){
        boolean isFlag = true;    //标识是否被除尽，一旦除尽，修改其值。
        int count = 0;    //记录质数的个数

        //获取当前时间举例1970-01-01 00:00:00 的毫秒数
        long start = System.currentTimeMillis();

        for(int i = 2;i <= 100000;i++){    //遍历100以内的自然数
            //优化2：对本身是质数的自然数有效 5447---> 11
        //    for(int j =2;j < i;j++){    //j:被i去除
            for(int j =2;j <= Math.sqrt(i);j++){    //j:被i去除
                if(i % j == 0){    //i被j除尽
                    isFlag = false;
                    break;    //优化一：只对本身非质数的自然数是有效的。
                }
            }
            if(isFlag == true){
            //    System.out.println(i);
                count++;
            }

            //重置isFlag
            isFlag = true;
        }

        //获取当前时间举例1970-01-01 00:00:00 的毫秒数
        long end = System.currentTimeMillis();


        System.out.println("质数的个数:" + count);
        System.out.println("所花费的时间为:" + (end - start));    //16843 --> 5447    优化一
    }
}
```

### 4.5、break、continue的使用

> 1、break的使用

•break语句用于终止某个语句块的执行`{    ......  break;  ......}`•**break语句出现在多层嵌套的语句块中时，可以通过标签指明要终止的是哪一层语句块**`label1:  {  ......label2:    {  ......label3:      {  ......          break label2;          ......        }      }    }`

> 2、continue的使用

•continue 语句•continue只能使用在循环结构中•continue语句用于跳过其所在循环语句块的一次执行，继续下一次循环•**continue语句出现在多层嵌套的循环语句体中时，可以通过标签指明要跳过的是哪一层循环**

> 3、return的使用

•return：并非专门用于结束循环的，它的功能是结束一个方法。当一个方法执行到一个return语句时，这个方法将被结束。•与break和continue不同的是，return直接结束整个方法，不管这个return处于多少层循环之内。

> 4、特殊流程控制语句说明

•break只能用于switch语句和循环语句中。•continue 只能用于循环语句中。•二者功能类似，但continue是终止本次循环，break是终止本层循环。•break、continue之后不能有其他的语句，因为程序永远不会执行其后的语句。•标号语句必须紧接在循环的头部。标号语句不能用在非循环语句的前面。•很多语言都有goto语句，goto语句可以随意将控制转移到程序中的任意一条语句上，然后执行它。但使程序容易出错。Java中的break和continue是不同于goto的。

> 5、练习1

```java
/*
break和countinue关键字的使用
                使用范围            循环中使用的作用(不同点)    相同点
break:            switch-case            结束当前循环                关键字后面不能声明执行语句
                循环结构中


countinue:        循环结构中            结束当次循环                关键字后面不能声明执行语句

*/
class BreakContinueTest{
    public static void main(String[] args){
        
        for(int i = 1;i <= 10;i++){
            if(i % 4 == 0){
            //    break;    //1、2、3
                continue;    //1、2、3、5、6、7、9、10
            //    System.out.println("该吃饭了！！！");
            }
        //    System.out.println(i);
        }
        //********************************
        for(int i = 1;i <= 4;i++){
            
                for(int j = 1;j <= 10; j++){
                    if(i % 4 == 0){
                //        break;    //默认跳出包裹此关键字最近的一层的循环
                        continue;
                    }
                    System.out.print(j);
                }
                System.out.println();
        }
    }
}
```

## 五：数 组

#### 文章目录

•01、 数组的概述•02、 一维数组的使用••2.1、内存的简化结构•2.2、一维数组的内存解析•2.3、练习1•03、 多维数组的使用••3.1、二位数组•3.2、二维数组的内存解析•3.3、练习•3.4、面试题目•04、 数组中涉及到的常见算法••4.1、数组元素的赋值•4.2、数组元素的基本操作•4.3、数组元素的基本操作 2•4.4、数组的复制、反转、查找•4.5、数组元素的排序算法•4.6、十大内部排序算法•4.7、算法的 5 大特征•4.8、冒泡排序(重要)•4.9、快速排序(初学Java，仅作了解)•4.10排序算法性能对比•05、 Arrays 工具类的使用•06、 数组使用中的常见异常•其他

## 01、 数组的概述

```java
/*
 * 一、数组的概述
 * 1.数组的理解：数组(Array)，是多个相同类型数据按一定顺序排列的集合，
 * 并使用一个名字命名，并通过编号的方式对这些数据进行统一管理。
 * 
 * 2.数组的相关概念：
 * >数组名
 * >元素
 * >角标、下标、索引
 * >数组的长度：元素的个数
 * 
 * 3.数组的特点：
 * 1)数组属于引用类型的变量。数组的元素，既可以是基本数据类型，也可以是引用数据类型。
 * 2)创建数组对象会在内存中开辟一整块连续的空间；
 * 3)数组的长度一旦确定，就不能修改;
 * 4)数组是有序排列的。
 * 
 * 4.数组的分类：
 *     ① 按照维数：一维数组、二维数组、三维数组……
 *  ② 按照数组元素类型：基本数据类型元素的数组、引用类型元素的数组
 *  
 */
```

## 02、 一维数组的使用

```java
/*
 *     ① 一维数组的声明和初始化
 *  ② 如何调用数组的指定位置的元素
 *  ③ 如何获取数组的长度
 *  ④ 如何遍历数组
 *  ⑤ 数组元素的默认初始化值：见ArrayTest1.java
 *  ⑥ 数组的内存解析：见ArrayTest1.java
 */
```

> 1、代码案例1——ArrayTest.java

```java
public class ArrayTest {
    public static void main(String[] args) {
        
        //1. 一维数组的声明和初始化
        int num;    //声明
        num = 10;    //初始化
        int id = 1001;    //声明 + 初始化
        
        int[] ids;    //声明
        //1.1静态初始化:数组的初始化和数组元素的赋值操作同时进行
        ids = new int[]{1001,1002,1003,1004};    
        //1.2动态初始化:数组的初始化和数组元素的赋值操作分开进行
        String[] names = new String[5]; 
        
        //错误的写法：
//        int[] arr1 = new int[];    //未赋值、未指明长度
//        int[5] arr2 = new int[5];
//        int[] arr3 = new int[3]{1,2,3};
        
        //也是正确的写法：
        int[] arr7 = {1,2,3,5,4};//类型推断
        
        /*总结：数组一旦初始化完成，其长度就确定了。
        */
        
        //2.如何调用数组的指定位置的元素：通过角标的方式调用。
        //数组的角标(或索引)从0开始的，到数组的长度-1结束
        names[0] = "张郃";
        names[1] = "王陵";
        names[2] = "张学良";
        names[3] = "王传志";    //charAt(0)
        names[4] = "李峰";
//        names[5] = "周礼";    //如果数组超过角标会通过编译，运行失败。
        
        //3.如何获取数组的长度
        //属性：length
        System.out.println(names.length);    //5
        System.out.println(ids.length);    //4
        
        //4.如何遍历数组
//        System.out.println(names[0]);
//        System.out.println(names[1]);
//        System.out.println(names[2]);
//        System.out.println(names[3]);
//        System.out.println(names[4]);
        
        for(int i = 0;i < names.length;i++){
            System.out.println(names[i]);
        }
        
    }
}
```

> 2、代码案例2——ArrayTest1.java

```java
/*
 * ⑤ 数组元素的默认初始化值
 *         > 数组元素是整形：0
 *         > 数组元素是浮点型：0.0
 *         > 数组元素是char型：0或'\u0000'，而非'0'
 *         > 数组元素是boolean型:false
 * 
 *         > 数组元素是引用数据类型：null 
 */
public class ArrayTest1 {
    public static void main(String[] args) {
        //5.数组元素的默认初始化值
        int[] arr = new int[4];
        for(int i = 0;i < arr.length;i++){
            System.out.println(arr[i]);
        }
        System.out.println("*****************");
        
        short[] arr1 = new short[4];
        for(int i = 0;i < arr1.length;i++){
            System.out.println(arr1[i]);
        }
        System.out.println("*****************");
        
        float[] arr2 = new float[5]; 
        for(int i = 0;i < arr2.length;i++){
            System.out.println(arr2[i]);
        }
        System.out.println("*****************");
        
        char[] arr3 = new char[5]; 
        for(int i = 0;i < arr3.length;i++){
            System.out.println("----" + arr3[i] + "****");
        }
        
        if(arr3[0] == 0){
            System.out.println("你好！");
        }
        System.out.println("*****************");
        
        boolean[] arr4 = new boolean[5];
        System.out.println(arr4[0]);
        
        System.out.println("*****************");
        String[] arr5 = new String[5];
        System.out.println(arr5[0]);
        //验证
        if(arr5[0] == null){
            System.out.println("北京天气好差！");
        }
        
    }
}
```

### 2.1、内存的简化结构

![null](https://i-blog.csdnimg.cn/blog_migrate/b16d3dcf0d36a98a89b060361204c9aa.png)

### 2.2、一维数组的内存解析

```java
int[] arr = new int[]{1,2,3};
String[] arr1 = new String[4];
arr1[1] = “刘德华”;
arr1[2] = “张学友”;
arr1 = new String[3];
System.out.println(arr1[1]);//null
```

![null](https://i-blog.csdnimg.cn/blog_migrate/d90757902abada989fa2939b28ef4881.png)

> 按照图中步骤，最后数组内存解析完成，数组内部值为null。

### 2.3、练习1

```java
/*
 * 升景坊单间短期出租4个月，550元/月（水电煤公摊，网费35元/月），空调、卫生间、厨房齐全。
 * 屋内均是IT行业人士，喜欢安静。所以要求来租者最好是同行或者刚毕业的年轻人，爱干净、安静。
 * eclipse代码一键格式规范化：Ctrl+Shift+F
 */
public class ArrayDemo {
    public static void main(String[] args) {
        int[] arr = new int[] { 8, 2, 1, 0, 3 };
        int[] index = new int[] { 2, 0, 3, 2, 4, 0, 1, 3, 2, 3, 3 };
        String tel = "";
        for (int i = 0; i < index.length; i++) {
            tel += arr[index[i]];
        }
        System.out.println("联系方式：" + tel);
    }
}
```

> 1、练习2

```java
/*
 * 2. 从键盘读入学生成绩，找出最高分，并输出学生成绩等级。
 * 成绩>=最高分-10    等级为’A’   
 * 成绩>=最高分-20    等级为’B’
 * 成绩>=最高分-30    等级为’C’   
 * 其余等级为’D’
 * 提示：先读入学生人数，根据人数创建int数组，存放学生成绩。
 */
import java.util.Scanner;
public class ArrayDemo2 {
    public static void main(String[] args) {
        //1.使用Scanner，读取学生的个数
        Scanner scan = new Scanner(System.in);
        System.out.print("请输入学生人数：");
        int num = scan.nextInt();
        
        //2.创建数组，存储学生成绩，动态初始化
        int[] str = new int[num];
        System.out.println("请输入" + num + "个学生成绩");
                
        //3.给数组中的元素赋值
        int maxnum = 0;
        for(int i = 0;i < str.length;i++){
            str[i] = scan.nextInt();
            //4.获取数组元素中的最大值：最高分
            if(maxnum < str[i]){
                maxnum = str[i];
            }
        }
        
        //5.根据每个学生成绩与最高分的差值，得到每个学生的等级，并输出等级和成绩    
        char Grade;    //成绩等级
        for(int i = 0;i < str.length;i++){
            if(maxnum - str[i] <= 10){
                Grade = 'A';
            }else if(maxnum - str[i] <= 20){
                Grade = 'B';
            }else if(maxnum - str[i] <= 30){
                Grade = 'C';
            }else{
                Grade = 'D';
            }
            
            System.out.println("student " + i + "score is" + str[i] + 
                    " grade is " + Grade);
        }
    }
}
```

## 03、 多维数组的使用

Java 语言里提供了支持多维数组的语法。

> 如果说可以把一维数组当成几何中的线性图形，那么二维数组就相当于是一个表格，像下图Excel中的表格一样。

![null](https://i-blog.csdnimg.cn/blog_migrate/64ea3ff3e8dcf058c3abb7f2db44b376.png)

### 3.1、二位数组

> 1、代码案例——ArrayTest2.java

```java
/*
 * 二维数组的使用
 * 
 * 1.理解
 * 对于二维数组的理解，我们可以看成是一维数组array1又作为另一个一维数组array2的元素而存在。
 * 其实，从数组底层的运行机制来看，其实没有多维数组。
 * 
 * 2.二维数组的使用：
 *     ① 二维数组的初始化
 *  ② 如何调用数组的指定位置的元素
 *  ③ 如何获取数组的长度
 *  ④ 如何遍历数组
 *  ⑤ 数组元素的默认初始化值:见ArrayTest3.java
 *  ⑥ 数组的内存解析:见ArrayTest3.java
 * 
 */
public class ArrayTest2 {
    public static void main(String[] args) {
        //1.二维数组的声明和初始化
        int[] arr = new int[]{1,2,3};
        //静态初始化
        int[][] arr1 = new int[][]{{1,2,3},{4,5,6},{7,8,9}};
        //动态初始化1
        String[][] arr2 = new String[3][2];
        //动态初始化2
        String[][] arr3 = new String[3][];
        
        //错误的情况
//        String[][] arr4 = new String[][];
//        String[][] arr5 = new String[][4];
//        String[][] arr6 = new String[4][3]{{1,2,3},{4,5,6},{7,8,9}};
        
        //正确的情况：
        int arr4[][] = new int[][]{{1,2,3},{4,5,12,6},{7,8,9}};
        int[] arr5[] = new int[][]{{1,2,3},{4,5,6},{7,8,9}};
        int[][] arr6 = {{1,2,3},{4,5,6},{7,8,9}};        
        
        //2.如何调用数组的指定位置的元素
        System.out.println(arr1[0][1]);    //2
        System.out.println(arr2[1][1]);    //null
        
        arr3[1] = new String[4];    //定义arr3的[1]为长度为4的字符数组
        System.out.println(arr3[1][0]);    //没有上句，会报错
        
        //3.获取数组的长度
        System.out.println(arr4.length);    //3
        System.out.println(arr4[0].length);    //3
        System.out.println(arr4[1].length);    //4
        
        //4.如何遍历二维数组
        for(int i = 0;i < arr4.length;i++){
            for(int j = 0;j < arr4[i].length;j++){
                System.out.print(arr4[i][j] + " ");
            }
            System.out.println();
        }
    }
}
```

> 2、代码案例——ArrayTest3.java

```java
/*
 * 二维数组的使用：
 *     规定：二维数组分为外层数组的元素，内层数组的元素
 *     int[][] arr = new int[4][3]; 
 *  外层元素:arr[0],arr[1]等
 *  内层元素:arr[0][0],arr[1][2]等
 *  
 *     ⑤ 数组元素的默认初始化值
 *     针对于初始化方式一：比如：int[][] arr = new int[4][3];
 *         外层元素的初始化值为：地址值
 *         内层元素的初始化值为：与一维数组初始化情况相同
 *     
 * 针对于初始化方式而：比如：int[][] arr = new int[4][];
 *         外层元素的初始化值为：null
 *         内层元素的初始化值为：不能调用，否则报错。
 * 
 *     ⑥ 数组的内存解析
 */
public class ArrayTest3 {
    public static void main(String[] args) {
        
        int[][] arr = new int[4][3];
        System.out.println(arr[0]);    //[I@15db9742
        System.out.println(arr[0][0]);    //0
        
//        System.out.println(arr);    //ArrayTest3.java
        
        System.out.println("***********************");
        float[][] arr1 = new float[4][3];
        System.out.println(arr1[0]);    //地址值
        System.out.println(arr1[0][0]);    //0.0
        
        System.out.println("***********************");
        
        String[][] arr2 = new String[4][2];
        System.out.println(arr2[1]);    //地址值
        System.out.println(arr2[1][1]);    //null
        
        System.out.println("*********************");
        double[][] arr3 = new double[4][];
        System.out.println(arr3[1]);    //null
//        System.out.println(arr3[1][0]);    //报错
    }
}
```

### 3.2、二维数组的内存解析

> 1、案例1

```java
int[][] arr1 = new int[4][];
arr1[1] = new int[]{1,2,3};
arr1[2] = new int[4];
arr1[2][1] = 30;
```

![null](https://i-blog.csdnimg.cn/blog_migrate/2849f926e522a9e03443fc68f5ee311a.png)

> 2、案例2

```java
int[][] arr4= newint[3][];
System.out.println(arr4[0]);//null
System.out.println(arr4[0][0]);//报错
arr4[0] = new int[3];
arr4[0][1] = 5;
arr4[1] = new int[]{1,2};
```

![null](https://i-blog.csdnimg.cn/blog_migrate/e4700a1c5048de0ad32be88711f7a12a.png)

> 3、案例3

```java
int[][] arr = new int[3][];
arr[1] = new int[]{1,2,3};
arr[2] = new int[3];
System.out.println(arr[0]);//null
System.out.println(arr[0][0]);//报异常
```

![null](https://i-blog.csdnimg.cn/blog_migrate/8f14946127c2c50a83e5cab83721d84c.png)

> 4、案例4

```java
int[][] arr1= newint[4][];
arr1[0] = new int[3];
arr1[1] = new int[]{1,2,3};
arr1[0][2] = 5;
arr1 = new int[2][];
```

![null](https://i-blog.csdnimg.cn/blog_migrate/3a17d4abe1e7eae30c6bf349d2ecc8bd.png)

### 3.3、练习

> 1、练习1

![null](https://i-blog.csdnimg.cn/blog_migrate/3437b9845fcaa6fa6a08f1222aface50.png)

```java
public class ArrayEver1 {
    public static void main(String[] args) {
        int[][] arr = new int[][]{{3,5,8},{12,9},{7,0,6,4}};
        int sum = 0;    //记录总和
        for(int i = 0;i < arr.length;i++){
            for(int j = 0;j < arr[i].length;j++){
                sum += arr[i][j];
            }
        }
        System.out.println(sum);
    }
}
```

> 2、练习 2

![null](https://i-blog.csdnimg.cn/blog_migrate/7ea830dcefb16b5ee42b9131a7fb5549.png)

> 3、练习 3

使用二维数组打印一个 10 行杨辉三角。

```java
/*
 * 【提示】
 * 1. 第一行有 1 个元素, 第 n 行有 n 个元素
 * 2. 每一行的第一个元素和最后一个元素都是 1
 * 3. 从第三行开始, 对于非第一个元素和最后一个元素的元素。
 * 即：yanghui[i][j] = yanghui[i-1][j-1] + yanghui[i-1][j];
 */
public class ArrayEver2 {
    public static void main(String[] args) {
        //1.声明并初始化二维数组
        int[][] arr = new int[10][];
        
        //2.给数组的元素赋值，遍历二维数组
        for(int i = 0;i < arr.length;i++){
            arr[i] = new int[i+1];
            
            //2.1 给首末元素赋值
            arr[i][0]=arr[i][i]=1;
            //2.2 给每行的非首末元素赋值
        //    if(i > 1){
            for(int j = 1;j < arr[i].length-1;j++){
                    arr[i][j] = arr[i-1][j-1] + arr[i-1][j];
                }
        //    }
    
        }
        
    //    3.遍历数组
        for(int i = 0;i < arr.length;i++){
            for(int j = 0;j <arr[i].length;j++){
                System.out.print(arr[i][j] + " ");
            }
            System.out.println();
        }
        
    }
}
```

### 3.4、面试题目

> 1、创建一个长度为 6 的 int 型数组，要求取值为 1-30，同时元素值各不相同

```java
//此题只做了解，初学不必精通。
public class ArrayEver3 {
    public static void main(String[] args) {
        // 方式一：
//        int[] arr = new int[6];
//        for (int i = 0; i < arr.length; i++) {// [0,1) [0,30) [1,31)
//            arr[i] = (int) (Math.random() * 30) + 1;
//
//            boolean flag = false;
//            while (true) {
//                for (int j = 0; j < i; j++) {
//                    if (arr[i] == arr[j]) {
//                        flag = true;
//                        break;
//                    }
//                }
//                if (flag) {
//                    arr[i] = (int) (Math.random() * 30) + 1;
//                    flag = false;
//                    continue;
//                }
//                break;
//            }
//        }
//
//        for (int i = 0; i < arr.length; i++) {
//            System.out.println(arr[i]);
//        }
        // 方式二：
        int[] arr2 = new int[6];
        for (int i = 0; i < arr2.length; i++) {// [0,1) [0,30) [1,31)
            arr2[i] = (int) (Math.random() * 30) + 1;

            for (int j = 0; j < i; j++) {
                if (arr2[i] == arr2[j]) {
                    i--;
                    break;
                }
            }
        }

        for (int i = 0; i < arr2.length; i++) {
            System.out.println(arr2[i]);
        }
    }
}    
```

## 04、 数组中涉及到的常见算法

1.数组元素的赋值(杨辉三角、回形数等)2.求数值型数组中元素的最大值、最小值、平均数、总和等3.数组的复制、反转、查找(线性查找、二分法查找)4.数组元素的排序算法

### 4.1、数组元素的赋值

```java
import java.util.Scanner;
/*
 * 此题了解！！！
 * 
 * 回形数格式方阵的实现
 * 从键盘输入一个整数（1~20） 
 * 则以该数字为矩阵的大小，把 1,2,3…n*n 的数字按照顺时针螺旋的形式填入其中。例如： 输入数字2，则程序输出： 1 2 
 * 4 3 
 * 输入数字 3，则程序输出：1 2 3 
 * 8 9 4 
 * 7 6 5 
 * 输入数字 4， 则程序输出： 
 * 1   2   3   4
 * 12  13  14  5 
 * 11  16  15  6 
 * 10  9   8   7
 */
public class ArrayTest {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("输入一个数字:");
        int len = scanner.nextInt();
        int[][] arr = new int[len][len];
        int s = len * len;
        /*
         * k = 1:向右 k = 2:向下 k = 3:向左 k = 4:向上
         */
        int k = 1;
        int i = 0, j = 0;
        for (int m = 1; m <= s; m++) {
            if (k == 1) {
                if (j < len && arr[i][j] == 0) {
                    arr[i][j++] = m;
                } else {
                    k = 2;
                    i++;
                    j--;
                    m--;
                }
            } else if (k == 2) {
                if (i < len && arr[i][j] == 0) {
                    arr[i++][j] = m;
                } else {
                    k = 3;
                    i--;
                    j--;
                    m--;
                }
            } else if (k == 3) {
                if (j >= 0 && arr[i][j] == 0) {
                    arr[i][j--] = m;
                } else {
                    k = 4;
                    i--;
                    j++;
                    m--;
                }
            } else if (k == 4) {
                if (i >= 0 && arr[i][j] == 0) {
                    arr[i--][j] = m;
                } else {
                    k = 1;
                    i++;
                    j++;
                    m--;
                }
            }
        }
        // 遍历
        for (int m = 0; m < arr.length; m++) {
            for (int n = 0; n < arr[m].length; n++) {
                System.out.print(arr[m][n] + "\t");
            }
            System.out.println();
        }
    }
}
```

### 4.2、数组元素的基本操作

```java
/*
 * 算法的考察：求数值型数组中元素的最大值、最小值、平均数、总和等
 * 
 * 定义一个 int 型的一维数组，包含 10 个元素，分别赋一些随机整数，
 * 然后求出所有元素的最大值，最小值，和值，平均值，并输出出来。
 * 要求：所有随机数都是两位数。
 * 
 * [10,99]
 * 公式：(int)(Math.random() * (99 - 10 + 1) + 10)
 */
public class ArrayTest1 {
    public static void main(String[] args) {
        int[] arr = new int[10];
        //数组赋值
        for(int i = 0;i <arr.length;i++){
            arr[i] = (int)(Math.random() * (99 - 10 + 1) + 10);
        }
        
        //遍历
        for(int i =0;i < arr.length;i++){
            System.out.print(arr[i] + " ");
        }
        System.out.println();
        
        //求数组元素的最大值
        int maxValue = arr[0];
        for(int i = 1;i <arr.length;i++){
            if(maxValue < arr[i]){
                maxValue = arr[i];
            }
        }
        System.out.println("最大值：" + maxValue);
        
        //求数组元素的最小值
        int minValue = arr[0];
        for(int i = 1;i <arr.length;i++){
            if(minValue > arr[i]){
                minValue = arr[i];
            }
        }
        System.out.println("最小值：" + minValue);
        
        //求数组元素的总和
        int sum = 0;
        for(int i = 1;i <arr.length;i++){
            sum += arr[i];
        }
        System.out.println("总和：" + sum);
        
        //求数组元素的平均数
        double avgVales = sum / arr.length;
        System.out.println("平均数：" + avgVales);        
    }
}
```

### 4.3、数组元素的基本操作 2

```java
/*
 * 使用简单数组
 * (1)创建一个名为 ArrayTest 的类，在 main()方法中声明 array1 和 array2 两个变量，他们是 int[]类型的数组。
 * (2)使用大括号{}，把 array1 初始化为 8 个素数：2,3,5,7,11,13,17,19。
 * (3)显示 array1 的内容。
 * (4)赋值 array2 变量等于 array1，修改 array2 中的偶索引元素，使其等于索引值(如 array[0]=0,array[2]=2)。打印出 array1。
 */
public class ArrayTest2 {
    public static void main(String[] args) {
        //声明 array1 和 array2 两个 int[]变量
        int[] array1,array2;
        //array1 初始化
        array1 = new int[]{2,3,5,7,11,13,17,19};
        
        //显示 array1 的内容==遍历。
        for(int i = 0;i < array1.length;i++){
            System.out.print(array1[i] + "\t");
        }
        
        //赋值 array2 变量等于 array1
        //不能称作数组的复制。
        array2 = array1;
        
        //修改 array2 中的偶索引元素，使其等于索引值(如 array[0]=0,array[2]=2)。
        for(int i = 0;i < array2.length;i++){
            if(i % 2 == 0){
                array2[i] = i;
            }
        }
        System.out.println();
        
        //打印出 array1。
        for(int i = 0;i < array1.length;i++){
            System.out.print(array1[i] + "\t");
        }
    }
}
```

> 1、思考：上述 array1 和 array2 是什么关系？

```java
//array1 和 array2 地址值相同，都指向了堆空间的唯一的一个数组实体。
int[] array1,array2;
array1 = new int[]{2,3,5,7,11,13,17,19};
array2 = array1;
for(int i = 0;i < array2.length;i++){
    if(i % 2 == 0){
        array2[i] = i;
    }
}
```

![null](https://i-blog.csdnimg.cn/blog_migrate/44936b84b1b212ad4fac04994dee4505.png)

> 2、拓展：修改题目，实现 array2 对 array1 数组的复制

```java
int[] array1,array2;
array1 = new int[]{2,3,5,7,11,13,17,19};
//数组的复制
array2 = new int[array1.length];
for(int i = 0;i < array2.length;i++){
    array2[i] = array1[i];
}
```

![null](https://i-blog.csdnimg.cn/blog_migrate/872cf7154a7445e07adc7a4a0ff7bf91.png)

### 4.4、数组的复制、反转、查找

> 1、复制、反转

```java
/*
 * 算法的考察：数组的复制、反转、查找(线性查找、二分法查找)
 */
public class ArrayTest3 {
    public static void main(String[] args) {
    
        String[] arr = new String[]{"SS","QQ","YY","XX","TT","KK","EE","GG"};
        
        //数组的复制
        String[] arr1 = new String[arr.length];
        for(int i = 0;i < arr1.length;i++){
            arr1[i] = arr[i];
        }
        
        //数组的反转
        //方法一：
//        for(int i = 0;i < arr.length / 2;i++){
//            String temp = arr[i];
//            arr[i] = arr[arr.length - i - 1];
//            arr[arr.length - i - 1] = temp;
//        }
        
        //方法二：
        for(int i = 0,j = arr.length - 1;i < j;i++,j--){
            String temp = arr[i];
            arr[i] = arr[j];
            arr[j] = temp;
        }
        
        //遍历
        for(int i = 0;i < arr.length;i++){
            System.out.print(arr[i] + "\t");
        }
        System.out.println();
        
        //查找（或搜索）
        //线性查找
        String dest = "BB";    //要查找的元素
        dest = "CC";
        
        boolean isFlag = true;
        
        for(int i = 0;i < arr.length;i++){
            if(dest.equals(arr[i])){
                System.out.println("找到了指定元素，位置为：" + i);
                isFlag = false;
                break;
            }
        }
        if(isFlag){
            System.out.println("很遗憾，没找到！");
        }
        
        //二分法查找：
        
    }
}
```

> 2、二分法查找算法

![null](https://i-blog.csdnimg.cn/blog_migrate/7fd5f5f98e8091b6a5bc2848e613bf9a.png)

```java
public class ArrayTest3 {
    public static void main(String[] args) {
        //二分法查找：
        //前提：所要查找的数组必须有序
        int[] arr2 = new int[]{-98,-34,2,34,54,66,79,105,210,333};
        
        int dest1 = -34;
        int head = 0;    //初始的首索引
        int end = arr2.length - 1;    //初始的末索引
        boolean isFlag1 = true;
        while(head <= end){
            int middle = (head + end)/2;
            
            if(dest1 == arr2[middle]){
                System.out.println("找到了指定元素，位置为：" + middle);
                isFlag1 = false;
                break;
            }else if(arr2[middle] > dest1){
                end = middle - 1;
            }else{    //arr2[middle] < dest1
                head = middle + 1;
            }    
        }
        
        if(isFlag1){
            System.out.println("很遗憾，没找到！");
        }        
    }
}
```

### 4.5、数组元素的排序算法

•排序：假设含有 n 个记录的序列为{R1，R2，…,Rn},其相应的关键字序列为{K1，K2，…,Kn}。将这些记录重新排序为{Ri1,Ri2,…,Rin},使得相应的关键字值满足条 Ki1<=Ki2<=…<=Kin,这样的一种操作称为排序。•通常来说，排序的目的是快速查找。•衡量排序算法的优劣：1.**时间复杂度**：分析关键字的比较次数和记录的移动次数2.空间复杂度：分析排序算法中需要多少辅助内存3.**稳定性**：若两个记录 A 和 B 的关键字值相等，但排序后 A、B 的先后次序保持不变，则称这种排序算法是稳定的。•排序算法分类：**内部排序**和**外部排序**。•内部排序：整个排序过程不需要借助于外部存储器（如磁盘等），所有排序操作都在内存中完成。•外部排序：参与排序的数据非常多，数据量非常大，计算机无法把整个排序过程放在内存中完成，必须借助于外部存储器（如磁盘）。外部排序最常见的是多路归并排序。可以认为外部排序是由多次内部排序组成。

### 4.6、十大内部排序算法

•选择排序•直接选择排序、堆排序•交换排序•**冒泡排序、快速排序**•插入排序•直接插入排序、折半插入排序、Shell 排序•归并排序•桶式排序•基数排序

1.详细操作，见《附录》
附录：尚硅谷_宋红康_排序算法.pdf

### 4.7、算法的 5 大特征

| 输入（Input）                   | 有 0 个或多个输入数据，这些输入必须有清楚的描述和定义        |
| ------------------------------- | ------------------------------------------------------------ |
| 输出（Output）                  | 至少有 1 个或多个输出结果，不可以没有输出结果                |
| 有穷性（有限性，Finiteness）    | 算法在有限的步骤之后会自动结束而不会无限循环，并且每一个步骤可以在可接受的时间内完成 |
| 确定性（明确性，Definiteness）  | 算法中的每一步都有确定的含义，不会出现二义性                 |
| 可行性（有效性，Effectiveness） | 算法的每一步都是清楚且可行的，能让用户用纸笔计算而求出答案   |

> 说明：满足确定性的算法也称为：确定性算法。现在人们也关注更广泛的概念，例如考虑各种非确定性的算法，如并行算法、概率算法等。另外，人们也关注并不要求终止的计算描述，这种描述有时被称为过程（procedure）。

### 4.8、冒泡排序(重要)

冒泡排序的基本思想：通过对待排序序列从前向后，依次比较相邻元素的排序码，若发现逆序则交换，使排序码较大的元素逐渐从前部移向后部。

因为排序的过程中，各元素不断接近自己的位置，如果一趟比较下来没有进行过交换，就说明序列有序， 因此要在排序过程中设置一个标志swap判断元素是否进行过交换。从而减少不必要的比较。

![null](https://i-blog.csdnimg.cn/blog_migrate/3d2bb713b82e23fcf61c3e5b817c4437.png)

```java
/*
 * 数组的冒泡排序的实现
 * 
 */
public class BubbleSortTest {
    public static void main(String[] args) {
        
        int[] arr = new int[]{43,32,76,92,-65,85,71,-42};
        
        //冒泡排序
        for(int i = 0;i < arr.length - 1;i++){
            
            for(int j = 0;j < arr.length - 1 - i;j++){
                
                if(arr[j] > arr[j+1]){
                    int temp = arr[j];
                    arr[j] = arr[j+1];
                    arr[j+1] = temp;
                }
            }
        }
        
        for(int i = 0;i < arr.length;i++){
            System.out.print(arr[i] + "\t");
        }
    }
}
```

### 4.9、快速排序(初学Java，仅作了解)

> 快速排序（Quick Sort）由图灵奖获得者Tony Hoare发明，被列为20世纪十大算法之一，是迄今为止所有内排序算法中速度最快的一种。冒泡排序的升级版，交换排序的一种。快速排序的时间复杂度为O(nlog(n))。

**排序思想：**

1.从数列中挑出一个元素，称为"基准"（pivot），2.重新排序数列，所有元素比基准值小的摆放在基准前面，所有元素比基准值大的摆在基准的后面（相同的数可以到任一边）。在这个分区结束之后，该基准就处于数列的中间位置。这个称为分区（partition）操作。3.递归地（recursive）把小于基准值元素的子数列和大于基准值元素的子数列排序。4.递归的最底部情形，是数列的大小是零或一，也就是永远都已经被排序好了。虽然一直递归下去，但是这个算法总会结束，因为在每次的迭代（iteration）中，它至少会把一个元素摆到它最后的位置去。

![null](https://i-blog.csdnimg.cn/blog_migrate/4fd59a2d068fee16b6487e700ad1e8ba.png)

```java
/**
  * 快速排序
  * 通过一趟排序将待排序记录分割成独立的两部分，其中一部分记录的关键字均比另一部分关键字小，
  * 则分别对这两部分继续进行排序，直到整个序列有序。
  *
 */
public class QuickSort {
    private static void swap(int[] data, int i, int j) {
        int temp = data[i];
        data[i] = data[j];
        data[j] = temp;
    }
    private static void subSort(int[] data, int start, int end) {
        if (start < end) {
            int base = data[start];
            int low = start;
            int high = end + 1;
            while (true) {
                while (low < end && data[++low] - base <= 0)
                    ;
                while (high > start && data[--high] - base >= 0)
                    ;
                if (low < high) {
                    swap(data, low, high);
                } else {
                    break;
                }
            }
            swap(data, start, high);
            
            subSort(data, start, high - 1);//递归调用
            subSort(data, high + 1, end);
        }
    }
    public static void quickSort(int[] data){
        subSort(data,0,data.length-1);
    }
    
    public static void main(String[] args) {
        int[] data = { 9, -16, 30, 23, -30, -49, 25, 21, 30 };
        System.out.println("排序之前：\n" + java.util.Arrays.toString(data));
        quickSort(data);
        System.out.println("排序之后：\n" + java.util.Arrays.toString(data));
    }
}
```

### 4.10排序算法性能对比

![null](https://i-blog.csdnimg.cn/blog_migrate/3767557cf48f626b9b3a8755d31c4bd2.png)

> **各种内部排序方法性能比较**

1.从平均时间而言：快速排序最佳。但在最坏情况下时间性能不如堆排序和归并排序。2.从算法简单性看：由于直接选择排序、直接插入排序和冒泡排序的算法比较简单，将其认为是简单算法。对于Shell排序、堆排序、快速排序和归并排序算法，其算法比较复杂，认为是复杂排序。3.从稳定性看：直接插入排序、冒泡排序和归并排序是稳定的；而直接选择排序、快速排序、Shell排序和堆排序是不稳定排序4.从待排序的记录数n的大小看，n较小时，宜采用简单排序；而n较大时宜采用改进排序。

> **排序算法的选择**

(1) 若n较小(如n≤50)，可采用直接插入或直接选择排序。当记录规模较小时，直接插入排序较好；否则因为直接选择移动的记录数少于直接插入，应选直接选择排序为宜。
(2) 若文件初始状态基本有序(指正序)，则应选用直接插入、冒泡或随机的快速排序为宜；
(3) 若n较大，则应采用时间复杂度为O(nlgn)的排序方法：快速排序、堆排序或归并排序。

## 05、 Arrays 工具类的使用

> java.util.Arrays类即为操作数组的工具类，包含了用来操作数组（比如排序和搜索）的各种方法。

| 1    | boolean equals(int[] a,int[] b)   | 判断两个数组是否相等。                 |
| ---- | --------------------------------- | -------------------------------------- |
| 2    | String toString(int[] a)          | 输出数组信息。                         |
| 3    | void fill(int[] a,int val)        | 将指定值填充到数组之中。               |
| 4    | void sort(int[] a)                | 对数组进行排序。                       |
| 5    | int binarySearch(int[] a,int key) | 对排序后的数组进行二分法检索指定的值。 |

```java
import java.util.Arrays;
/*
 * java.util.Arrays:作数组的工具类，包含了用来操作数组（比如排序和搜索）的各种方法。
 */
public class ArrayTest4 {
    public static void main(String[] args) {
        
        //1.boolean equals(int[] a,int[] b)判断两个数组是否相等。
        int[] arr1 = new int[]{1,2,3,4};
        int[] arr2 = new int[]{1,2,9,3};
        boolean isEquals = Arrays.equals(arr1, arr2);
        System.out.println(isEquals);
        
        //2.String toString(int[] a)输出数组信息。
        System.out.println(Arrays.toString(arr1));        
        
        //3.void fill(int[] a,int val)将指定值填充到数组之中。
        Arrays.fill(arr1, 10);
        System.out.println(Arrays.toString(arr1));        
        
        //4.void sort(int[] a)对数组进行排序。
        Arrays.sort(arr2);
        System.out.println(Arrays.toString(arr2));
        
        //5.int binarySearch(int[] a,int key)对排序后的数组进行二分法检索指定的值。
        int[] arr3 = new int[]{43,32,76,92,-65,85,71,-42}; 
        int index = Arrays.binarySearch(arr3, 210);
        if(index >= 0){
            System.out.println(index);
        }else{
            System.err.println("未找到。");
        }        
    }
}
```

## 06、 数组使用中的常见异常

```java
/*
 * 数组中的常见异常：
 * 1.数组角标越界的异常:ArrayIndexOutOfBoundsException
 * 
 * 2.空指针异常:NullPointerException
 * 
 */
public class ArrayExceptionTest {
    public static void main(String[] args) {
        
        //1.数组角标越界的异常:ArrayIndexOutOfBoundsException
        int[] arr = new int[]{1,2,3,4,5,6};
        
        //错误1：
//        for(int i = 0;i <= arr.length;i++){
//            System.out.println(arr[i]);
//        }
        
        //错误2：
//        System.out.println(arr[-2]);
        
        //错误3
//        System.out.println("hello");
        
        //2.空指针异常:NullPointerException
        //情况一:
//        int[] arr2= new int[]{1,2,3};
//        arr2 = null;
//        System.out.println(arr2[0]);
        //情况二:
//        int[][] arr2 = new int[4][];
//        System.out.println(arr2[0][0]);
        
        //情况三:
//        String[] arr3 = new String[]{"AA","QQ","YY","XX","TT","KK"};
//        arr3[0] = null;
//        System.out.println(arr3[0].toString());        
    }
}
```

## 六：面向对象（上）

#### 文章目录

•01、面向过程与面向对象•02、 类和对象••2.1、Java 类及类的成员•2.2、类与对象的创建及使用•2.3、对象的创建和使用：内存解析•03、类的成员之一：属性•04、 类的成员之二：方法••4.1、类中方法的声明和使用•4.2、理解“万事万物皆对象”•4.3、对象数组的内存解析•4.4、匿名对象的使用•4.5、自定义数组的工具类•4.6、方法的重载(overload)•4.7、可变个数的形参•4.8、方法参数的值传递机制(重点！！！)••4.8.1、**针对基本数据类型**•4.8.2、**针对引用数据类型**•4.8.3、**练习1**•4.8.4、**练习2**•4.8.5、**练习3**•4.8.6、**练习4**•4.8.7、**练习5：将对象作为参数传递给方法**•4.9、递归(recursion)方法•05、面向对象特征之一：封装与隐藏••5.1、四种权限修饰符的理解与测试•5.2、封装性的练习•06、 构造器(构造方法)••6.1、构造器的理解•6.2、总结属性赋值的过程•6.3、JavaBean 的使用•6.4、UML 类图•07、关键字：this 的使用••7.1、this 调用属性、方法、构造器•7.2、this 的练习•8、 关键字：package、import 的使用••8.1、关键字—package•8.2、MVC 设计模式•8.3、关键字—import•其他

## 01、面向过程与面向对象

何谓“面向对象”的编程思想？
首先解释一下“思想”。
先问你个问题：你想做个怎样的人？
可能你会回答：我想做个好人，孝敬父母，尊重长辈，关爱亲朋…
你看，这就是思想。这是你做人的思想，或者说，是你做人的原则。做人有做人的原则，编程也有编程的原则。这些编程的原则呢，就是编程思想。

> 面向过程(POP) 与面向对象(OOP)

•面向对象：Object Oriented Programming•面向过程：Procedure Oriented Programming

```java
/*
 * 一、学习面向对象内容的三条主线
 * 1.Java 类及类的成员：属性、方法、构造器、代码块、内部类
 * 2.面向对象的三大特征：封装、继承、多态性、(抽象性)
 * 3.其它关键字：this、super、static、final、abstract、interface、package、import 等
 * 
 * 二、人把大象装进冰箱
 * 1.面向过程:强调的是功能行为，以函数为最小单位，考虑怎么做。
 * 
 * ① 打开冰箱
 * ② 把大象装进冰箱
 * ③ 把冰箱门关住 
 * 
 * 2.面向对象:强调具备了功能的对象，以类/对象为最小单位，考虑谁来做。
 * 人{
 *         打开(冰箱){
 *             冰箱.开门();
 *         }操作(大象){
 *             大象.进入(冰箱);
 *         }关闭(冰箱){
 *              冰箱.关门();     
 *         }
 * }
 * 
 * 冰箱{
 *         开门(){
 *         }  
 *         关门(){
 *         }
 * }
 * 
 * 大象{
 *         进入(冰箱){
 *         }
 * }
 */
```

> 面向对象的思想概述

•程序员从面向过程的执行者转化成了面向对象的指挥者•面向对象分析方法分析问题的思路和步骤：•根据问题需要，选择问题所针对的现实世界中的实体。•从实体中寻找解决问题相关的属性和功能，这些属性和功能就形成了概念世界中的类。•把抽象的实体用计算机语言进行描述，形成计算机世界中类的定义。即借助某种程序语言，把类构造成计算机能够识别和处理的数据结构。•将类实例化成计算机世界中的对象。对象是计算机世界中解决问题的最终工具。

## 02、 类和对象

```java
/* 
 * 三、面向对象的两个要素：
 * 类:对一类事物的描述，是抽象的、概念上的定义
 * 对象:是实际存在的该类事物的每个个体，因而也称为实    例(instance)。
 * 可以理解为：类= 抽象概念的人；对象= 实实在在的某个人
 * 面向对象程序设计的重点是类的设计；
 * 设计类，其实就是设计类的成员。
 */
```

### 2.1、Java 类及类的成员

现实世界的生物体，大到鲸鱼，小到蚂蚁，都是由最基本的细胞构成的。同理，Java 代码世界是由诸多个不同功能的类构成的。

现实生物世界中的细胞又是由什么构成的呢？细胞核、细胞质、… 那么，Java 中用类 class 来描述事物也是如此。常见的类的成员有：

•属性：对应类中的成员变量•行为：对应类中的成员方法

![null](https://i-blog.csdnimg.cn/blog_migrate/9e2a4953a0325c278e3cdba31ec9ff08.png)

### 2.2、类与对象的创建及使用

```java
/*
 * 一、设计类、其实就是设计类的成员
 * Field = 属性 = 成员变量 = 域、字段
 * Method = (成员)方法 = 函数 
 * 
 * 创建类 = 类的实例化 = 实例化类
 * 
 * 二.类和对象的使用(面向对象思想落地的实现)
 * 1.创建类，设计类的成员
 * 2.创建类的对象
 * 3.通过“对象.属性”或“对象.方法”调用对象的结构
 * 三、如果创建类一个类的多个对象，则每个对象都独立的拥有一套类的属性。(非 static 的)
 *       意味着:如果我们修改一个对象的属性 a，则不影响另外一个对象属性 a 的值。
 */
//测试类
public class PersonTest {
    public static void main(String[] args) {
        //2.创建 Person 类的对象
        //创建对象语法：类名对象名= new 类名();
        Person p1 = new Person();
        //Scanner scan = new Scanner(System.in);
        
        //调用类的结构：属性、方法
        //调用属性:“对象.属性”
        p1.name = "Tom";
        p1.age = 25;
        p1.isMale = true;
        System.out.println(p1.name);
        
        //调用方法:“对象.方法”
        p1.eat();
        p1.sleep();
        p1.talk("chinese");
        //**********************
        Person p2 = new Person();
        System.out.println(p2.name); //null
        System.out.println(p2.isMale);
        //**********************
        //将 p1 变量保存的对象地址值赋给 p3,导致 p1 和 p3 指向了堆空间中的一个对象实体。
        Person p3 = p1;
        System.out.println(p3.name);
        
        p3.age = 10;
        System.out.println(p1.age); //10
    }
}
/*
 * 类的语法格式：
 * 修饰符 class 类名{
 *         属性声明;
 *         方法声明;
 * }
 * 说明：修饰符 public：类可以被任意访问类的正文要用{  }括起来
 */
//1.创建类，设计类的成员
class Person{
    
    //属性:对应类中的成员变量
    String name;
    int age;
    boolean isMale;
    
    //方法:对应类中的成员方法
    public void eat(){
        System.out.println("吃饭");
    }
    
    public void sleep(){
        System.out.println("睡觉");
    }
    
    public void talk(String language){
        System.out.println("人可以说话，使用的是：" + language);
    }
}
```

### 2.3、对象的创建和使用：内存解析

![null](https://i-blog.csdnimg.cn/blog_migrate/a3ec6c35d141f5994b760e1b310cb7ab.png)

•堆（Heap），此内存区域的唯一目的就是存放对象实例，几乎所有的对象实例都在这里分配内存。这一点在 Java 虚拟机规范中的描述是：所有的对象实例以及数组都要在堆上分配。•通常所说的栈（Stack），是指虚拟机栈。虚拟机栈用于存储局部变量等。局部变量表存放了编译期可知长度的各种基本数据类型（boolean、byte、char、short、int、float、long、double）、对象引用（reference 类型，它不等同于对象本身，是对象在堆内存的首地址）。方法执行完，自动释放。•方法区（MethodArea），用于存储已被虚拟机加载的类信息、常量、静态变量、即时编译器编译后的代码等数据。

> 1、案例 1

```java
Person p1= newPerson();
p1.name = "Tom";
p1.isMale = true;
Person p2 = new Person();
sysout(p2.name);//null
Person p3 = p1;
p3.age = 10;
```

![null](https://i-blog.csdnimg.cn/blog_migrate/a094e2a1dab6165d6150da30d108ffdf.png)

> 2、案例 2

```java
Person p1= newPerson();
p1.name = "胡利民";
p1.age = 23;
Person p2 = new Person();
p2.age = 10;
```

![null](https://i-blog.csdnimg.cn/blog_migrate/412872eb936434e9fe3a43e1cb1a2d01.png)

## 03、类的成员之一：属性

```java
/*
 * 类中属性的使用
 * 
 * 属性(成员变量)    vs    局部变量
 * 1.相同点:
 *         1.1 定义变量的格式:数据类型 变量名 = 变量值
 *         1.2 先声明，后使用
 *         1.3 变量都有其对应的作用域
 *                 
 * 2.不同点:
 *         2.1 在类中声明的位置不同
 *         属性:直接定义在类的一对{}内
 *         局部变量:声明在方法内、方法形参、构造器形参、构造器内部的变量
 * 
 *         2.2 关于权限修饰符的不同
 *         属性:可以在声明属性时，指明其权限，使用权限修饰符。
 *             常用的权限修饰符:private、public、缺省、protected
 *             目前声明属性时，都使用缺省即可。
 *         局部变量:不可以使用权限修饰符。
 * 
 *         2.3 默认初始化值的情况:
 *         属性:类的属性，根据其类型，都有默认初始化值。
 *             整型(byte、short、int、long):0
 *             浮点型(float、double):0.0
 *             字符型(char):0(或‘\u0000’)
 *             布尔型(boolean):false
 * 
 *             引用数据类型(类、数组、接口):null
 * 
 *         局部变量:没有默认初始化值
 *             意味着:在调用局部变量之前，一定要显式赋值。
 *             特别地:形参在调用时,赋值即可。例，45 行
 * 
 *         2.4 在内存中加载的位置，亦各不相同。
 *         属性:加载到堆空间中(非 static)
 *         局部变量:加载到栈空间
 */
public class UserTest {
    public static void main(String[] args) {
        User u1 = new User();
        System.out.println(u1.name);
        System.out.println(u1.age);
        System.out.println(u1.isMale);
        
        u1.talk("俄语");
    }
}
class User{
    //属性(或成员变量)
    String name;    //不加 private 即为缺省
    public int age;    //不加 public 即为缺省
    boolean isMale;
    
    public void talk(String language){//language:形参，也是局部变量
        System.out.println("我们使用" + language + "进行交流。");
    }
    
    public void eat(){
        String food = "石头饼";    //石头饼:局部变量
        System.out.println("北方人喜欢吃:" + food);
    }
}
```

> 1、练习1

```java
/*
编写教师类和学生类，并通过测试类创建对象进行测试
Student类
属性:
name:String age:int major:String interests:String
方法:say() 返回学生的个人信息
Teacher类
属性:
name:String age:int teachAge:int course:String
方法:say() 输出教师的个人信息
*/
public class School {
    public static void main(String[] args) {
        Student stu = new Student();
        stu.name = "小明";
        stu.age = 16;
        
        Teacher tea = new Teacher();
        tea.name = "王老师";
        tea.age = 27;
        
        tea.say(stu.name,stu.age);
        stu.say(tea.name, tea.age);
    }    
}
class Student{
    String name;
    int age;
    String major;
    String interests;
    
    void say(String name, int age){
        System.out.println("这个学生是："+name+"年龄是："+age);    }
}
class Teacher{
    String name;
    int age;
    String teachAge;
    String course;
    
    void say(String name, int age){
        System.out.println("这个老师是："+name+"年龄是："+age);
    }
}
```

## 04、 类的成员之二：方法

### 4.1、类中方法的声明和使用

```java
/*
 * 类中方法的声明和使用
 * 
 * 方法：描述类应该具有的功能。
 * 比如：Math类：sqrt()\random() \...
 *     Scanner类：nextXxx() ...
 *     Arrays类：sort() \ binarySearch() \ toString() \ equals() \ ...
 * 
 * 1.举例：
 * public void eat(){}
 * public void sleep(int hour){}
 * public String getName(){}
 * public String getNation(String nation){}
 * 
 * 2. 方法的声明：权限修饰符  返回值类型  方法名(形参列表){
 *                     方法体
 *               }
 *   注意：static、final、abstract 来修饰的方法，后面再讲。
 *   
 * 3. 说明：
 *         3.1 关于权限修饰符：默认方法的权限修饰符先都使用public
 *             Java规定的4种权限修饰符：private、public、缺省、protected  -->封装性再细说
 * 
 *         3.2 返回值类型： 有返回值  vs 没有返回值
 *             3.2.1  如果方法有返回值，则必须在方法声明时，指定返回值的类型。同时，方法中，需要使用
 *                return关键字来返回指定类型的变量或常量：“return 数据”。
 *                   如果方法没有返回值，则方法声明时，使用void来表示。通常，没有返回值的方法中，就不需要
 *               使用return.但是，如果使用的话，只能“return;”表示结束此方法的意思。
 * 
 *             3.2.2 我们定义方法该不该有返回值？
 *                 ① 题目要求
 *                 ② 凭经验：具体问题具体分析
 * 
 *      3.3 方法名：属于标识符，遵循标识符的规则和规范，“见名知意”
 *      3.4 形参列表:方法名可以声明0个、1个，或多个形参。
 *          3.4.1 格式:数据类型1 形参1，数据类型2 形参2,...
 *      
 *          3.4.2 我们定义方法时，该不该定义形参？
 *              ① 题目要求
 *              ② 凭经验，具体问题具体分析
 *      3.5 方法体:方法功能的体现。
 *  4. return关键字的使用：
 *      1.使用范围:使用在方法体中
 *      2.作业:① 结束方法
 *            ② 针对于有返回值类型的方法，使用"return 数据"方法返回所要的数据。
 *      3.注意点:return关键字后不可声明执行语句。
 *  5. 方法的使用中，可以调用当前类的属性或方法。
 *          特殊的:方法A中又调用了方法A:递归方法。
 *      方法中不能定义其他方法。
 */
public class CustomerTest {
    public static void main(String[] args) {
        
        Customer cust1 = new Customer();
        
        cust1.eat();
        
        //测试形参是否需要设置的问题
//        int[] arr = new int[]{3,4,5,2,5};
//        cust1.sort();
        
        cust1.sleep(8);
        
    }
}
//客户类
class Customer{
    
    //属性
    String name;
    int age;
    boolean isMale;
    
    //方法
    public void eat(){
        System.out.println("客户吃饭");
        return;
        //return后不可以声明表达式
//        System.out.println("hello");
    }
    
    public void sleep(int hour){
        System.out.println("休息了" + hour + "个小时");
        
        eat();
//        sleep(10);
    }
    
    public String getName(){
        
        if(age > 18){
            return name;
            
        }else{
            return "Tom";
        }
    }
    
    public String getNation(String nation){
        String info = "我的国籍是：" + nation;
        return info;
    }
    
    //体会形参是否需要设置的问题
//    public void sort(int[] arr){
//        
//    }
//    public void sort(){
//        int[] arr = new int[]{3,4,5,2,5,63,2,5};
//        //。。。。
//    }
    
    public void info(){
        //错误的
//        public void swim(){
//            
//        }
        
    }
}
```

> 1、练习1

创建一个Person类，其定义如下：

![null](https://i-blog.csdnimg.cn/blog_migrate/4a9137ef1e18c6c6a47a57eb042007a1.png)

```java
public class Person {
    String name;
    int age;
    /*
     * sex:1表示为男性
     * sex:0表示为女性
     */
    int sex;
    
    public void study(){
        System.out.println("studying");
    }
    
    public void showAge(){
        System.out.println("age:" + age);
    }
    
    public int addAge(int i){
        age += i;
        return age;
    }
}
```

测试类

```java
/*
 * 要求:
 * (1)创建Person类的对象，设置该对象的name、age和sex属性，
 *     调用study方法，输出字符串“studying”，
 *     调用showAge()方法显示age值，
 *     调用addAge()方法给对象的age属性值增加2岁。
 * (2)创建第二个对象，执行上述操作，体会同一个类的不同对象之间的关系。
 * 
 */
public class PersonTest {
    public static void main(String[] args) {
        Person p1 = new Person();
        
        p1.name = "Tom";
        p1.age = 18;
        p1.sex = 1;
        
        p1.study();
        
        p1.showAge();
        
        int newAge = p1.addAge(2);
        System.out.println(p1.name + "的年龄为" + newAge);
        
        System.out.println(p1.age);    //20
        
        //*******************************
        Person p2 = new Person();
        p2.showAge();    //0
        p2.addAge(10);
        p2.showAge();    //10
        
        p1.showAge();    //20
    }
}
```

> 2、练习2

```java
/*
 * 2.利用面向对象的编程方法，设计类Circle计算圆的面积。
 */
//测试类
public class CircleTest {
    public static void main(String[] args) {
        Circle c1 = new Circle();
        
        c1.radius = 2.1;
        
        //对应方式一:
//        double area = c1.findArea();
//        System.out.println(area);
        
        //对应方式二:
        c1.findArea();
        //错误的调用
        double area = c1.findArea(3.4);
        System.out.println(area);
    }
}
//圆:3.14*r*r
class Circle{
    //属性
    double radius;
    
    //圆的面积方法
    //方法1：
//    public double findArea(){
//        double area = 3.14 * radius * radius;
//        return area;
//    }    
    //方法2：
    public void findArea(){
        double area = Math.PI * radius * radius;
        System.out.println("面积为:" + area);
    }
    //错误情况:
    public double findArea(Double r){
        double area = 3.14 * r * r;
        return area;
    }
}
```

> 3、练习3

```java
/*
 * 3.1 编写程序，声明一个method方法，在方法中打印一个10*8的*型矩形，在main方法中调用该方法。
 * 3.2修改上一个程序，在method方法中，除打印一个10*8的*型矩形外，再计算该矩形的面积，
 * 并将其作为方法返回值。在main方法中调用该方法，接收返回的面积值并打印。
 * 
 * 3.3 修改上一个程序，在method方法提供m和n两个参数，方法中打印一个m*n的*型矩形，
 * 并计算该矩形的面积，将其作为方法返回值。在main方法中调用该方法，接收返回的面积值并打印。
 * 
 */
public class ExerTest {
    
    public static void main(String[] args) {
        
        ExerTest esr = new ExerTest();
        //3.1测试
//        esr.method();
        
        //3.2测试
        //方式一：
//        int area = esr.method();
//        System.out.println("面积为:" + area);
        
        //方式二:
//        System.out.println("面积为:" + esr.method());
        
        //3.3测试
        System.out.println("面积为:" + esr.method(6,5));
    }
    //3.1
//    public void method(){
//        for(int i = 0;i < 10;i++){
//            for(int j = 0;j < 8;j++){
//                System.out.print("* ");
//            }
//            System.out.println();
//        }
//    }
    
    //3.2
//    public int method(){
//        for(int i = 0;i < 10;i++){
//            for(int j = 0;j < 8;j++){
//                System.out.print("* ");
//            }
//            System.out.println();
//        }
//        return 10 * 8;
//    }
    
    //3.3
    public int method(int m,int n){
        for(int i = 0;i < m;i++){
            for(int j = 0;j < n;j++){
                System.out.print("* ");
            }
            System.out.println();
        }
        return m * n;
    }
}
```

> 4、练习四

```java
/*
 * 4. 对象数组题目：定义类Student，包含三个属性：
 * 学号number(int)，年级state(int)，成绩score(int)。
 * 创建20个学生对象，学号为1到20，年级和成绩都由随机数确定。
 * 问题一：打印出3年级(state值为3）的学生信息。
 * 问题二：使用冒泡排序按学生成绩排序，并遍历所有学生信息
 * 提示：  1) 生成随机数：Math.random()，返回值类型double;  
 *         2) 四舍五入取整：Math.round(double d)，返回值类型long。
 * 
 */
public class StudentTest {
    public static void main(String[] args) {
        //声明一个Student类型的数组
        Student[] stu = new Student[20];
        
        for(int i = 0;i <stu.length;i++){
            //给数组元素赋值
            stu[i] = new Student();
            //给Student的对象的属性赋值
            stu[i].number = i + 1;
            //年级:[1,6]
            stu[i].state = (int)(Math.random() * (6 - 1 + 1) + 1);
            //成绩:[0,100]
            stu[i].score = (int)(Math.random() * (100 - 0 + 1));
        }
        
        //遍历学生数组
        for(int i = 0;i < stu.length;i++){
//            System.out.println(stu[i].number + "," + stu[i].state 
//                +  "," + stu[i].score);
            
            System.out.println(stu[i].info());
        }
        System.out.println("*********以下是问题1*********");
        
        //问题一：打印出3年级(state值为3）的学生信息。
        for(int i = 0;i < stu.length;i++){
            if(stu[i].state == 3){
                System.out.println(stu[i].info());
            }
        }
        System.out.println("********以下是问题2**********");
        
        //问题二：使用冒泡排序按学生成绩排序，并遍历所有学生信息。
        for(int i = 0;i < stu.length - 1;i++){
            for(int j = 0;j <stu.length - 1 - i;j++){
                if(stu[j].score >stu[j+1].score){
                    //如果需要换序，交换的是数组的元素，Student对象！！！
                    Student temp = stu[j];
                    stu[j] = stu[j+1];
                    stu[j+1] = temp;
                }
            }
        }
        
        //遍历学生数组
        for(int i = 0;i < stu.length;i++){
            System.out.println(stu[i].info());
        }
        
    }
}
class Student{
    int number;    //学号
    int state;    //年级
    int score;    //成绩
    
    //显示学生信息的方法
    public String info(){
        return "学号:" + number + ",年级:" + state + ",成绩:" + score;
    }
}
```

> 4-1、练习四优化

```java
/*
 * 4. 对象数组题目：定义类Student，包含三个属性：
 * 学号number(int)，年级state(int)，成绩score(int)。
 * 创建20个学生对象，学号为1到20，年级和成绩都由随机数确定。
 * 问题一：打印出3年级(state值为3）的学生信息。
 * 问题二：使用冒泡排序按学生成绩排序，并遍历所有学生信息
 * 提示：  1) 生成随机数：Math.random()，返回值类型double;  
 *         2) 四舍五入取整：Math.round(double d)，返回值类型long。
 * 
 * 此代码是对StudentTest.java的改进，将操作数组的功能封装到方法中。
 */
public class StudentTest2 {
    public static void main(String[] args) {
        //声明一个Student类型的数组
        Student2[] stu = new Student2[20];
        
        for(int i = 0;i <stu.length;i++){
            //给数组元素赋值
            stu[i] = new Student2();
            //给Student的对象的属性赋值
            stu[i].number = i + 1;
            //年级:[1,6]
            stu[i].state = (int)(Math.random() * (6 - 1 + 1) + 1);
            //成绩:[0,100]
            stu[i].score = (int)(Math.random() * (100 - 0 + 1));
        }
        
        StudentTest2 test = new StudentTest2();
        
        //遍历学生数组
        test.print(stu);
        
        System.out.println("*********以下是问题1*********");
        
        //问题一：打印出3年级(state值为3）的学生信息。
        test.searchState(stu, 3);
        System.out.println("********以下是问题2**********");
        
        //问题二：使用冒泡排序按学生成绩排序，并遍历所有学生信息。
        test.sort(stu);
        
        //遍历学生数组
        for(int i = 0;i < stu.length;i++){
            System.out.println(stu[i].info());
        }
    }
    
    /**
      * 
      * @Description 遍历Student[]数组的操作
     */
    public void print(Student2[] stu){
        for(int i = 0;i < stu.length;i++){    
            System.out.println(stu[i].info());
        }
    }
    
    /**
      * 
      * @Description 查找Student数组中指定年级的学习信息
     */
    public void searchState(Student2[] stu,int state){
        for(int i = 0;i < stu.length;i++){
            if(stu[i].state == state){
                System.out.println(stu[i].info());
            }
        }
    }
    
    /**
      * 
      * @Description 给Student数组排序
     */
    public void sort(Student2[] stu){
        for(int i = 0;i < stu.length - 1;i++){
            for(int j = 0;j <stu.length - 1 - i;j++){
                if(stu[j].score >stu[j+1].score){
                    //如果需要换序，交换的是数组的元素，Student对象！！！
                    Student2 temp = stu[j];
                    stu[j] = stu[j+1];
                    stu[j+1] = temp;
                }
            }
        }
    }
}
class Student2{
    int number;    //学号
    int state;    //年级
    int score;    //成绩
    
    //显示学生信息的方法
    public String info(){
        return "学号:" + number + ",年级:" + state + ",成绩:" + score;
    }
}
```

### 4.2、理解“万事万物皆对象”

```java
/* 1.在Java语言范畴中，我们都将功能、结构等封装到类中，通过类的实例化，来调用具体的功能结构。
 *         》Scanner,String等
 *         》文件：File
 *         》网络资源：URL
 * 2.涉及到Java语言与前端html、后端的数据库交互时，前后端的结构在Java层面交互时，都体现为类、对象。
 */
```

### 4.3、对象数组的内存解析

```java
/*引用类型的变量，只可能存储量两类值：null或地址值（含变量类型）*/
Student[] stus= newStudent[5];
stus[0] = new Student();
sysout(stus[0].state);//1
sysout(stus[1]);//null
sysout(stus[1].number);//异常
stus[1] = new Student();
sysout(stus[1].number);//0

class Student{
  int number;//学号
  int state = 1;//年级
  int score;//成绩
}
```

![null](https://i-blog.csdnimg.cn/blog_migrate/e8b522384bd70c59c20b4d1c078e9275.png)

### 4.4、匿名对象的使用

```java
/* 
 * 三、匿名对象的使用
 * 1.理解:我们创建的对象，没有显示的赋值给一个变量名。即为匿名对象。
 * 2.特征：匿名对象只能调用一次。
 * 3.使用:如下
 */
public class InstanceTest {
    public static void main(String[] args) {
        Phone p = new Phone();
//        p = null;
        System.out.println(p);
        
        p.sendEmail();
        p.playGame();
        
        //匿名对象
//        new Phone().sendEmail();
//        new Phone().playGame();
        
        new Phone().price = 1999;
        new Phone().showPrice();    //0.0
        
        //*******************************
        PhoneMall mall = new PhoneMall();
//        mall.show(p);
        //匿名对象的使用
        mall.show(new Phone());    
    }
}

class PhoneMall{
    
    public void show(Phone phone){
        phone.sendEmail();
        phone.playGame();
    }
}

class Phone{
    double price;    //价格
    
    public void sendEmail(){
        System.out.println("发邮件");
    }
    public void playGame(){
        System.out.println("打游戏");
    }
    public void showPrice(){
        System.out.println("手机价格为:" + price);
    }
}
```

### 4.5、自定义数组的工具类

> 1、**工具类**

```java
/*
 * 自定义数组工具类
 */
public class ArrayUtil {

    // 求数组的最大值
    public int getMax(int[] arr) {
        int maxValue = arr[0];
        for (int i = 1; i < arr.length; i++) {
            if (maxValue < arr[i]) {
                maxValue = arr[i];
            }
        }
        return maxValue;
    }

    // 求数组的最小值
    public int getMin(int[] arr) {
        int minValue = arr[0];
        for (int i = 1; i < arr.length; i++) {
            if (minValue > arr[i]) {
                minValue = arr[i];
            }
        }
        return minValue;
    }

    // 求数组总和
    public int getSum(int[] arr) {
        int sum = 0;
        for (int i = 0; i < arr.length; i++) {
            sum += arr[i];
        }
        return sum;
    }

    // 求数组平均值
    public int getAvg(int[] arr) {
        int avgValue = getSum(arr) / arr.length;
        return avgValue;
    }

    // 反转数组
    public void reverse(int[] arr) {
        for (int i = 0; i < arr.length / 2; i++) {
            int temp = arr[i];
            arr[i] = arr[arr.length - i - 1];
            arr[arr.length - i - 1] = temp;
        }
    }

    // 复制数组
    public int[] copy(int[] arr) {
        int[] arr1 = new int[arr.length];
        for (int i = 0; i < arr1.length; i++) {
            arr1[i] = arr[i];
        }
        return null;
    }

    // 数组排序
    public void sort(int[] arr) {
        for (int i = 0; i < arr.length - 1; i++) {
            for (int j = 0; j < arr.length - 1 - i; j++) {
                if (arr[j] > arr[j + 1]) {
                    int temp = arr[j];
                    arr[j] = arr[j + 1];
                    arr[j + 1] = temp;
                }
            }
        }
    }

    // 遍历数组
    public void print(int[] arr) {
        System.out.print("[");
        for (int i = 0; i < arr.length; i++) {
            System.out.print(arr[i] + ",");
        }
        System.out.println("]");
    }

    // 查找指定元素
    public int getIndex(int[] arr, int dest) {
        //线性查找
        for (int i = 0; i < arr.length; i++) {
            if (dest==arr[i]) {
                return i;
            }
        }
        return -1;
    }
}
```

> 2、**测试类**

```java
/**
  * @Description 测试类
  *
 */
public class ArrayUtilTest {


    public static void main(String[] args) {
        ArrayUtil util = new ArrayUtil();
        int[] arr = new int[]{32,5,26,74,0,96,14,-98,25};
        int max = util.getMax(arr);
        System.out.println("最大值为:" + max);
        
//        System.out.print("排序前:");
//        util.print(arr);
//        
//        util.sort(arr);
//        System.out.print("排序后:");
//        util.print(arr);
        
        System.out.println("查找:");
        int index = util.getIndex(arr, 5);
        if(index > 0){
            System.out.println("找到了，索引地址:" + index);
        }else{
            System.out.println("没找到");
        }
    }
}
```

### 4.6、方法的重载(overload)

```java
/*
 * 方法的重载(overload) loading...
 * 
 * 1.定义:在同一个类中，允许存在一个以上的同名方法，只要它们的参数个数或者参数类型不同即可。
 *     
 *         “两同一不同”:同一个类、相同方法名
 *                   参数列表不同：参数个数不同，参数类型不同
 * 
 * 2.举例:
 *         Arrays类中重载的sort() / binarySearch()
 * 
 * 3.判断是否重载
 *         与方法的返回值类型、权限修饰符、形参变量名、方法体都无关。
 * 
 * 4.在通过对象调用方法时，如何确定某一个指定的方法：
 *         方法名---》参数列表
 */
public class OverLoadTest {
    
    public static void main(String[] args) {
        OverLoadTest test = new OverLoadTest();
        test.getSum(1, 2);    //调用的第一个，输出1
    }

    //如下的四个方法构成了重载
    public void getSum(int i,int j){
        System.out.println("1");
    }
    public void getSum(double d1,double d2){
        System.out.println("2");
    }
    public void getSum(String s,int i){
        System.out.println("3");
    }
    
    public void getSum(int i,String s){
        
    }
    
    //以下3个是错误的重载
//    public int getSum(int i,int j){
//        return 0;
//    }
    
//    public void getSum(int m,int n){
//        
//    }
    
//    private void getSum(int i,int j){
//        
//    }
}
```

> 1、**举例**

```java
1.判断：与void show(int a,char b,double c){}构成重载的有：
    
a)void show(int x,char y,double z){} // no
b)int show(int a,double c,char b){} // yes
c) void show(int a,double c,char b){} // yes
d) boolean show(int c,char b){} // yes
e) void show(double c){} // yes 
f) double show(int x,char y,double z){} // no
g) void shows(){double c} // no
```

> 2、**编程**

```java
/*
 * 1.编写程序，定义三个重载方法并调用。方法名为mOL。
 * 三个方法分别接收一个int参数、两个int参数、一个字符串参数。
 * 分别执行平方运算并输出结果，相乘并输出结果，输出字符串信息。
 * 在主类的main ()方法中分别用参数区别调用三个方法。
 * 2.定义三个重载方法max()，
 * 第一个方法求两个int值中的最大值，
 * 第二个方法求两个double值中的最大值，
 * 第三个方法求三个double值中的最大值，并分别调用三个方法。
 * 
 */
public class OverLoadever {
    
    public static void main(String[] args) {
        OverLoadever test = new OverLoadever();
        //1.调用3个方法
        test.mOL(5);
        test.mOL(6, 4);
        test.mOL("fg");
        
        //2.调用3个方法
        int num1 = test.max(18, 452);
        System.out.println(num1);
        double num2 = test.max(5.6, -78.6);
        System.out.println(num2);
        double num3 = test.max(15, 52, 42);
        System.out.println(num3);
    }

    //1.如下三个方法构成重载
    public void mOL(int i){
        System.out.println(i*i);
    }
    public void mOL(int i,int j){
        System.out.println(i*j);
    }
    public void mOL(String s){
        System.out.println(s);
    }
    
    //2.如下三个方法构成重载
    public int max(int i,int j){
        return (i > j) ? i : j;
    }
    public double max(double i,double j){
        return (i > j) ? i : j;
    }
    public double max(double d1,double d2,double d3){
        double max = (d1 > d2) ? d1 : d2;
        return (max > d3) ? max : d3;
    }
}
```

### 4.7、可变个数的形参

JavaSE 5.0 中提供了Varargs(variable number of arguments)机制，允许`直接定义能和多个实参相匹配的形参`。从而，可以用一种更简单的方式，来传递个数可变的实参。

```java
/*
 * 可变个数形参的方法
 * 1.jdk 5.0新增的内容
 * 2.具体使用：
 *     2.1 可变个数形参的格式：数据类型 ... 变量名
 *     2.2 当调用可变个数形参的方法时，传入的参数的个数可以是：0个，1个，2个...
 *     2.3可变个数形参的方法与本类中方法名相同，形参不同的方法之间构成重载。
 *  2.4可变个数形参的方法与本类中方法名相同，形参类型也相同的数组之间不构成重载。即二者不可共存。
 *  2.5可变个数形参在方法中的形参中,必须声明在末尾。
 *  2.6可变个数形参在方法中的形参中，最多只能声明一个可变形参。
 */
public class MethodArgs {

    public static void main(String[] args) {
        MethodArgs test = new MethodArgs();
        test.show(12);
        // test.show("hell0");
        // test.show("hello","world");
        // test.show();

        test.show(new String[] { "AA", "BB", "CC" });
    }

    public void show(int i) {

    }

    // public void show(String s){
    // System.out.println("show(String)");
    // }
    public void show(String... strs) {
        System.out.println("show(String ...strs)");


        for (int i = 0; i < strs.length; i++) {
            System.out.println(strs[i]);
        }
    }

    // 此方法与上一方法不可共存
    // public void show(String[] strs){
    //
    // }

    public void show(int i, String... strs) {

    }

    //The variable argument type String of the method show must be the last parameter
//    public void show(String... strs,int i,) {
//
//    }
}
```

### 4.8、方法参数的值传递机制(重点！！！)

```java
/*
 * 关于变量的赋值
 * 
 *     如果变量是基本数据类型，此时赋值的是变量所保存的数据值。
 *     如果变量是引用数据类型，此时赋值的是变量所保存的数据的地址值。
 * 
 */
public class ValueTransferTest {

    public static void main(String[] args) {
        
        System.out.println("**********基本数据类型：***********");
        int m = 10;
        int n = m;
        
        System.out.println("m = " + m + ", n = " + n);
        
        n = 20;
        
        System.out.println("m = " + m + ", n = " + n);

        System.out.println("***********引用数据类型:********");
        
        Order o1 = new Order();
        o1.orderId = 1001;
        
        Order o2 = o1;    //赋值后，o1和o2的地址值相同，都指向了堆空间中同一个对象实体
        System.out.println("o1.orderId = " + o1.orderId + ",o2.orderId = " + o2.orderId);
        
        o2.orderId = 1002;
        System.out.println("o1.orderId = " + o1.orderId + ",o2.orderId = " + o2.orderId);
        
    }
}

class Order{
    int orderId;
}
```

#### 4.8.1、**针对基本数据类型**

```java
/*
 * 方法的形参的传递机制：值传递
 * 
 * 1.形参：方法定义时，声明的小括号内的参数
 *   实参：方法调用时，实际传递给形参的数据
 * 
 * 2.值传递机制：
 *  如果参数是基本数据类型，此时实参赋值给形参的是实参真是存储的数据值。
 */
public class ValueTransferTest1 {

    public static void main(String[] args) {
        
        int m = 10;
        int n = 20;
        
        System.out.println("m = " + m + ", n = " + n);
        //交换两个变量的值的操作
//        int temp = m;
//        m = n;
//        n = temp;
        
        ValueTransferTest1 test = new ValueTransferTest1();
        test.swap(m, n);
        
        System.out.println("m = " + m + ", n = " + n);
        
    }
    
    public void swap(int m,int n){
        int temp = m;
        m = n;
        n = temp;
    }
}
```

![null](https://gitee.com/lsqpic/BlogPicBed-1/raw/master/img/2021/01/28/20210131185954)

#### 4.8.2、**针对引用数据类型**

```java
/*
 *  如果参数是引用数据类型，此时实参赋值给形参的是实参存储数据的地址值。
 */
public class ValueTransferTest2 {

    public static void main(String[] args) {
        Data data = new Data();
        
        data.m = 10;
        data.n = 20;
        
        System.out.println("m = " + data.m + ", n = " + data.n);

        //交换m和n的值
//        int temp = data.m;
//        data.m = data.n;
//        data.n = temp;

        ValueTransferTest2 test = new ValueTransferTest2();
        test.swap(data);
        
        System.out.println("m = " + data.m + ", n = " + data.n);

    }
    
    public void swap(Data data){
        int temp = data.m;
        data.m = data.n;
        data.n = temp;
    }
}


class Data{
    
    int m;
    int n;
}
```

![null](https://i-blog.csdnimg.cn/blog_migrate/70103bd9f00a1c24da7b548740eff10a.png)

#### 4.8.3、**练习1**

```java
public class TransferTest3{
    public static void main(String args[]){
        TransferTest3 test=new TransferTest3();
        test.first();
    }
    
    public void first(){
        int i=5;
        Value v=new Value();
        v.i=25;
        second(v,i);
        System.out.println(v.i);
    }
    
    public void second(Value v,int i){
        i=0;
        v.i=20;
        Value val=new Value();
        v=val;
        System.out.println(v.i+" "+i);
        
    }
}
class Value {
    int i= 15;
} 
```

![null](https://i-blog.csdnimg.cn/blog_migrate/a68948d8948eb8a513d6d12de35fb9ed.png)

#### 4.8.4、**练习2**

![null](https://i-blog.csdnimg.cn/blog_migrate/ddd09429eef59fae5c20ba2f6e3da404.png)

```java
public static void method(int a,int b){
    a = a * 10;
    b = b * 20;
    System.out.println(a);
    System.out.println(b);
    System.exit(0);
}
```

#### 4.8.5、**练习3**

```java
/*
 * 微软：
 * 定义一个int型的数组：int[] arr = new int[]{12,3,3,34,56,77,432};
 * 让数组的每个位置上的值去除以首位置的元素，得到的结果，作为该位置上的新值。遍历新的数组。 
 */
 
//错误写法
for(int i= 0;i < arr.length;i++){
    arr[i] = arr[i] / arr[0];
}

//正确写法1
for(int i = arr.length –1;i >= 0;i--){
    arr[i] = arr[i] / arr[0];
}

//正确写法2
int temp = arr[0];
for(int i= 0;i < arr.length;i++){
    arr[i] = arr[i] / temp;
}
```

#### 4.8.6、**练习4**

```java
/*
 * int[] arr = new int[10];
 * System.out.println(arr);//地址值?
 * 
 * char[] arr1 = new char[10];
 * System.out.println(arr1);//地址值?
 */
public class ArrayPrint {

    public static void main(String[] args) {
        int[] arr = new int[]{1,2,3};
        //传进去的是一个Object的对象
        System.out.println(arr);//地址值
        
        char[] arr1 = new char[]{'a','b','c'};
        //传进去的是一个数组，里面遍历数据了
        System.out.println(arr1);//abc
    }
}
```

#### 4.8.7、**练习5：将对象作为参数传递给方法**

```java
/*
 * 练习5：将对象作为参数传递给方法
 * (1)定义一个Circle类，包含一个double型的radius属性代表圆的半径，一个findArea()方法返回圆的面积。
 * 
 * (2)定义一个类PassObject，在类中定义一个方法printAreas()，该方法的定义如下：
 * public void printAreas(Circle c,int time)
 * 在printAreas方法中打印输出1到time之间的每个整数半径值，以及对应的面积。
 * 例如，times为5，则输出半径1，2，3，4，5，以及对应的圆面积。
 * 
 * (3)在main方法中调用printAreas()方法，调用完毕后输出当前半径值。
 *
 */
public class Circle {

    double radius;    //半径
    
    //返回圆的面积
    public double findArea(){
        return radius * radius * Math.PI;
    }
}
```

> **PassObject类**

```java
public class PassObject {
    
    public static void main(String[] args) {
        PassObject test = new PassObject();
        
        Circle c = new Circle();
        
        test.printAreas(c, 5);
        
        System.out.println("no radius is:" + c.radius);
    }
    
    public void printAreas(Circle c,int time){
        
        System.out.println("Radius\t\tAreas");
        
        //设置圆的半径
        for(int i = 1;i <= time ;i++){
            c.radius = i;
            System.out.println(c.radius + "\t\t" + c.findArea());
        }
        
        //重新赋值
        c.radius = time + 1;
    }
}
```

### 4.9、递归(recursion)方法

```java
/*
 * 递归方法的使用(了解)
 * 1.递归方法：一个方法体内调用它自身。
 * 2.方法递归包含了一种隐式的循环，它会重复执行某段代码，但这种重复执行无须循环控制。
 * 
 * 3.递归一定要向已知方向递归，否则这种递归就变成了无穷递归，类似于死循环。
 * 
 */
public class RecursionTest {

    public static void main(String[] args) {

        // 例1:计算1-100之间所有自然数的和
        // 方法1:
        int sum = 0;
        for (int i = 1; i <= 100; i++) {
            sum += i;
        }
        System.out.println("sum = " + sum);

        // 方法2:
        RecursionTest test = new RecursionTest();
        int sum1 = test.getSum(100);
        System.out.println("sum1 = " + sum1);
    }

    // 例1:计算1-n之间所有自然数的和
    public int getSum(int n) {

        if (n == 1) {
            return 1;
        } else {
            return n + getSum(n - 1);
        }
    }

    // 例2:计算1-n之间所有自然数的乘积
    //归求阶乘(n!)的算法
    public int getSum1(int n) {


        if (n == 1) {
            return 1;
        } else {
            return n * getSum1(n - 1);
        }
    }
}
```

> 1、**练习1**

```java
public class RecursionTest {

    public static void main(String[] args) {

        int value = test.f(10);
        System.out.println(value);
    }

    //例3:已知有一个数列：f(0) = 1,f(1) = 4,f(n+2)=2*f(n+1) + f(n),
    //其中n是大于0的整数，求f(10)的值。
    public int f(int n){
        if(n == 0){
            return 1;
        }else if(n == 1){
            return 4;
        }else{
            return 2*f(n-1) + f(n-2);
        }
    }
    
    //例4:已知一个数列：f(20) = 1,f(21) = 4,f(n+2) = 2*f(n+1)+f(n),
    //其中n是大于0的整数，求f(10)的值。
    public int f1(int n){
        if(n == 20){
            return 1;
        }else if(n == 21){
            return 4;
        }else{
            return 2*f1(n-1) + f1(n-2);
        }
    }
}
```

> 2、**练习2**

```java
/*
 * 输入一个数据n，计算斐波那契数列(Fibonacci)的第n个值
 * 1  1  2  3  5  8  13  21  34  55
 * 规律：一个数等于前两个数之和
 * 要求：计算斐波那契数列(Fibonacci)的第n个值，并将整个数列打印出来
 * 
 */
public class Recursion2 {

    public static void main(String[] args) {
        
        Recursion2 test = new Recursion2();
        int value = test.f(10);
        System.out.println(value);
    }
    
    public int f(int n) {

        if (n == 1 || n == 2) {
            return 1;
        } else {
            return f(n - 1) + f(n - 2);
        }
    }
}
```

## 05、面向对象特征之一：封装与隐藏

> 1、封装性的引入与体现

为什么需要封装？封装的作用和含义？
我要用洗衣机，只需要按一下开关和洗涤模式就可以了。有必要了解洗衣机内部的结构吗？有必要碰电动机吗？
我要开车，…

> 2、我们程序设计追求“高内聚，低耦合”。

高内聚：类的内部数据操作细节自己完成，不允许外部干涉；
低耦合：仅对外暴露少量的方法用于使用。

> 3、隐藏对象内部的复杂性，只对外公开简单的接口。

便于外界调用，从而提高系统的可扩展性、可维护性。通俗的说，**把该隐藏的隐藏起来，该暴露的暴露出来。这就是封装性的设计思想。**

```java
/*
 * 面向对象的特征一:封装与隐藏
 * 一、问题的引入：
 *    当我们创建一个类的对象以后，我们可以通过"对象.属性"的方式，对对象的属性进行赋值。这里，赋值操作要受到
 *    属性的数据类型和存储范围的制约。但除此之外，没有其他制约条件。但是，实际问题中，我们往往需要给属性赋值
 *    加入额外限制条件。这个条件就不能在属性声明时体现，我们只能通过方法进行条件的添加。比如说，setLegs
 *    同时，我们需要避免用户再使用“对象.属性”的方式对属性进行赋值。则需要将属性声明为私有的(private)
 *    --》此时，针对于属性就体现了封装性。
 *    
 * 二、封装性的体现：
 *    我们将类的属性私有化(private),同时,提供公共的(public)方法来获取(getXxx)和设置(setXxx)
 *    
 *    拓展：封装性的体现：① 如上 ② 单例模式 ③ 不对外暴露的私有方法
 *
 */
public class AnimalTest {

    public static void main(String[] args) {
        Animal a = new Animal();
        a.name = "大黄";
//        a.age = 1;
//        a.legs = 4;//The field Animal.legs is not visible
        
        a.show();
        
//        a.legs = -4;
//        a.setLegs(6);
        a.setLegs(-6);
        
//        a.legs = -4;//The field Animal.legs is not visible
        a.show();
        
        System.out.println(a.name);
        System.out.println(a.getLegs());
    }
}
class Animal{
    
    String name;
    private int age;
    private int legs; //腿的个数
    
    //对于属性的设置
    public void setLegs(int l){
        if(l >= 0 && l % 2 == 0){
            legs = l;
        }else{
            legs = 0;
        }
    }
    
    //对于属性的获取
    public int getLegs(){
        return legs;
    }
    
    public void eat(){
        System.out.println("动物进食");
    }
    
    public void show(){
        System.out.println("name = " + name + ",age = " + age + ",legs = " + legs);
    }
    
    //提供关于属性 age 的 get 和 set 方法
    public int getAge(){
        return age;
    }
    
    public void setAge(int a){
        age = a;
    }
}
```

### 5.1、四种权限修饰符的理解与测试

Java 权限修饰符 `public、protected、default(缺省)、private` 置于类的成员定义前，用来限定对象对该类成员的访问权限。

![图片: https://uploader.shimo.im/f/BnOxeu6anBqhLyCW.png](https://i-blog.csdnimg.cn/blog_migrate/3facdddaedf1205bce14b7a344787aa2.png)图片: https://uploader.shimo.im/f/BnOxeu6anBqhLyCW.png

**对于 class 的权限修饰只可以用 public 和 default(缺省)。**

•public 类可以在任意地方被访问。•default 类只可以被同一个包内部的类访问。

> 1、**Order 类**

```java
/*
 * 三、封装性的体现，需要权限修饰符来配合。
 *   1.Java 规定的 4 种权限：(从小到大排序)private、缺省、protected、public
 *   2.4 种权限用来修饰类及类的内部结构：属性、方法、构造器、内部类
 *   3.具体的，4 种权限都可以用来修饰类的内部结构：属性、方法、构造器、内部类
 *          修饰类的话，只能使用：缺省、public
 *  总结封装性：Java 提供了 4 中权限修饰符来修饰类积累的内部结构，体现类及类的内部结构的可见性的方法。
 * 
 */
public class Order {

    private int orderPrivate;
    int orderDefault;
    public int orderPublic;
    
    private void methodPrivate(){
        orderPrivate = 1;
        orderDefault = 2;
        orderPublic = 3;
    }
    
    void methodDefault(){
        orderPrivate = 1;
        orderDefault = 2;
        orderPublic = 3;
    }
    
    public void methodPublic(){
        orderPrivate = 1;
        orderDefault = 2;
        orderPublic = 3;
    }
}
```

> 2、**OrderTest 类**

```java
public class OrderTest {

    public static void main(String[] args) {
        
        Order order = new Order();
        
        order.orderDefault = 1;
        order.orderPublic = 2;
        //出了 Order 类之后，私有的结构就不可调用了
//        order.orderPrivate = 3;//The field Order.orderPrivate is not visible
        
        order.methodDefault();
        order.methodPublic();
        //出了 Order 类之后，私有的结构就不可调用了
//        order.methodPrivate();//The method methodPrivate() from the type Order is not visible
    }
}
```

> **相同项目不同包的 OrderTest 类**

```java
import github.Order;

public class OrderTest {

    public static void main(String[] args) {
        Order order = new Order();
        
        order.orderPublic = 2;
        //出了 Order 类之后，私有的结构、缺省的声明结构就不可调用了
//        order.orderDefault = 1;
//        order.orderPrivate = 3;//The field Order.orderPrivate is not visible
        
        order.methodPublic();
        //出了 Order 类之后，私有的结构、缺省的声明结构就不可调用了
//        order.methodDefault();
//        order.methodPrivate();//The method methodPrivate() from the type Order is not visible
    }
}
```

![null](https://gitee.com/lsqpic/BlogPicBed-1/raw/master/img/2021/01/28/20210131190033.png)

### 5.2、封装性的练习

![null](https://i-blog.csdnimg.cn/blog_migrate/a2af3c5cc1add866548aa1e97d7b35d3.png)

```java
/*
 * 1.创建程序,在其中定义两个类：Person 和 PersonTest 类。
 * 定义如下：用 setAge()设置人的合法年龄(0~130)，用 getAge()返回人的年龄。
 * 
 */
public class Person {

    private int age;
    
    public void setAge(int a){
        if(a < 0 || a > 130){
//            throw new RuntimeException("传入的数据据非法");
            System.out.println("传入的数据据非法");
            return;
        }
        
        age = a;
        
    }
    
    public int getAge(){
        return age;
    }
    
    //绝对不能这样写！！！
    public int doAge(int a){
        age = a;
        return age;
    }
}
```

> 3、**测试类**

```java
/*
 *  在 PersonTest 类中实例化 Person 类的对象 b，
 *  调用 setAge()和 getAge()方法，体会 Java 的封装性。
 */
public class PersonTest {

    public static void main(String[] args) {
        Person p1 = new Person();
//        p1.age = 1;    //编译不通过
        
        p1.setAge(12);
        
        System.out.println("年龄为:" + p1.getAge());
    }
}
```

## 06、 构造器(构造方法)

### 6.1、构造器的理解

```java
/*
 * 类的结构之三:构造器(构造方法、constructor)的使用
 * constructor:
 * 
 * 一、构造器的作用:
 * 1.创建对象
 * 2.初始化对象的属性
 * 
 * 二、说明
 * 1.如果没有显示的定义类的构造器的话，则系统默认提供一个空参的构造器。
 * 2.定义构造器的格式:
 *             权限修饰符  类名(形参列表) { }
 * 3.一个类中定义的多个构造器，彼此构成重载。
 * 4.一旦显示的定义了类的构造器之后，系统不再提供默认的空参构造器。
 * 5.一个类中，至少会有一个构造器        
 */
public class PersonTest {

    public static void main(String[] args) {
        //创建类的对象:new + 构造器
        Person p = new Person();    //Person()这就是构造器
        
        p.eat();
        
        Person p1 = new Person("Tom");
        System.out.println(p1.name);
    }
}
class Person{
    //属性
    String name;
    int age;
    
    //构造器
    public Person(){
        System.out.println("Person()......");
    }
    
    public Person(String n){
        name = n;
    }
    
    public Person(String n,int a){
        name = n;
        age = a;
    }
    
    //方法
    public void eat(){
        System.out.println("人吃饭");
    }
    
    public void study(){
        System.out.println("人学习");
    }
}
```

> 1、**练习 1**

```java
/* 2.在前面定义的 Person 类中添加构造器，
 * 利用构造器设置所有人的 age 属性初始值都为 18。
 * 
 */
public class Person {

    private int age;
    
    public Person(){
        age = 18;
    }
}

public class PersonTest {

    public static void main(String[] args) {
        Person p1 = new Person();

        System.out.println("年龄为:" + p1.getAge());
    }
}
```

> 2、**练习 2**

```java
/* 3.修改上题中类和构造器，增加 name 属性,
 *   使得每次创建 Person 对象的同时初始化对象的 age 属性值和 name 属性值。
 */
public class Person {

    private int age;
    private String name;
    
    public Person(){
        age = 18;
    }
    
    public Person(String n,int a){
        name = n;
        age = a;
    }
    
    public void setName(String n){
        name = n;
    }
    
    public String getName(){
        return name;
    }
    
    public void setAge(int a){
        if(a < 0 || a > 130){
//            throw new RuntimeException("传入的数据据非法");
            System.out.println("传入的数据据非法");
            return;
        }
        
        age = a;
        
    }
    
    public int getAge(){
        return age;
    }
}

public class PersonTest {

    public static void main(String[] args) {
        
        Person p2 = new Person("Tom",21);
        
        System.out.println("name = " + p2.getName() + ",age = " + p2.getAge());
    }
}
```

> 3、**练习 3**

```java
/*
 * 编写两个类，TriAngle 和 TriAngleTest，
 * 其中 TriAngle 类中声明私有的底边长 base 和高 height，同时声明公共方法访问私有变量。
 * 此外，提供类必要的构造器。另一个类中使用这些公共方法，计算三角形的面积。
 * 
 */
public class TriAngle {

    private double base;//底边长
    private double height;//高
    
    public TriAngle(){
        
    }
    
    public TriAngle(double b,double h){
        base = b;
        height = h;
    }
    
    public void setBase(double b){
        base = b;
    }
    
    public double getBase(){
        return base;
    }
    
    public void setHeight(double h){
        height = h;
    }
    
    public double getHeight(){
        return height;
    }
}

public class TriAngleTest {

    public static void main(String[] args) {
        
        TriAngle t1 = new TriAngle();
        t1.setBase(2.0);
        t1.setHeight(2.5);
//        t1.base = 2.5;//The field TriAngle.base is not visible
//        t1.height = 4.3;        
        System.out.println("base : " + t1.getBase() + ",height : " + t1.getHeight());
        
        TriAngle t2 = new TriAngle(5.1,5.6);
        System.out.println("面积 : " + t2.getBase() * t2.getHeight() / 2);

    }
}
```

### 6.2、总结属性赋值的过程

```java
/*
 * 总结:属性赋值的先后顺序
 * 
 * ① 默认初始化值
 * ② 显式初始化
 * ③ 构造器中赋值
 * ④ 通过"对象.方法" 或 “对象.属性”的方式，赋值
 * 
 * 以上操作的先后顺序:① - ② - ③ - ④
 * 
 */
public class UserTest {

    public static void main(String[] args) {
        User u = new User();
        
        System.out.println(u.age);
        
        User u1 = new User(2);
        
        u1.setAge(3);
        
        System.out.println(u1.age);
    }
}
class User{
    String name;
    int age = 1;
    
    public User(){
        
    }
    
    public User(int a){
        age = a;
    }
    
    public void setAge(int a){
        age = a;
    }
}
```

### 6.3、JavaBean 的使用

```java
/*
 * JavaBean 是一种 Java 语言写成的可重用组件。
 * 所谓 javaBean，是指符合如下标准的 Java 类：
 *         > 类是公共的
 *         > 有一个无参的公共的构造器
 *         > 有属性，且有对应的 get、set 方法
 * 
 */
public class Customer {
    
    private int id;
    private String name;

    public Customer(){
        
    }
    
    public void setId(int i){
        id = i;
    }
    
    public int getId(){
        return id;
    }
    
    public void setName(String n){
        name = n;
    }
    
    public String getName(){
        return name;
    }
}
```

### 6.4、UML 类图

![null](https://i-blog.csdnimg.cn/blog_migrate/80f6714587cae3e899d24d331d024e9f.png)

•表示 public 类型，-表示 private 类型，#表示 protected 类型•方法的写法: 方法的类型(+、-) 方法名(参数名：参数类型)：返回值类型

## 07、关键字：this 的使用

### 7.1、this 调用属性、方法、构造器

```java
/*
 * this 关键字的使用
 * 1.this 用来修饰、调用：属性、方法、构造器
 * 
 * 2.this 修饰属性和方法:
 *         this 理解为：当前对象,或当前正在创建的对象。
 *      
 *  2.1 在类的方法中，我们可以使用"this.属性"或"this.方法"的方式，调用当前对象属性和方法。
 *      通常情况下，我们都选择省略“this.”。特殊情况下，如果方法的形参和类的属性同名，我们必须显式
 *      的使用"this.变量"的方式，表明此变量是属性，而非形参。
 * 
 *  2.2 在类的构造器中，我们可以使用"this.属性"或"this.方法"的方式，调用正在创建的对象属性和方法。
 *      但是，通常情况下，我们都选择省略“this.”。特殊情况下，如果构造器的形参和类的属性同名，我们必须显式
 *      的使用"this.变量"的方式，表明此变量是属性，而非形参。
 *  
 *  3.this 调用构造器
 *      ① 我们可以在类的构造器中，显式的使用"this(形参列表)"的方式，调用本类中重载的其他的构造器！
 *      ② 构造器中不能通过"this(形参列表)"的方式调用自己。
 *      ③ 如果一个类中声明了n个构造器，则最多有n -1个构造器中使用了"this(形参列表)"。
 *      ④ "this(形参列表)"必须声明在类的构造器的首行！
 *      ⑤ 在类的一个构造器中，最多只能声明一个"this(形参列表)"。
 */
public class PersonTest {

    public static void main(String[] args) {
        Person p1 = new Person();
        
        p1.setAge(1);
        System.out.println(p1.getAge());
        
        p1.eat();
        System.out.println();
        
        Person p2 = new Person("jerry" ,20);
        System.out.println(p2.getAge());
    }
}
class Person{
    
    private String name;
    private int age;
    
    public Person(){
        this.eat();
        String info = "Person 初始化时，需要考虑如下的 1,2,3,4...(共 40 行代码)";
        System.out.println(info);
    }
    
    public Person(String name){
        this();
        this.name = name;
    }
    
    public Person(int age){
        this();
        this.age = age;
    }
    
    public Person(String name,int age){
        this(age);    //调用构造器的一种方式
        this.name = name;
//        this.age = age;
    }
    
    public void setNmea(String name){
        this.name = name;
    }
    
    public String getName(){
        return this.name;
    }
    
    public void setAge(int age){
        this.age = age;
    }
    
    public int getAge(){
        return this.age;
    }
    
    public void eat(){
        System.out.println("人吃饭");
        this.study();
    }
    
    public void study(){
        System.out.println("学习");
    }
}
```

### 7.2、this 的练习

![null](https://i-blog.csdnimg.cn/blog_migrate/9ab0c7765593e0969b1f756eec66472e.png)

> 1、**Boy 类**

```java
public class Boy {

    private String name;
    private int age;
    
    public void setName(String name){
        this.name = name;
    }
    
    public String getName(){
        return name;
    }
    
    public void setAge(int ahe){
        this.age = age;
    }
    
    public int getAge(){
        return age;
    }
    
    public Boy(String name, int age) {
        this.name = name;
        this.age = age;
    }


    public void marry(Girl girl){
        System.out.println("我想娶" + girl.getName());
    }
    
    public void shout(){
        if(this.age >= 22){
            System.out.println("可以考虑结婚");
        }else{
            System.out.println("好好学习");
        }
    }
}
```

> 2、**Girl 类**

```java
public class Girl {

    private String name;
    private int age;
    
    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }
    
    public Girl(){
        
    }
    public Girl(String name, int age) {
        this.name = name;
        this.age = age;
    }
    
    public void marry(Boy boy){
        System.out.println("我想嫁给" + boy.getName());
    }
    /**
      * 
      * @Description 比较两个对象的大小
      * @author subei
      * @date 2020 年 4 月 21 日上午 9:17:35
      * @param girl
      * @return
     */
    public int compare(Girl girl){
//        if(this.age >girl.age){
//            return 1;
//        }else if(this.age < girl.age){
//            return -1;
//        }else{
//            return 0;
//        }
        
        return this.age - girl.age;
    }
    
}
```

> 3、**测试类**

```java
public class BoyGirlTest {

    public static void main(String[] args) {
        
        Boy boy = new Boy("罗密欧",21);
        boy.shout();
        
        Girl girl = new Girl("朱丽叶", 18);
        girl.marry(boy);
        
        Girl girl1 = new Girl("祝英台", 19);
        int compare = girl.compare(girl1);
        if(compare > 0){
            System.out.println(girl.getName() + "大");
        }else if(compare < 0){
            System.out.println(girl1.getName() + "大");
        }else{
            System.out.println("一样的");
        }
    }
}
```

> 2、练习2

**Account 类**

```java
public class Account {

    private int id; // 账号
    private double balance; // 余额
    private double annualInterestRate; // 年利率

    public void setId(int id) {

    }

    public double getBalance() {
        return balance;
    }

    public void setBalance(double balance) {
        this.balance = balance;
    }

    public double getAnnualInterestRate() {
        return annualInterestRate;
    }

    public void setAnnualInterestRate(double annualInterestRate) {
        this.annualInterestRate = annualInterestRate;
    }

    public int getId() {
        return id;
    }

    public void withdraw(double amount) { // 取钱
        if(balance < amount){
            System.out.println("余额不足，取款失败");
            return;
        }
        balance -= amount;
        System.out.println("成功取出" + amount);
    }

    public void deposit(double amount) { // 存钱
        if(amount > 0){
            balance += amount;
            System.out.println("成功存入" + amount);
        }
    }

    public Account(int id, double balance, double annualInterestRate) {
        this.id = id;
        this.balance = balance;
        this.annualInterestRate = annualInterestRate;
    }
    
    
}
```

**Customer 类**

```java
public class Customer {

    private String firstName;
    private String lastName;
    private Account account;

    public Customer(String f, String l) {
        this.firstName = f;
        this.lastName = l;
    }

    public String getFirstName() {
        return firstName;
    }

    public String getLastName() {
        return lastName;
    }

    public Account getAccount() {
        return account;
    }

    public void setAccount(Account account) {
        this.account = account;
    }
    
}
```

**CustomerTest 类**

```java
/*
 * 写一个测试程序。
 * （1）创建一个 Customer，名字叫 Jane Smith, 他有一个账号为 1000，
 * 余额为 2000 元，年利率为 1.23％的账户。
 * （2）对 Jane Smith 操作。存入 100 元，再取出 960 元。再取出 2000 元。
 * 打印出 Jane Smith 的基本信息
 * 
 * 成功存入：100.0
 * 成功取出：960.0
 * 余额不足，取款失败
 * Customer  [Smith,  Jane]  has  a  account:  id  is 1000, 
 *  annualInterestRate  is 1.23％,  balance  is 1140.0
 *  
 */
public class CustomerTest {

    public static void main(String[] args) {
        Customer cust = new Customer("Jane" , "Smith");
        
        Account acct = new Account(1000,2000,0.0123);
        
        cust.setAccount(acct);
        
        cust.getAccount().deposit(100); //存入 100
        cust.getAccount().withdraw(960); //取钱 960
        cust.getAccount().withdraw(2000); //取钱 2000
        
        System.out.println("Customer[" + cust.getLastName() + cust.getFirstName() + "]  has  a  account:  id  is "
                + cust.getAccount().getId() + ",annualInterestRate  is " + cust.getAccount().getAnnualInterestRate() * 100 + "%,  balance  is "
                + cust.getAccount().getBalance());
    }
}
```

> 3、练习3

**Account 类**

```java
public class Account {

    private double balance;

    public double getBalance() {
        return balance;
    }

    public Account(double init_balance){
        this.balance = init_balance;
    }
    
    //存钱操作
    public void deposit(double amt){
        if(amt > 0){
            balance += amt;
            System.out.println("存钱成功");
        }
    }
    
    //取钱操作
    public void withdraw(double amt){
        if(balance >= amt){
            balance -= amt;
            System.out.println("取钱成功");
        }else{
            System.out.println("余额不足");
        }
    }
}
```

**Customer 类**

```java
public class Customer {

    private String firstName;
    private String lastName;
    private Account account;
    
    public String getFirstName() {
        return firstName;
    }
    public String getLastName() {
        return lastName;
    }
    public Account getAccount() {
        return account;
    }
    public void setAccount(Account account) {
        this.account = account;
    }
    public Customer(String f, String l) {
        this.firstName = f;
        this.lastName = l;
    }    
}
```

**Bank 类**

```java
public class Bank {

    private int numberOfCustomers;    //记录客户的个数
    private Customer[] customers;    //存放多个客户的数组
    
    public Bank(){
        customers = new Customer[10];
    }
    
    //添加客户
    public void addCustomer(String f,String l){
        Customer cust = new Customer(f,l);
//        customers[numberOfCustomers] = cust;
//        numberOfCustomers++;
        customers[numberOfCustomers++] = cust;
    }

    //获取客户的个数
    public int getNumberOfCustomers() {
        return numberOfCustomers;
    }

    //获取指定位置上的客户
    public Customer getCustomers(int index) {
//        return customers;    //可能报异常
        if(index >= 0 && index < numberOfCustomers){
            return customers[index];
        }
        
        return null;
    }    
    
}
```

**BankTest 类**

```java
public class BankTest {

    public static void main(String[] args) {
        
        Bank bank = new Bank();
        
        bank.addCustomer("Jane", "Smith");    
        
        bank.getCustomers(0).setAccount(new Account(2000));
        
        bank.getCustomers(0).getAccount().withdraw(500);
        
        double balance = bank.getCustomers(0).getAccount().getBalance();
        
        System.out.println("客户: " + bank.getCustomers(0).getFirstName() + "的账户余额为：" + balance);
        
        System.out.println("***************************");
        bank.addCustomer("万里", "杨");
        
        System.out.println("银行客户的个数为: " + bank.getNumberOfCustomers());
        
    }
}
```

## 8、 关键字：package、import 的使用

### 8.1、关键字—package

```java
/*
 * 一、package 关键字的使用
 * 1.为了更好的实现项目中类的管理，提供包的概念
 * 2.使用 package 声明类或接口所属的包，声明在源文件的首行
 * 3.包，属于标识符，遵循标识符的命名规则、规范"见名知意"
 * 4.每“.”一次,就代表一层文件目录。
 * 
 * 补充:同一个包下，不能命名同名接口或同名类
 *     不同包下，可以命名同名的接口、类。
 *
 */
public class PackageImportTest {

}
```

> **JDK 中主要的包介绍**

```java
1.java.lang----包含一些 Java 语言的核心类，如 String、Math、Integer、System 和 Thread，提供常用功能
2.java.net----包含执行与网络相关的操作的类和接口。
3.java.io----包含能提供多种输入/输出功能的类。
4.java.util----包含一些实用工具类，如定义系统特性、接口的集合框架类、使用与日期日历相关的函数。
5.java.text----包含了一些 java 格式化相关的类
6.java.sql----包含了 java 进行 JDBC 数据库编程的相关类/接口
7.java.awt----包含了构成抽象窗口工具集（abstractwindowtoolkits）的多个类，这些类被用来构建和管理应用程序的图形用户界面(GUI)。B/S  C/S
```

### 8.2、MVC 设计模式

MVC 是常用的设计模式之一，将整个程序分为三个层次：**视图模型层，控制器层，数据模型层**。这种将程序输入输出、数据处理，以及数据的展示分离开来的设计模式使程序结构变的灵活而且清晰，同时也描述了程序各个对象间的通信方式，降低了程序的耦合性。

![null](https://i-blog.csdnimg.cn/blog_migrate/28e3ddc6d7e4ac634b0fe422a51298f5.png)



![null](https://i-blog.csdnimg.cn/blog_migrate/d8f8edff166a0783a893f349a4d93655.png)

### 8.3、关键字—import

```java
import java.util.*;

import account2.Bank;

/*
 * 二、import关键字的使用
 * import:导入
 * 1.在源文件中显式的使用import结构导入指定包下的类、接口
 * 2.声明在包的声明和类的声明之间
 * 3.如果需要导入多个结构，则并列写出即可
 * 4.可以使用"xxx.*"的方式,表示可以导入xxx包下的所有结构。
 * 5.如果导入的类或接口是java.lang包下的，或者是当前包下的，则可以省略此import语句。
 * 6.如果在代码中使用不同包下的同名的类。那么就需要使用类的全类名的方式指明调用的是哪个类。
 * 7.如果已经导入java.a包下的类。那么如果需要使用a包的子包下的类的话，仍然需要导入。
 * 8.import static组合的使用：调用指定类或接口下的静态的属性或方法.
 * 
 */
public class PackageImportTest {

    public static void main(String[] args) {
        String info = Arrays.toString(new int[]{1,2,3});
        
        Bank bank = new Bank();
        
        ArrayList list = new ArrayList();
        HashMap map = new HashMap();
        
        Scanner s = null;    
        
        System.out.println("hello");
        
        UserTest us = new UserTest();
        
    }
}
```

## 七：面向对象（中）

#### 文章目录

•01、继承性的使用与理解••1.1、继承性练习•02、方法的重写(override/overwrite)••2.1、方法重写的细节•2.2、方法的练习•03、四种访问权限修饰符•04、关键字：super•05、子类对象实例化过程•06、面向对象特征之三：多态性••6.1、虚拟方法的补充•6.2、向下转型的使用•6.3、多态性的练习•07、Object 类的使用••7.1、Object类中的主要结构•7.2、==操作符与equals方法••7.2.1、重写equals()方法的原则•7.3、toString的使用•08、包装类(Wrapper)的使用••8.1、单元测试方法的使用•8.2、包装类的使用•8.3、包装类与基本数据类型相互转换•8.4、练习•其他

## 01、继承性的使用与理解

> 1、Person 类

```java
/*
 * 为描述和处理个人信息，定义类 Person
 */
public class Person {
    
    String name;
    private int age;
    
    public Person(){
        
    }
    
    public Person(String name,int age){
        this.name = name;
        this.age = age;
    }
    
    public void eat(){
        System.out.println("吃饭");
        sleep();
    }
    
    private void sleep(){
        System.out.println("睡觉");
    }

    public int getAge() {
        return age;
    }

    public void setAge(int age) {
        this.age = age;
    }
    
}
```

> 2、Student 类

```java
/*
 * 为描述和处理学生信息，定义类 Student
 */
public class Student extends Person {

//    String name;
//    int age;
    String major;
    
    public Student(){
        
    }
    
    public Student(String name,int age,String major){
        this.name = name;
//        this.age = age;
        setAge(age);
        this.major = major;
    }
    
//    public void eat(){
//        System.out.println("吃饭");
//    }
//    
//    public void sleep(){
//        System.out.println("睡觉");
//    }
    
    public void study(){
        System.out.println("学习");
    }
    
    public void show(){
        System.out.println("name:" + name + ",age = " + getAge());
    }

}
```

> 3、测试类

```java
/*
 * 面向对象的特征二:继承性
 * 
 * 为什么要有继承？
 *         多个类中存在相同属性和行为时，将这些内容抽取到单独一个类中，
 *         那么多个类无需再定义这些属性和行为，只要继承那个类即可。
 *  * 一、继承性的好处
 * ① 减少了代码的冗余，提高了代码的复用性；
 * ② 便于功能的扩展；
 * ③ 为之后多态性的使用，提供了前提。
 * 
 * 二、继承性的格式
 *     class A extends B{}
 *  A:子类、派生类、subclass
 *  B:父类、超类、基类、superclass
 *  
 *  2.1 体现：一旦子类 A 继承父类以后，子类 A 中就获取了父类 B 中声明的结构：属性、方法
 *         特别的，父类中声明为 private 的属性或方法，子类继承父类以后，仍然认为获取了父类中私有的结构。
 *         只有因为封装性的影响，使得子类不能直接调用父类的结构而已。
 *  2.2 子类继承父类以后，还可以声明自己特有的属性或方法，实现功能的拓展。
 *      子类和父类的关系：不同于子集与集合的关系。
 *      extends:延展、扩展
 * 
 */
public class ExtendsTest {

    public static void main(String[] args) {
        Person p1 = new Person();
//        p1.age = 1;
        p1.eat();
        System.out.println("********************");
        
        Student s1 = new Student();
        s1.eat();
//        s1.sleep();
        s1.name = "Tom";
        
        s1.setAge(10);
        System.out.println(s1.getAge());
        
    }
}
```

![null](https://i-blog.csdnimg.cn/blog_migrate/d26726baa0748a4de4cf9da79d0ab81a.png)



![null](https://i-blog.csdnimg.cn/blog_migrate/905182236416f14e691ff4a191c86dd6.png)

> 3、Java 中关于继承性的规定

```java
/*  三、Java 中关于继承性的规定：
 *      1.一个类可以被多个类继承
 *      2.Java 中类的单继承性：一个类只能有一个父类
 *      3.子父类是相对的概念。
 *      4.子类直接继承的父类，称为：直接父类。间接继承的父类，称为，间接父类。
 *      5.子类继承父类后，就获取了直接父类以及所有间接父类中声明的属性和方法。
 *     
 * 四、1.如果我们没有显式的声明一个类的父类的话，则此类继承于 java.lang.Object 类
 *       2.所有的 java 类(除 java.long.Object 类之外)都直接或间接地继承于 java.lang.Object 类;
 *       3.意味着，所有的 java 类具有 java.lang.Object 类声明的功能。
 */
public class ExtendsTest {

    public static void main(String[] args) {    
        s1.brease();
        
        Creature c = new Creature();
        System.out.println(c.toString());
        
    }
}
```

> 4、将上述 Person 类改为如下

```java
public class Person extends Creature {
    ...
}
```

> 5、Creature 类

```java
public class Creature {

    public void brease(){
        System.out.println("呼吸");
    }
}
```

![null](https://i-blog.csdnimg.cn/blog_migrate/65793dc3b390b28d97f5acc7d971c795.png)

### 1.1、继承性练习

> 1、练习1

![null](https://i-blog.csdnimg.cn/blog_migrate/b951354b304b3d69d27454a5b4b01962.png)

```java
/*
 * 定义类Kids继承ManKind，并包括
 * 成员变量int yearsOld；
 * 方法printAge()打印yearsOld的值
 * 
 */
public class Kids extends ManKind{

    private int yearsOld;    //年限
    
    public Kids() {


    }

    public Kids(int yearsOld) {
        this.yearsOld = yearsOld;
    }

    public int getYearsOld() {
        return yearsOld;
    }

    public void setYearsOld(int yearsOld) {
        this.yearsOld = yearsOld;
    }

    public void printAge(){
        System.out.println("I am " + yearsOld);
    }
}
```

ManKind类

```java
/*
 * 定义一个ManKind类，包括
 * 成员变量int sex和int salary；
 * 方法void manOrWoman()：根据sex的值显示“man”(sex==1)或者“woman”(sex==0)；
 * 方法void employeed()：根据salary的值显示“no job”(salary==0)或者“job”(salary!=0)。
 * 
 */
public class ManKind {

    private int sex;    //性别
    private int salary;    //薪资
    
    public ManKind() {
        
    }

    public ManKind(int sex, int salary) {
        this.sex = sex;
        this.salary = salary;
    }

    public void manOrWoman(){
        if(sex==1){
            System.out.println("man");
        }else if(sex==0){
            System.out.println("woman");
        }
    }
    
    public void employeed(){
        if(salary==0){
            System.out.println("no job");
        }else if(salary!=0){
            System.out.println("job");
        }
    }

    public int getSex() {
        return sex;
    }

    public void setSex(int sex) {
        this.sex = sex;
    }

    public int getSalary() {
        return salary;
    }

    public void setSalary(int salary) {
        this.salary = salary;
    }
    
}
```

KidsTest

```java
/*
 * 定义类KidsTest，在类的main方法中实例化Kids的对象someKid，
 * 用该对象访问其父类的成员变量及方法。
 * 
 */
public class KidsTest {
    public static void main(String[] args) {
        
        Kids someKid = new Kids(12);
        
        someKid.printAge();
        
        someKid.setYearsOld(15);
        someKid.setSalary(0);
        someKid.setSex(1);
        
        someKid.employeed();
        someKid.manOrWoman();
    }
}
```

> 2、练习2

![null](https://i-blog.csdnimg.cn/blog_migrate/9ceff974c6d6d937fc91570a49d52838.png)

```java
public class Circle {

    public double radius;    //半径
    
    public Circle(){
        radius = 1.0;
    }

    public double getRadius() {
        return radius;
    }

    public void setRadius(double radius) {
        this.radius = radius;
    }
    
    public double findArea(){    //计算圆的面积
        return Math.PI * radius * radius;
    }
}
```

Cylinder类

```java
public class Cylinder extends Circle{

    private double length;
    
    public Cylinder(){
        length = 1.0;
    }

    public double getLength() {
        return length;
    }

    public void setLength(double length) {
        this.length = length;
    }
    
    public double findVolume(){    //计算圆柱体积
        return findArea() * length;
    }
}
```

测试类

```java
public class CylinderTest {
    public static void main(String[] args) {
        
        Cylinder cy = new Cylinder();
        
        cy.setRadius(2.1);
        cy.setLength(3.4);
        double volues = cy.findVolume();
        System.out.println("圆柱的体积:" + volues);
        
        double area = cy.findArea();
        System.out.println("圆的面积: " + area);
    }
}
```

## 02、方法的重写(override/overwrite)

> 1、Person类

```java
public class Person {

    String name;
    int age;
    
    public Person(){
        
    }
    
    public Person(String name,int age){
        this.name = name;
        this.age = age;
    }
    
    public void eat(){
        System.out.println("吃饭");
    }
    
    public void walk(int distance){
        System.out.println("走路，走的距离是：" + distance + "公里");
        show();
    }
    
    private void show(){
        System.out.println("我是一个人。");
    }
    
    public Object info(){
        return null;
    }
    
    public double info1(){
        return 1.0;
    }
}
```

> 2、Student类

```java
public class Student extends Person{

    String major;
    
    public Student(){
        
    }
    
    public Student(String major){
        this.major = major;
    }
    
    public void study(){
        System.out.println("学习，专业是:" + major);
    }
    
    //对父类中的eat()进行了重写
    public void eat(){
        System.out.println("学生应该多吃有营养的。");
    }
    
    public void show(){
        System.out.println("我是一个学生。");
    }
    
    public String info(){
        return null;
    }
    
    //不是一个类型，所以报错。
//    public int info1(){
//        return 1;
//    }
    
    //可以直接将父类的方法的第一行粘过来，直接写方法体
//    public void walk(int distance){
//        System.out.println("重写的方法");
//    }
    
    //直接输入父类的方法名，Alt + /，选择即可生成
    @Override
    public void walk(int distance) {
        System.out.println("自动生成");
    }
}
```

> 3、测试类

```java
/*
 * 方法的重写(override/overwrite)
 * 
 * 1.重写：子类继承父类以后，可以对父类中的方法进行覆盖操作。
 * 2.应用：重写以后，当创建子类对象以后，通过子类对象去调用子父类中同名同参数方法时，执行的是子类重写父类的方法。
 *   即在程序执行时，子类的方法将覆盖父类的方法。
 * 
 * 面试题：区分方法的重载与重写(有的书也叫做“覆盖”)
 *         答：方法的重写Overriding和重载Overloading是Java多态性的不同表现。
 *         重写Overriding是父类与子类之间多态性的一种表现，重载Overloading是一个类中多态性的一种表现。
 *         如果在子类中定义某方法与其父类有相同的名称和参数，我们说该方法被重写 (Overriding)。
 *         子类的对象使用这个方法时，将调用子类中的定义，对它而言，父类中的定义如同被"屏蔽"了。
 *         如果在一个类中定义了多个同名的方法，它们或有不同的参数个数或有不同的参数类型，则称为方法的重载(Overloading)。
 * 
 */
public class PersonTest {


    public static void main(String[] args) {
        Student s = new Student("计算机科学与技术");
        s.eat();
        s.walk(10);
        
        s.study();
    }
}
```

### 2.1、方法重写的细节

> 1、Person类

```java
public class Person {

    String name;
    int age;
    
    public Person(){
        
    }
    
    public Person(String name,int age){
        this.name = name;
        this.age = age;
    }
    
//    public void eat(){
//        System.out.println("吃饭");
//    }
    static void eat(){
        System.out.println("吃饭");
    }
    
    public void walk(int distance){
        System.out.println("走路，走的距离是：" + distance + "公里");
        show();
    }
    
    private void show(){
        System.out.println("我是一个人。");
    }
    
    public Object info(){
        return null;
    }
    
    public double info1(){
        return 1.0;
    }
}
```

> 2、Student类

```java
public class Student extends Person{

    String major;
    
    public Student(){
        
    }
    
    public Student(String major){
        this.major = major;
    }
    
    public void study(){
        System.out.println("学习，专业是:" + major);
    }
    
    //对父类中的eat()进行了重写
//    public void eat(){
//        System.out.println("学生应该多吃有营养的。");
//    }
    
    //这样不会报错，但已经不是重写了！！
    public static void eat(){
        System.out.println("学生应该多吃有营养的。");
    }
    
    public void show(){
        System.out.println("我是一个学生。");
    }
    
    public String info(){
        return null;
    }
    
    //不是一个类型，所以报错。
//    public int info1(){
//        return 1;
//    }
    
    //可以直接将父类的方法的第一行粘过来，直接写方法体
//    public void walk(int distance){
//        System.out.println("重写的方法");
//    }
    
    //直接输入父类的方法名，Alt + /，选择即可生成
    @Override
    public void walk(int distance) {
        System.out.println("自动生成");
    }
}
```

> 3、测试类

```java
/*
 * 3.重写的规定：
 *         方法的声明：权限修饰符 返回值类型 方法名(形参列表){
 *                         //方法体
 *                  }
 *         约定俗称:子类中的叫重写的方法，父类中的叫被重写的方法。
 *         ① 子类重写的方法的方法名和形参列表必须和父类被重写的方法的方法名、形参列表相同; 
 *         ② 子类重写的方法使用的访问权限不能小于父类被重写的方法的访问权限,
 *           特殊情况: 子类不能重写父类中声明为private权限的方法;
 *       ③ 返回值类型:
 *           > 父类被重写的方法的返回值类型是void,则子类重写的方法的返回值类型只能是void;
 *           > 父类被重写的方法的返回值类型是A类型，则子类重写的方法的返回值类型可以是A类或A类的子类;
 *           > 父类被重写的方法的返回值类型如果是基本数据类型(比如:double)，则子类重写的方法的返回值类型必须是相同的基本数据类型(必须是:double)。
 *           
 *       ④ 子类方法抛出的异常不能大于父类被重写的方法抛出的异常;
 * 
 * 注意：子类与父类中同名同参数的方法必须同时声明为非static的(即为重写)，或者同时声明为static的（不是重写）。
 *         因为static方法是属于类的，子类无法覆盖父类的方法。
 */
public class PersonTest {


    public static void main(String[] args) {
        Student s = new Student("计算机科学与技术");
        s.eat();
        s.walk(10);
        System.out.println("*******************");
        
        s.study();
        
        Person p1 = new Person();
        p1.eat();
    }
}
```

### 2.2、方法的练习

> 1、练习1

```java
1.如果现在父类的一个方法定义成private访问权限，在子类中将此方法声明为default访问权限，那么这样还叫重写吗？(NO)
1
```

> 2、练习2

```java
/*
 * 2.修改练习1.2中定义的类Kids，在Kids中重新定义employeed()方法，
 *       覆盖父类ManKind中定义的employeed()方法，
 *   输出“Kids should study and no job.”
 */
public class Kids extends ManKind{

    private int yearsOld;    //年限
    
    public Kids() {

    }

    public Kids(int yearsOld) {
        this.yearsOld = yearsOld;
    }

    public int getYearsOld() {
        return yearsOld;
    }

    public void setYearsOld(int yearsOld) {
        this.yearsOld = yearsOld;
    }

    public void printAge(){
        System.out.println("I am " + yearsOld);
    }
    
    public void employeed(){
        System.out.println("Kids should study and no job.");
    }
}
```

MindKids类

```java
public class ManKind {

    private int sex;    //性别
    private int salary;    //薪资
    
    public ManKind() {
        
    }

    public ManKind(int sex, int salary) {
        this.sex = sex;
        this.salary = salary;
    }

    public void manOrWoman(){
        if(sex==1){
            System.out.println("man");
        }else if(sex==0){
            System.out.println("woman");
        }
    }
    
    public void employeed(){
        if(salary==0){
            System.out.println("no job");
        }else if(salary!=0){
            System.out.println("job");
        }
    }

    public int getSex() {
        return sex;
    }

    public void setSex(int sex) {
        this.sex = sex;
    }

    public int getSalary() {
        return salary;
    }

    public void setSalary(int salary) {
        this.salary = salary;
    }
    
}
```

测试类

```java
public class KidsTest {
    public static void main(String[] args) {
        
        Kids someKid = new Kids(12);
        
        someKid.printAge();
        
        someKid.setYearsOld(15);
        someKid.setSalary(0);
        someKid.setSex(1);
        
        someKid.employeed();
        someKid.manOrWoman();
    }
}
```

## 03、四种访问权限修饰符

> 四种权限修饰符

![null](https://i-blog.csdnimg.cn/blog_migrate/964e56c1505ce51660efb495e43697eb.png)

> Order类

```java
package githubb;
/*
 * 体会四种不同的权限修饰符
 */
public class Order {

    private int orderPrivate;
    int orderDefault;
    protected int orderProtected;
    public int orderPublic;
    
    private void methodPrivate(){
        orderPrivate = 1;
        orderDefault = 2;
        orderProtected = 3;
        orderPublic = 4;
    }
    
    void methodDefault(){
        orderPrivate = 1;
        orderDefault = 2;
        orderProtected = 3;
        orderPublic = 4;
    }
    
    protected void methodProtected(){
        orderPrivate = 1;
        orderDefault = 2;
        orderProtected = 3;
        orderPublic = 4;
    }
    
    public void methodPublic(){
        orderPrivate = 1;
        orderDefault = 2;
        orderProtected = 3;
        orderPublic = 4;
    }
}
```

> Ordertest类

```java
package githubb;

public class OrderTest {
    public static void main(String[] args) {
        
        Order order = new Order();
        
        order.orderDefault = 1;
        order.orderProtected = 2;
        order.orderPublic = 3;
        
        order.methodDefault();
        order.methodProtected();
        order.methodPublic();
        
        //同一个包中的其它类，不可以调用Order类中私有的属性
//        order.orderPrivate = 4;    //The field Order.orderPrivate is not visible
//        order.methoPrivate();
    }
}
```

> SubOrder类

```java
package githubc;

import githubb.Order;

public class SubOrder extends Order{

    public void method(){
        orderProtected = 1;
        orderPublic = 2;
        
        methodProtected();
        methodPublic();
        
        //在不同包的子类中，不能调用Order类中声明为private和缺省的权限的属性、方法
//        orderDefault = 3;
//        orderPrivate = 4;
//        
//        methodDefault();
//        methodPrivate();
    }
}
```

> OrderTest类

```java
package githubc;

import githubb.Order;

public class OrderTest {
    public static void main(String[] args) {
        
        Order order = new Order();
        order.orderPublic = 1;
        order.methodPublic();
        
        //不同包下的普通类(非子类)要使用Order类，不可以调用声明为private、缺省、protected权限的属性、方法。
//        order.orderPrivate = 2;
//        order.orderProtected = 3;
//        order.orderProtected = 4;
//        
//        order.methodPrivate();
//        order.methodDefault();
//        order.methodProtected();
        
    }
    
    public void show(Order order){
        order.orderPublic = 1;
        order.methodPublic();
        
        //不同包下的普通类(非子类)要使用Order类，不可以调用声明为private、缺省、protected权限的属性、方法。
//        order.orderPrivate = 2;
//        order.orderProtected = 3;
//        order.orderProtected = 4;
//        
//        order.methodPrivate();
//        order.methodDefault();
//        order.methodProtected();
    }
}
```

## 04、关键字：super

> Person类

```java
public class Person {

    String name;
    int age;
    int id = 1003;    //身份证号
    
    public Person(){
        System.out.println("我无处不在");
    }
    
    public Person(String name){
        this.name = name;
    }
    
    public Person(String name,int age){
        this(name);
        this.age = age;
    }
    
    public void eat(){
        System.out.println("人，吃饭");
    }
    
    public void walk(){
        System.out.println("人，走路");
    }
}
```

> Student类

```java
public class Student extends Person{
    
    String major;
    int id = 1002;    //学号
    
    public Student(){

    }
    
    public Student(String name,int age,String major){
//        this.age = age;
//        this.name = name;
        super(name,age);
        this.major = major;
    }
    
    public Student(String major){
        this.major = major;
    }
    
    public void eat(){
        System.out.println("学生多吃有营养的食物");
    }
    
    public void Study(){
        System.out.println("学生，学习知识。");
        this.eat();
        //如果，想调用父类中被重写的，不想调用子类中的方法，可以：
        super.eat();
        super.walk();//子父类中未重写的方法，用"this."或"super."调用都可以
    }
    public void show(){
        System.out.println("name = " + this.name + ",age = " + super.age);
        System.out.println("id = " + this.id);    
        System.out.println("id = " + super.id);
    }
}
```

> 测试类

```java
/*
 * super关键字的使用
 * 1.super理解为:父类的
 * 2.super可以用来调用:属性、方法、构造器 
 * 
 * 3.super的使用
 *         3.1 我们可以在子类的方法或构造器中，通过"super.属性"或"super.方法"的方式，显式的调用
 *     父类中声明的属性或方法。但是，通常情况下，我们习惯去省略这个"super."
 *         3.2 特殊情况:当子类和父类中定义了同名的属性时，我们要想在子类中调用父类中声明的属性，则必须显式的 
 *  使用"super.属性"的方式，表明调用的是父类中声明的属性。
 *      3.3 特殊情况:当子类重写了父类中的方法后，我们想在子类的方法中调用父类中被重写的方法时，必须显式的
 *  使用"super.方法"的方式，表明调用的是父类中被重写的方法。
 * 
 * 4.super调用构造器
 *       4.1  我们可以在子类的构造器中显式的使用"super(形参列表)"的方式,调用父类中声明的指定的构造器
 *       4.2 "super(形参列表)"的使用，必须声明在子类构造器的首行！
 *    4.3 我们在类的构造器中，针对于"this(形参列表)"或"super(形参列表)"只能二选一，不能同时出现。
 *    4.4 在构造器的首行，既没有显式的声明"this(形参列表)"或"super(形参列表)",则默认的调用的是父类中的空参构造器。super()
 *    4.5 在类的多个构造器中，至少有一个类的构造器使用了"super(形参列表)",调用父类中的构造器。
 *  
 */
public class SuperTest {
    public static void main(String[] args) {
        
        Student s = new Student();
        s.show();
        
        s.Study();
        
        Student s1 = new Student("Ton",21,"IT" );
        s1.show();
        
        System.out.println("***********************");
        Student s2 = new Student();
        
    }
}
```

## 05、子类对象实例化过程

![null](https://i-blog.csdnimg.cn/blog_migrate/2121c3c0187e95e5a56fa82a74bde8cc.png)



![null](https://i-blog.csdnimg.cn/blog_migrate/d01ee802f2e258931b867ba1d747877b.png)

```java
/*
 * 子类对象实例化的全过程
 * 
 * 1.从结果上看:
 *         子类继承父类以后，就获取了父类中声明的属性或方法。
 *         创建子类的对象中，在堆空间中，就会加载所有父类中声明的属性。
 * 
 * 2.从过程上看:
 *         当我们通过子类的构造器创建子类对象时,我们一定会直接或间接的调用其父类构造器， 
 *         直到调用了java.lang.Object类中空参的构造器为止。正因为加载过所有的父类结构，所以才可以看到内存中有
 *         父类中的结构，子类对象可以考虑进行调用。
 * 
 * 明确:虽然创建子类对象时，调用了父类的构造器，但自始至终就创建过一个对象，即为new的子类对象。
 */
public class InstanceTest {

}
```

> 练习

Account类

```java
/*
 * 写一个名为Account的类模拟账户。该类的属性和方法如下图所示。
 * 该类包括的属性：账号id，余额balance，年利率annualInterestRate；
 * 包含的方法：访问器方法（getter和setter方法），
 * 返回月利率的方法getMonthlyInterest()，
 * 取款方法withdraw()，存款方法deposit()。
 * 
 */
public class Account {

    private int id;    //账号
    private double balance;    //余额
    private double annualInterestRate;    //年利率
    
    public Account(int id, double balance, double annualInterestRate) {
        super();
        this.id = id;
        this.balance = balance;
        this.annualInterestRate = annualInterestRate;
    }

    public int getId() {
        return id;
    }

    public void setId(int id) {
        this.id = id;
    }

    public double getBalance() {
        return balance;
    }

    public void setBalance(double balance) {
        this.balance = balance;
    }

    public double getAnnualInterestRate() {
        return annualInterestRate;
    }

    public void setAnnualInterestRate(double annualInterestRate) {
        this.annualInterestRate = annualInterestRate;
    }
    
    public double getMonthlyInterest(){    //返回月利率的方法
        return annualInterestRate / 12;
    }
    
    public void withdraw (double amount){    //取款方法
        if(balance >= amount){
            balance -= amount;
            return;
        }
        System.out.println("余额不足");
    }
    
    public void deposit (double amount){    //存款方法
        if(amount > 0){
            balance += amount;
            
        }
    }
    
}
```

AccountTest类

```java
/*
 * 写一个用户程序测试Account类。在用户程序中，
 * 创建一个账号为1122、余额为20000、年利率4.5%的Account对象。
 * 使用withdraw方法提款30000元，并打印余额。再使用withdraw方法提款2500元，
 * 使用deposit方法存款3000元，然后打印余额和月利率。
 */
public class AccountTest {
    public static void main(String[] args) {
        Account acct = new Account(1122,20000,0.045);
        
        acct.withdraw(30000);
        System.out.println("你的账户余额为:" + acct.getBalance());
        acct.withdraw(2500);
        System.out.println("你的账户余额为:" + acct.getBalance());
        acct.deposit(3000);
        System.out.println("你的账户余额为:" + acct.getBalance());


        System.out.println("月利率为: " + (acct.getAnnualInterestRate() * 100) + "%");
    }
}
```

CheckAccount类

```java
/*
 * 创建Account类的一个子类CheckAccount代表可透支的账户，该账户中定义一个属性overdraft代表可透支限额。
 * 在CheckAccount类中重写withdraw方法，其算法如下：
 * 如果（取款金额<账户余额），
 * 可直接取款
 * 如果（取款金额>账户余额），
 * 计算需要透支的额度
 * 判断可透支额overdraft是否足够支付本次透支需要，如果可以
 *         将账户余额修改为0，冲减可透支金额
 * 如果不可以
 *         提示用户超过可透支额的限额
 * 
 */
public class CheckAccount extends Account{

    private double overdraft;    //代表可透支限额
    
    public CheckAccount(int id, double balance, double annualInterestRate,double overdraft){
        super(id, balance, annualInterestRate);
        this.overdraft = overdraft;
    }
    
    public double getOverdraft() {
        return overdraft;
    }

    public void setOverdraft(double overdraft) {
        this.overdraft = overdraft;
    }

    @Override
    public void withdraw(double amount) {
        if(getBalance() >= amount){    //余额足够消费
            //方式一
//            setBalance(getBalance() - amount); 
            //方式二
            super.withdraw(amount);
        }else if(overdraft >= amount - getBalance()){    //余额不够
            
            overdraft -= (amount - getBalance());
//            setBalance(0);
            //或
            super.withdraw(getBalance());
            
        }else{    //超过可透支限额
            System.out.println("超过可透支限额！");
        }
        
    }
}
```

CheckAccountTest类

```java
/*
 * 写一个用户程序测试CheckAccount类。在用户程序中，
 * 创建一个账号为1122、余额为20000、年利率4.5%，
 * 可透支限额为5000元的CheckAccount对象。
 * 使用withdraw方法提款5000元，并打印账户余额和可透支额。
 * 再使用withdraw方法提款18000元，并打印账户余额和可透支额。
 * 再使用withdraw方法提款3000元，并打印账户余额和可透支额。
 * 
 */
public class CheckAccountTest {
    public static void main(String[] args) {
        CheckAccount cat = new CheckAccount(1122,20000,0.045,5000);
        
        cat.withdraw(5000);
        System.out.println("您的账户余额为: " + cat.getBalance());
        System.out.println("您的可透支额度为: " + cat.getOverdraft());
        
        cat.withdraw(18000);
        System.out.println("您的账户余额为: " + cat.getBalance());
        System.out.println("您的可透支额度为: " + cat.getOverdraft());
        
        cat.withdraw(3000);
        System.out.println("您的账户余额为: " + cat.getBalance());
        System.out.println("您的可透支额度为: " + cat.getOverdraft());
    }
}
```

## 06、面向对象特征之三：多态性

> Person类

```java
public class Person {
    String name;
    int age;
    
    public void eat(){
        System.out.println("人，吃饭");
    }
    
    public void walk(){
        System.out.println("人，走路");
    }
    
}
```

> Woman类

```java
public class Woman extends Person{

    boolean isBeauty;
    
    public void goShopping(){
        System.out.println("女人喜欢购物");
    }
    
    public void eat(){
        System.out.println("女人少吃，为了减肥。");
    }
    
    public void walk(){
        System.out.println("女人，窈窕的走路。");
    }
}
```

> Man类

```java
public class Man extends Person{
    
    boolean isSmoking;
    
    public void earnMoney(){
        System.out.println("男人负责工作养家");
    }
    
    public void eat() {
        System.out.println("男人多吃肉，长肌肉");
    }
    
    public void walk() {
        System.out.println("男人霸气的走路");
    }
}
```

> 测试类

```java
/*
 * 面向对象之三:多态性
 * 
 * 1.理解多态性:可以理解为一个事物的多种态性。
 * 2.何为多态性:
 *      对象的多态性:父类的引用指向子类的对象(或子类的对象赋值给父类的引用)
 * 
 * 3.多态的使用：虚拟方法调用
 *     有了对象多态性以后，我们在编译期，只能调用父类声明的方法，但在执行期实际执行的是子类重写父类的方法
 *             简称：编译时，看左边；运行时，看右边。
 *  
 *  若编译时类型和运行时类型不一致，就出现了对象的多态性(Polymorphism)
 *  多态情况下，
 *      “看左边”：看的是父类的引用（父类中不具备子类特有的方法）
 *      “看右边”：看的是子类的对象（实际运行的是子类重写父类的方法）
 *  
 *  4.多态性的使用前提：
 *      ① 类的继承关系
 *      ② 方法的重写
 *  5.对象的多态性:只适用于方法，不适用于属性(编译和运行都看左边)
 */
public class PersonTest {
    public static void main(String[] args) {
        
    Person p1 = new Person();
    p1.eat();
    
    Man man = new Man();
    man.eat();
    man.age = 25;
    man.earnMoney();
    
    //************************************
    //对象的多态性，父类的引用指向子类的对象
    Person p2 = new Man();
//    Person p3 = new Woman();
    
    //多态的使用:当调用子父类同名同参数方法时，实际调用的是子类重写父类的方法---虚拟方法调用
    p2.eat();
    p2.walk();
    
//    p2.earnMoney();
    
    }
}
```

> 举例

```java
/*
 * 多态性应用举例
 */
public class AnimalTest {
    
    public static void main(String[] args) {
        AnimalTest test = new AnimalTest();
        test.func(new Dog());
        
        test.func(new Cat());
    }

    public void func(Animal animal){    //Animal animal = new Dog();
        animal.eat();
        animal.shout();
    }
    
    //如果没有多态性，就会写很多如下的方法，去调用
    public void func(Dog dog){
        dog.eat();
        dog.shout();
    }
    
    public void func(Cat cat){
        cat.eat();
        cat.shout();
    }
}

class Animal{
    
    public void eat(){
        System.out.println("动物，进食");
    }
    
    public void shout(){
        System.out.println("动物：叫");
    }
}

class Dog extends Animal{
    public void eat(){
        System.out.println("狗吃骨头");
    }
    
    public void shout() {
        System.out.println("汪！汪！汪！");
    }
}

class Cat extends Animal{
    public void eat(){
        System.out.println("猫吃鱼");
    }
    
    public void shout() {
        System.out.println("喵！喵！喵！");
    }
}
```

### 6.1、虚拟方法的补充

```java
import java.util.Random;
/*
 * 2.从编译和运行的角度看：
 * 重载，是指允许存在多个同名方法，而这些方法的参数不同。
 * 编译器根据方法不同的参数表，对同名方法的名称做修饰。
 * 对于编译器而言，这些同名方法就成了不同的方法。
 * 它们的调用地址在编译期就绑定了。Java的重载是可以包括父类和子类的，
 * 即子类可以重载父类的同名不同参数的方法。所以：对于重载而言，在方法调用之前，
 * 编译器就已经确定了所要调用的方法，这称为“早绑定”或“静态绑定”；
 * 而对于多态，只有等到方法调用的那一刻，解释运行器才会确定所要调用的具体方法，
 * 这称为“晚绑定”或“动态绑定”。
 * 
 * 引用一句Bruce Eckel的话：“不要犯傻，如果它不是晚绑定，它就不是多态。”
 */
//面试题：多态是编译时行为还是运行时行为？
//证明如下：
class Animal  {
 
    protected void eat() {
        System.out.println("animal eat food");
    }
}

class Cat  extends Animal  {
 
    protected void eat() {
        System.out.println("cat eat fish");
    }
}

class Dog  extends Animal  {
 
    public void eat() {
        System.out.println("Dog eat bone");

    }

}

class Sheep  extends Animal  {
 
    public void eat() {
        System.out.println("Sheep eat grass");

    }
 
}

public class InterviewTest {

    public static Animal  getInstance(int key) {
        switch (key) {
        case 0:
            return new Cat ();
        case 1:
            return new Dog ();
        default:
            return new Sheep ();
        }

    }

    public static void main(String[] args) {
        int key = new Random().nextInt(3);

        System.out.println(key);

        Animal  animal = getInstance(key);
        
        animal.eat();
         
    }

}
```

### 6.2、向下转型的使用

> Person 类

```java
public class Person {
    String name;
    int age;
    
    public void eat(){
        System.out.println("人，吃饭");
    }
    
    public void walk(){
        System.out.println("人，走路");
    }
    
}
```

> Man 类

```java
public class Man extends Person{
    
    boolean isSmoking;
    
    public void earnMoney(){
        System.out.println("男人负责工作养家");
    }
    
    public void eat() {
        System.out.println("男人多吃肉，长肌肉");
    }
    
    public void walk() {
        System.out.println("男人霸气的走路");
    }
}
```

> Woman 类

```java
public class Woman extends Person{

    boolean isBeauty;
    
    public void goShopping(){
        System.out.println("女人喜欢购物");
    }
    
    public void eat(){
        System.out.println("女人少吃，为了减肥。");
    }
    
    public void walk(){
        System.out.println("女人，窈窕的走路。");
    }
}
```

> PersonTest 类

```java
/*
 * 面向对象之三:多态性
 * 
 * 1.理解多态性:可以理解为一个事物的多种态性。
 * 2.何为多态性:
 *      对象的多态性:父类的引用指向子类的对象(或子类的对象赋值给父类的引用)
 * 
 * 3.多态的使用：虚拟方法调用
 *     有了对象多态性以后，我们在编译期，只能调用父类声明的方法，但在执行期实际执行的是子类重写父类的方法
 *             简称：编译时，看左边；运行时，看右边。
 *  
 *  若编译时类型和运行时类型不一致，就出现了对象的多态性(Polymorphism)
 *  多态情况下，
 *      “看左边”：看的是父类的引用（父类中不具备子类特有的方法）
 *      “看右边”：看的是子类的对象（实际运行的是子类重写父类的方法）
 *  
 *  4.多态性的使用前提：
 *      ① 类的继承关系
 *      ② 方法的重写
 *  5.对象的多态性:只适用于方法，不适用于属性(编译和运行都看左边)
 */
public class PersonTest {
    public static void main(String[] args) {

        Person p1 = new Person();
        p1.eat();

        Man man = new Man();
        man.eat();
        man.age = 25;
        man.earnMoney();

        // ************************************
        System.out.println("************************");
        // 对象的多态性，父类的引用指向子类的对象
        Person p2 = new Man();
        // Person p3 = new Woman();

        // 多态的使用:当调用子父类同名同参数方法时，实际调用的是子类重写父类的方法---虚拟方法调用
        p2.eat();
        p2.walk();

        // p2.earnMoney();

        System.out.println("**************************");
        // 不能调用子类所特有的方法、属性，编译时，p2是Person类型，

        // p2.earnMoney();

        p2.name = "Tom";
        // p2.isSmoking = true;
        // 有了对象的多态性以后，内存中实际上是加载了子类特有的属性和方法，但是由于变量声明为父类类型，导致
        // 编译时，只能调用父类中声明的属性和方法。子类的属性和方法不能调用。

        // 如何才能调用子类所特有的属性和方法？
        // 使用强制类型转换符，也可称为:向下转型
        Man m1 = (Man) p2;
        m1.earnMoney();
        m1.isSmoking = true;

        // 使用强转时，可能出现ClassCastException异常
        // Woman w1 = (Woman)p2;
        // w1.goShopping();

        /*
         * instanceof关键字的使用
         * 
         * a instanceof A:判断对象a是否是类A的实例。如果，返回true，如果不是，返回false;
         * 
         * 使用情境:为了避免在向下转型时出现ClassCastException异常，我们在进行向下转型之前，先进行
         * instanceof的判断,一旦返回true,就进行向下转型。如果返回false，不进行向下转型。
         * 
         * 如果a instanceof A返回true,则a instanceof B也返回true。 其中类B是类A的父类。
         * 
         */

        if (p2 instanceof Woman) {
            Woman w1 = (Woman) p2;
            w1.goShopping();
            System.out.println("**********Woman*********");
        }

        if (p2 instanceof Man) {
            Man m2 = (Man) p2;
            m2.earnMoney();
            System.out.println("*********Man************");
        }

        if (p2 instanceof Person) {
            System.out.println("***********Person************");
        }

        if (p2 instanceof Object) {
            System.out.println("***********object************");
        }
        
        //向下转型的常见问题
        //练习
        //问题1:编译时通过，运行时不通过
        //举例一
//        Person p3 = new Woman();
//        Man m3 = (Man)p3;
        
        //举例二
        Person p4 = new Person();
        Man m4 = (Man)p4;
        
        //问题二:编译通过，运行时也通过
        Object obj = new Woman();
        Person p = (Person)obj;
        
        //问题三:编译不通过
//        Man m5 = new woman();
        
//        String str = new Date();
        
//        Object o = new Date();
//        String str1 = (String)o;
    }
}
```

![null](https://i-blog.csdnimg.cn/blog_migrate/53daf729ad837653a4122dbe2a002d65.png)

### 6.3、多态性的练习

> 1、练习1

```java
/*
 * 练习:子类继承父类
 * 
 * 1.若子类重写了父类方法，就意味着子类里定义的方法彻底覆盖了父类里的同名方法，
 * 系统将不可能把父类里的方法转移到子类中。
 * 
 * 2.对于实例变量则不存在这样的现象，即使子类里定义了与父类完全相同的实例变量，
 * 这个实例变量依然不可能覆盖父类中定义的实例变量
 * 
 */
public class FieldMethodTest {
    public static void main(String[] args){
        Sub s= new Sub();
        System.out.println(s.count);    //20
        s.display();//20
        
        Base b = s;
        //==:对于引用数据类型来讲，比较的是两个引用数据类型变量的地址值是否一样。
        System.out.println(b == s);    //true
        System.out.println(b.count);    //10
        b.display();
    }
}

class Base {
    int count= 10;
    public void display() {
        System.out.println(this.count);
    }
}

class Sub extends Base {
    int count= 20;
    public void display() {
        System.out.println(this.count);
    }
}
```

> 2、练习2

```java
/*
 * 建立InstanceTest 类，在类中定义方法method(Person e);
 * 
 * 在method中:
 * (1)根据e的类型调用相应类的getInfo()方法。
 * (2)根据e的类型执行：
 *         如果e为Person类的对象，输出：“a person”;
 *         如果e为Student类的对象，输出：“a student”“a person ”
 *         如果e为Graduate类的对象，输出：“a graduated student”
 *         “a student” “a person”
 * 
 */
class Person {
    protected String name = "person";
    protected int age = 50;


    public String getInfo() {
        return "Name: " + name + "\n" + "age: " + age;
    }
}

class Student extends Person {
    protected String school = "pku";

    public String getInfo() {
        return "Name: " + name + "\nage: " + age + "\nschool: " + school;
    }
}

class Graduate extends Student {
    public String major = "IT";

    public String getInfo() {
        return "Name: " + name + "\nage: " + age + "\nschool: " + school + "\nmajor:" + major;
    }
}


public class InstanceTest{
    
    public static void main(String[] args) {
        //虚拟方法调用
        InstanceTest test = new InstanceTest();
        test.method(new Student());
        
    }
    
    public void method(Person e){
        String info = e.getInfo();
        System.out.println(info);
        
        //方法一
        if(e instanceof Graduate){
            System.out.println("a graduated student");
            System.out.println("a student");
            System.out.println("a person");
        }else if(e instanceof Student){
            System.out.println("a student");
            System.out.println("a person");
        }else{
            System.out.println("a person");
        }
        
        //方法二
        if(e instanceof Graduate){
            System.out.println("a graduated student");
        }
        if(e instanceof Student){
            System.out.println("a student");
        }
        if(e instanceof Person){
            System.out.println("a person");
        }
    }
}
```

> 3、练习3

GeometricObject类

```java
/*
 * 定义三个类，父类GeometricObject代表几何形状，子类Circle代表圆形，MyRectangle代表矩形。
 */
public class GeometricObject {
    protected String color;
    protected double weight;
    public String getColor() {
        return color;
    }
    public void setColor(String color) {
        this.color = color;
    }
    public double getWeight() {
        return weight;
    }
    public void setWeight(double weight) {
        this.weight = weight;
    }
    public GeometricObject(String color, double weight) {
        super();
        this.color = color;
        this.weight = weight;
    }
    
    public double findArea(){
        return 0.0;
    }
}
```

Circle类

```java
public class Circle extends GeometricObject {

    private double radius;
    
    public Circle(double weight,String color, double radius) {
        super(color,weight);
        this.radius = radius;
    }

    public double getRadius() {
        return radius;
    }

    public void setRadius(double radius) {
        this.radius = radius;
    }
    
    @Override
    public double findArea() {
        return 3.14 * radius * radius;
    }
}
```

MyRectangle类

```java
public class MyRectangle extends GeometricObject {

    private double width;
    private double height;
    
    public MyRectangle(double width, double height,String color,double weight) {
        super(color, weight);
        this.height = height;
        this.width = width;
    }

    public double getWidth() {
        return width;
    }

    public void setWidth(double width) {
        this.width = width;
    }

    public double getHeight() {
        return height;
    }

    public void setHeight(double height) {
        this.height = height;
    }

    @Override
    public double findArea() {
        return width * height;
    }
}
```

GeometricTest类

```java
/*
 * 定义一个测试类GeometricTest，编写equalsArea方法测试两个对象的面积是否相等（注意方法的参数类型，利用动态绑定技术），
 * 编写displayGeometricObject方法显示对象的面积（注意方法的参数类型，利用动态绑定技术）。
 * 
 */
public class GeometricTest {
    
    public static void main(String[] args) {
        GeometricTest test = new GeometricTest();
        
        Circle c1 = new Circle(2.3,"white",1.0);
        test.displayGeometricObject(c1);
        
        Circle c2 = new Circle(3.3,"white",1.0);
        test.displayGeometricObject(c2);
        
        boolean isEqual = test.equalsArea(c1, c2);
        System.out.println("面积是否相等: " + isEqual);
        
        MyRectangle rect = new MyRectangle(2.1, 3.4,"red",1.0);
        test.displayGeometricObject(rect);
    }
    
    public void displayGeometricObject(GeometricObject o){
        System.out.println("面积为: " + o.findArea());
    }
    
    //测试两个对象的面积是否相等
    public boolean equalsArea(GeometricObject o1,GeometricObject o2){
        return o1.findArea() == o2.findArea();
    }
}
```

练习4

```java
/*
 * 面试题：多态是编译时行为还是运行时行为？如何证明？
 * 
 * 证明见如下：
 */
import java.util.Random;

class Animal  {

    protected void eat() {
        System.out.println("animal eat food");
    }
}

class Cat  extends Animal  {

    protected void eat() {
        System.out.println("cat eat fish");
    }
}

class Dog  extends Animal  {

    public void eat() {
        System.out.println("Dog eat bone");
    }
}

class Sheep  extends Animal  {

    public void eat() {
        System.out.println("Sheep eat grass");

    }

}

public class InterviewTest {

    public static Animal  getInstance(int key) {
        switch (key) {
        case 0:
            return new Cat ();
        case 1:
            return new Dog ();
        default:
            return new Sheep ();
        }

    }

    public static void main(String[] args) {
        int key = new Random().nextInt(3);

        System.out.println(key);

        Animal  animal = getInstance(key);
        
        animal.eat();
         
    }
}
```

> 4、面试题拓展

```java
/* 考查多态的笔试题目：
 * 面试题：多态是编译时行为还是运行时行为？如何证明？
 * 
 * 拓展问题
 */
public class InterviewTest1 {

    public static void main(String[] args) {
        Base base = new Sub();
        base.add(1, 2, 3);

//        Sub s = (Sub)base;
//        s.add(1,2,3);
    }
}

class Base {
    public void add(int a, int... arr) {
        System.out.println("base");
    }
}

class Sub extends Base {

    public void add(int a, int[] arr) {
        System.out.println("sub_1");
    }

//    public void add(int a, int b, int c) {
//        System.out.println("sub_2");
//    }

}
```

## 07、Object 类的使用

```java
/*
 * java.lang.Object类
 * 1.Object类是所有Java类的根父类;
 * 2.如果在类的声明中未使用extends关键字指明其父类，则默认父类为java.lang.Object类
 * 3.Object类中的功能(属性、方法)就具有通用性。
 * 属性:无
 * 方法:equals() / toString() / getClass() / hashCode() / clone() /finalize()
 *      wait() 、notify()、notifyAll()
 * 
 * 4.Object类只声明了一个空参的构造器。
 * 
 * 面试题:
 * final、finally、finalize的区别？
 * 
 */
public class ObjectTest {

    public static void main(String[] args) {
        
    }
}

class Order{
    
}
```

### 7.1、Object类中的主要结构

![null](https://i-blog.csdnimg.cn/blog_migrate/bc52c18e6524f904fa9b91dffaa3abab.png)

### 7.2、==操作符与equals方法

```java
import java.sql.Date;

/*
 * 面试题: ==和equals的区别
 * 
 * 一、回顾==的使用
 * == : 运算符
 * 1.可以使用在基本数据类型变量和引用数据类型变量中
 * 2.如果比较的是基本数据类型变量：比较两个变量保存的数据是否相等。(不一定类型要相同)
 *        如果比较的是引用数据类型变量：比较两个对象的地址值是否相同,即两个引用是否指向同一个对象实体
 *  补充: == 符号使用时，必须保证符号左右两边的变量类型一致。
 *
 * 二、equals()方法的使用
 * 1.是一个方法，而非运算符
 * 2.只能适用于引用数据类型。
 * 3.Object类中equals()的定义：
 *         public boolean equals(Object obj){
 *             return (this == obj);
 *         }
 * 说明：Object类中定义的equals()和==的作用是相同的，比较两个对象的地址值是否相同，即两个引用是否指向同一个对象实体。
 * 
 * 4.像String、Date、File、包装类等都重写了Object类中的equals()方法.
 *      两个引用的地址是否相同，而是比较两个对象的“实体内容”是否相同。
 * 
 * 5.通常情况下，我们自定义的类如果使用equals()的话，也通常是比较两个对象的"实体内容"是否相同。那么，我们
 *        就需要对Object类中的equals()进行重写。
 * 
 * 重写的原则:比较两个对象的实体内容是否相同。
 * 
 */
public class EqualsTest {
    public static void main(String[] args) {
        
        //基本数据类型
        int i = 10;
        int j = 10;
        double d = 10.0;
        System.out.println(i == j);    //true
        System.out.println(i == d); //true
        
//        boolean b =true;
//        System.out.println(i == b);
        
        char c = 10;
        System.out.println(i == c); //true
        
        char c1 = 'A';
        char c2 = 65;
        System.out.println(c1 == c2); //true
        
        //引用数据类型
        Customer cust1 = new Customer("Tom" ,21);
        Customer cust2 = new Customer("Tom" ,21);
        System.out.println(cust1 == cust2); //false
        
        String str1 = new String("BAT");
        String str2 = new String("BAT");
        System.out.println(str1 == str2); //false
        System.out.println("*************************");
        System.out.println(cust1.equals(cust2));    //false
        System.out.println(str1.equals(str2));    //true
        
        Date date1 = new Date(23432525324L);
        Date date2 = new Date(23432525324L);
        System.out.println(date1.equals(date2));    //true
    }
}
```

> Customer类

```java
public class Customer {
    
    private String name;
    private int age;
    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }
    public int getAge() {
        return age;
    }
    public void setAge(int age) {
        this.age = age;
    }
    public Customer() {
        super();
    }
    public Customer(String name, int age) {
        super();
        this.name = name;
        this.age = age;
    }


    //自动生成的equals()
    @Override
    public boolean equals(Object obj) {
        if (this == obj)
            return true;
        if (obj == null)
            return false;
        if (getClass() != obj.getClass())
            return false;
        Customer other = (Customer) obj;
        if (age != other.age)
            return false;
        if (name == null) {
            if (other.name != null)
                return false;
        } else if (!name.equals(other.name))
            return false;
        return true;
    }
    
    //重写原则，比较两个对象的实体内容(即name和age)是否相同
    //手动实现equals()的重写
//    @Override
//    public boolean equals(Object obj) {
//        
        System.out.println("Customer equals()....");
//        if(this == obj){
//            return true;
//        }
//        
//        if(obj instanceof Customer){
//            Customer cust = (Customer)obj;
//            //比较两个对象的属性是否都相同
            if(this.age == cust.age && this.name.equals(cust.name)){
                return true;
            }else{
                return false;
            }
//            
//            //或
//            return this.age == cust.age && this.name.equals(cust.name);
//        }
//        
//        return false;
//    }
        
}
```

#### 7.2.1、重写equals()方法的原则

•对称性：如果x.equals(y)返回是“true”，那么y.equals(x)也应该返回是“true”。•自反性：x.equals(x)必须返回是“true”。•传递性：如果x.equals(y)返回是“true”，而且y.equals(z)返回是“true”，那么z.equals(x)也应该返回是“true”。•一致性：如果x.equals(y)返回是“true”，只要x和y内容一直不变，不管你重复x.equals(y)多少次，返回都是“true”。•任何情况下，x.equals(null)，永远返回是“false”；x.equals(和x不同类型的对象)永远返回是“false”。

```java
    int it = 65;
    float fl= 65.0f;
    System.out.println("65和65.0f是否相等？" + (it == fl)); //true
    char ch1 = 'A'; 
    char ch2 = 12;
    System.out.println("65和'A'是否相等？" + (it == ch1));//true
    System.out.println("12和ch2是否相等？" + (12 == ch2));//true 
    String str1 = new String("hello");
    String str2 = new String("hello");
    System.out.println("str1和str2是否相等？"+ (str1 == str2));//false
    System.out.println("str1是否equals str2？"+(str1.equals(str2)));//true
    System.out.println("hello" == new java.util.Date()); //编译不通过
```

> 练习一

```java
/*
 * .编写Order类，有int型的orderId，String型的orderName，
 * 相应的getter()和setter()方法，两个参数的构造器，重写父类的equals()方法：public booleanequals(Object obj)，
 * 并判断测试类中创建的两个对象是否相等。
 * 
 * 
 */
public class OrderTest {
    public static void main(String[] args) {
        Order order1 = new Order(1001,"AA");
        Order order2 = new Order(1001,"BB");
        
        System.out.println(order1.equals(order2));    //false
        
        Order order3 = new Order(1001,"BB");
        System.out.println(order2.equals(order3)); //true
    }
}

class Order{
    private int orderId;
    private String orderName;
    public int getOrderId() {
        return orderId;
    }
    public void setOrderId(int orderId) {
        this.orderId = orderId;
    }
    public String getOrderName() {
        return orderName;
    }
    public void setOrderName(String orderName) {
        this.orderName = orderName;
    }
    public Order(int orderId, String orderName) {
        super();
        this.orderId = orderId;
        this.orderName = orderName;
    }
    public boolean equals(Object obj){
        if(this == obj){            
            return true;
        }
        if(obj instanceof Order){
            Order order = (Order)obj;
            //正确的
            return this.orderId == order.orderId && this.orderName.equals(order.orderName);
            //错误的
//            return this.orderId == order.orderId && this.orderName == order.orderName;
        }
        return false;
    }
}
```

> 练习二

```java
/*
 * 请根据以下代码自行定义能满足需要的MyDate类,在MyDate类中覆盖equals方法，
 * 使其判断当两个MyDate类型对象的年月日都相同时，结果为true，否则为false。
 * public boolean equals(Object o)
 */
public class MyDateTest {
    public static void main(String[] args) {
        MyDate m1= new MyDate(14, 3, 1976);
        MyDate m2= new MyDate(14, 3, 1976);
        if(m1== m2) {
            System.out.println("m1==m2");
        } else{
            System.out.println("m1!=m2"); // m1 != m2
        }
        
        if(m1.equals(m2)) {
            System.out.println("m1 is equal to m2");// m1 is equal to m2
        } else{
            System.out.println("m1 is not equal to m2");
        }
    }
}

class MyDate{
    private int day;
    private int month;
    private int year;
    
    public MyDate(int day, int month, int year) {
        super();
        this.day = day;
        this.month = month;
        this.year = year;
    }

    public int getDay() {
        return day;
    }

    public void setDay(int day) {
        this.day = day;
    }

    public int getMonth() {
        return month;
    }


    public void setMonth(int month) {
        this.month = month;
    }

    public int getYear() {
        return year;
    }

    public void setYear(int year) {
        this.year = year;
    }
    
    @Override
    public boolean equals(Object obj) {
        if(this == obj){
            return true;
        }
        if(obj instanceof MyDate){
            MyDate myDate = (MyDate)obj;
            return this.day == myDate.day && this.month == myDate.month &&
                    this.year == myDate.year;
        }
        return false;
    }

//    @Override
//    public boolean equals(Object obj) {
//        if (this == obj)
//            return true;
//        if (obj == null)
//            return false;
//        if (getClass() != obj.getClass())
//            return false;
//        MyDate other = (MyDate) obj;
//        if (day != other.day)
//            return false;
//        if (month != other.month)
//            return false;
//        if (year != other.year)
//            return false;
//        return true;
//    }
        
}
```

### 7.3、toString的使用

```java
public class Customer {
    
    private String name;
    private int age;
    public String getName() {
        return name;
    }
    public void setName(String name) {
        this.name = name;
    }
    public int getAge() {
        return age;
    }
    public void setAge(int age) {
        this.age = age;
    }
    public Customer() {
        super();
    }
    public Customer(String name, int age) {
        super();
        this.name = name;
        this.age = age;
    }

    //自动生成的equals()
    @Override
    public boolean equals(Object obj) {
        if (this == obj)
            return true;
        if (obj == null)
            return false;
        if (getClass() != obj.getClass())
            return false;
        Customer other = (Customer) obj;
        if (age != other.age)
            return false;
        if (name == null) {
            if (other.name != null)
                return false;
        } else if (!name.equals(other.name))
            return false;
        return true;
    }
    
    //重写原则，比较两个对象的实体内容(即name和age)是否相同
    //手动实现equals()的重写
//    @Override
//    public boolean equals(Object obj) {
//        
        System.out.println("Customer equals()....");
//        if(this == obj){
//            return true;
//        }
//        
//        if(obj instanceof Customer){
//            Customer cust = (Customer)obj;
//            //比较两个对象的属性是否都相同
            if(this.age == cust.age && this.name.equals(cust.name)){
                return true;
            }else{
                return false;
            }
//            
//            //或
//            return this.age == cust.age && this.name.equals(cust.name);
//        }
//        
//        return false;
//    }
    
    //手动实现
//    @Override
//    public String toString() {
//        return "Customer[name = " + name + ",age = " + age + "]";
//    }
    
    //自动实现
    @Override
    public String toString() {
        return "Customer [name=" + name + ", age=" + age + "]";
    }

}
```

> ToStringTest类

```java
import java.util.Date;
/*
 * Object类中toString()的使用
 * 
 * 1.当我们输出一个引用对象时，实际上就是调用当前对象的toString()
 * 2.Object类中toString的定义方法
 *     public String toString() {
 *      return getClass().getName() + "@" + Integer.toHexString(hashCode());
 *  }
 * 
 * 3.像String、Date、File、包装类等都重写了Object类中的toString()方法。
 *      使得在调用toString()时，返回"实体内容"信息.
 * 
 * 4.自定义类如果重写toString()方法，当调用此方法时，返回对象的"实体内容".
 */
public class ToStringTest {
    public static void main(String[] args) {
        
        Customer cust1 = new Customer("Tom" ,21);
        System.out.println(cust1.toString());    //github4.Customer@15db9742
        System.out.println(cust1);     //github4.Customer@15db9742 ---> Customer[name = Tom,age = 21]
        
        String str = new String("MM");
        System.out.println(str);
        
        Date date = new Date(45362348664663L);
        System.out.println(date.toString());    //Wed Jun 24 12:24:24 CST 3407
        
    }
}
```

> 练习

GeometricObject类

```java
public class GeometricObject {
    protected  String  color;
    protected  double  weight;
    
    public GeometricObject() {
        super();
        this.color = "white";
        this.weight = 1.0;
    }
    
    public GeometricObject(String color, double weight) {
        super();
        this.color = color;
        this.weight = weight;
    }

    public String getColor() {
        return color;
    }

    public void setColor(String color) {
        this.color = color;
    }

    public double getWeight() {
        return weight;
    }

    public void setWeight(double weight) {
        this.weight = weight;
    }
}
```

> Circle类

```java
public class Circle extends GeometricObject{
    private double radius;

    public Circle() {    //初始化对象的color属性为“white”，weight属性为1.0，radius属性为1.0。
        super();    //super自带，不需再写
//        this.color = "white";
//        this.weight = 1.0;
        this.radius = 1.0;
    }

    //初始化对象的color属性为“white”，weight属性为1.0，radius根据参数构造器确定。
    public Circle(double radius) {    
        super();    //super自带，不需再写
//        this.color = "white";
//        this.weight = 1.0;
        this.radius = radius;
    }

    public Circle(double radius,String color,double weight) {
        super(color,weight);
        this.radius = radius;
    }
    
    public double getRadius() {
        return radius;
    }

    public void setRadius(double radius) {
        this.radius = radius;
    }

    //计算圆的面积
    public double findArea(){
        return Math.PI * radius * radius;
    }
    
    @Override    //重写equals方法,比较两个圆的半径是否相等，如相等，返回true。
    public boolean equals(Object obj) {
        if(this == obj){
            return true;
        }
        
        if(obj instanceof Circle){
            Circle c = (Circle)obj;
            return this.radius == c.radius;
        }
        
        return false;
    }

    @Override
    public String toString() {    //重写toString方法,输出圆的半径。
        return "Circle [radius=" + radius + "]";
    }
    
}
```

> 测试类

```java
/*
 * 写一个测试类，创建两个Circle对象，判断其颜色是否相等；
 * 利用equals方法判断其半径是否相等；利用toString()方法输出其半径。
 * 
 */
public class CircleTest {
    public static void main(String[] args) {
        
        Circle circle1 = new Circle(2.3);
        Circle circle2 = new Circle(3.3,"white",2.0);
        
        System.out.println("颜色是否相等: " + circle1.getColor().equals(circle2.color));
        
        System.out.println("半径是否相等: " + circle1.equals(circle2));
        
        System.out.println(circle1);
        System.out.println(circle2.toString());
    }
}
```

## 08、包装类(Wrapper)的使用

### 8.1、单元测试方法的使用

```java
import java.util.Date;
import org.junit.Test;
/*
 * java中的JUnit单元测试
 * 
 * 步骤:
 * 1.选中当前项目工程 --》 右键:build path --》 add libraries --》 JUnit 4 --》 下一步
 * 2.创建一个Java类进行单元测试。
 *      此时的Java类要求:①此类是公共的 ②此类提供一个公共的无参构造器 
 * 3.此类中声明单元测试方法。
 *   此时的单元测试方法:方法的权限是public,没有返回值，没有形参。
 * 
 * 4.此单元测试方法上需要声明注解:@Test并在单元测试类中调用:import org.junit.Test;
 * 5.声明好单元测试方法以后，就可以在方法体内测试代码。
 * 6.写好代码后，左键双击单元测试方法名：右键 --》 run as --》 JUnit Test
 * 
 * 说明:如果执行结果无错误，则显示是一个绿色进度条，反之，错误即为红色进度条。
 */
public class JUnit {
    
    int num = 10;
    
    //第一个单元测试方法
    @Test
    public void testEquals(){
        String s1 = "MM";
        String s2 = "MM";
        System.out.println(s1.equals(s2));
        
        //ClassCastException的异常
//        Object obj = new String("GG");
//        Date date = (Date)obj;
        
        System.out.println(num);
        show();
    }
    
    public void show(){
        num = 20;
        System.out.println("show()...");
    }
    
    //第二个单元测试方法
    @Test
    public void testToString(){
        String s2 = "MM";
        System.out.println(s2.toString());
    }
}
```

![null](https://i-blog.csdnimg.cn/blog_migrate/fd60c5a3bde94d06db75b72c03d98a17.png)



![null](https://i-blog.csdnimg.cn/blog_migrate/6c78285395bce734ee6f61a4059a9dc2.png)



![null](https://i-blog.csdnimg.cn/blog_migrate/b36b4eb121e1c851b31530f2720f3aff.png)

### 8.2、包装类的使用

```java
/*
 * 包装类的使用
 * 1.java提供了8种基本数据类型对应的包装类，使得基本数据类型的变量具有类的特征
 *         基本数据类型        包装类
 *         byte            Byte
 *         short            Short
 *         int             Integer
 *         long            Long
 *         float            Float
 *         double            Double
 *         boolean            Boolean
 *         char            Character
 * 注意:其中Byte、Short、Integer、Long、Float、Double的父类是:Number
 * /
```

### 8.3、包装类与基本数据类型相互转换

![null](https://i-blog.csdnimg.cn/blog_migrate/880a51c76b4520cae1b4fcfb44871830.png)

```java
import org.junit.Test;
/*
 * 2.基本数据类型、包装类、String三者之间的相互转换。
 * 
 */
public class WrapperTest {
    
    //String类型---> 基本数据类型、包装类,调用包装类的parseXxx()
    @Test
    public void test5(){
        String str1 = "123";
//        String str1 = "123a";
        
        //错误的情况，可能会报错
//        int num1 = (int)str1;
//        Integer in1 = (Integer)str1;
        
        int num2 = Integer.parseInt(str1); 
        System.out.println(num2 + 1);    //124
        
        String str2 = "true";
        Boolean b1 = Boolean.parseBoolean(str2);
        System.out.println(b1);    //true
        
    }
    
    //基本数据类型、包装类---》String类型，调用String重载的valueOf(Xxx xxx)
    @Test
    public void test4(){
        int num1 = 10;
        //方式1:连接运算
        String str1 = num1 + "";
        //方式2:调用String的valueOf(Xxx xxx)
        float f1 = 12.3f;
        String str2 = String.valueOf(f1); //"12.3"
        
        Double d1 = new Double(12.4);
        String str3 = String.valueOf(d1);
        System.out.println(str2);
        System.out.println(str3);    //"12.4"
        
    }
    
    /*
     * JDK 5.0 新特性:自动装箱与自动拆箱
     */
    @Test
    public void test3(){
//        int num1 = 10;
//        //基本数据类型 --》 包装类的对象
//        method(num1);    //Object obj = num1
        
        //自动装箱:基本数据类型 --》 包装类
        int num2 = 10;
        Integer in1 = num2;//自动装箱
        
        boolean b1 = true;
        Boolean b2 = b1;//自动装箱
        
        //自动拆箱：包装类 --》 基本数据类型
        System.out.println(in1.toString());
        
        int num3 = in1;
        
    }
    
    public void method(Object obj){
        System.out.println(obj);
    }
    
    //包装类 --》 基本数据类型:调用包装类的xxxValue()
    @Test
    public void test2() {
        Integer in1 = new Integer(12);
        int i1 = in1.intValue();
        System.out.println(i1 + 1); 
        
        Float f1 = new Float(12.3f);
        float f2 = f1.floatValue();
        System.out.println(f2 + 1); 
    }
    
    //基本数据类型--》包装类,调用包装类的构造器
    @Test
    public void test1() {
        int num1 = 10;
//        System.out.println(num1.toString());
        
        Integer in1 = new Integer(num1);
        System.out.println(in1.toString());
        
        Integer in2 = new Integer("123");
        System.out.println(in2.toString());
        
        //报异常
//        Integer in3 = new Integer("123abc");
//        System.out.println(in3.toString());
        
        Float f1 = new Float(12.3f);
        Float f2 = new Float("12.3");
        System.out.println(f1);
        System.out.println(f2);
        
        Boolean b1 = new Boolean(true);
        Boolean b2 = new Boolean("true");
        
        Boolean b3 = new Boolean("true123");
        System.out.println(b3); //false
        
        Order order = new Order();
        System.out.println(order.isMale); //false
        System.out.println(order.isFemale); //null
        
    }
}

class Order{
    
    boolean isMale;
    Boolean isFemale;
}
```

### 8.4、练习

> 1、面试题

```java
import org.junit.Test;
/*
 * 如下两个题目输出结果相同吗？各是什么：
 *         Object o1= true? new Integer(1) : new Double(2.0);
 *         System.out.println(o1);//
 * 
 *         Object o2;
 *         if(true)
 *             o2 = new Integer(1);
 *        else 
 *            o2 = new Double(2.0);
 *        System.out.println(o2);//
 *
 */
public class InterViewTest {

    @Test
    public void test(){
        Object o1= true? new Integer(1) : new Double(2.0);
        System.out.println(o1);// 1.0
    }
    
    @Test
    public void test2(){
        Object o2;
        if(true)
            o2 = new Integer(1);
        else 
            o2 = new Double(2.0);
        System.out.println(o2);// 1
    }
    
    @Test
    public void method1() {
        Integer i = new Integer(1);
        Integer j = new Integer(1);
        System.out.println(i == j); //false
        
        //Integer内部定义了一个IntegerCache结构，IntegerCache中定义Integer[]
        //保存了从-128-127范围的整数。如果我们使用自动装箱的方式，给Integer赋值的范围在其中时，
        //可以直接使用数组中的元素，不用再去new了。目的，提高效率。
        
        Integer m = 1;
        Integer n = 1;
        System.out.println(m == n);//true
        
        Integer x = 128;//相当于new了一个Integer对象
        Integer y = 128;//相当于new了一个Integer对象
        System.out.println(x == y);//false

    }
}
```

> 2、编程题

![null](https://i-blog.csdnimg.cn/blog_migrate/e141433abe3ddbd4245adb769d733fee.png)

```java
import java.util.Scanner;
import java.util.Vector;

/*
 * 利用Vector代替数组处理：从键盘读入学生成绩（以负数代表输入结束），
 * 找出最高分，并输出学生成绩等级。
 * 
 * 提示：数组一旦创建，长度就固定不变，所以在创建数组前就需要知道它的长度。
 * 而向量类java.util.Vector可以根据需要动态伸缩。
 * 
 * 创建Vector对象：Vector v=new Vector();
 * 给向量添加元素：v.addElement(Object obj);   //obj必须是对象
 * 取出向量中的元素：Object  obj=v.elementAt(0);
 * 注意第一个元素的下标是0，返回值是Object类型的。
 * 计算向量的长度：v.size();
 * 若与最高分相差
 *         10分内：A等；
 *         20分内：B等；
 *         30分内：C等；
 *         其它：D等
 * 
 */
public class VectorTest {
    public static void main(String[] args) {
        // 1.实例化Scanner，用于从键盘获取学生成绩
        Scanner scan = new Scanner(System.in);

        // 2.创建Vector对象：Vector v=new Vector();相当于原来的数组
        Vector v = new Vector();

        // 3.通过for(;;)或while(true)方式，给Vector中添加数组
        int maxScore = 0;
        for (;;) {
            System.out.println("请输入学生成绩（以负数代表输入结束）");
            int score = scan.nextInt();
            // 3.2 当输入是负数时，跳出循环
            if (score < 0) {
                break;
            }
            if (score > 100) {
                System.out.println("输入的数据非法，请重新输入");
                continue;
            }
            // 3.1 添加操作：：v.addElement(Object obj)
            // jdk5.0之前：
            // Integer inScore = new Integer(score);
            // v.addElement(inScore);//多态
            // jdk5.0之后：
            v.addElement(score);// 自动装箱
            // 4.获取学生成绩的最大值
            if (maxScore < score) {
                maxScore = score;
            }
        }

        // 5.遍历Vector，得到每个学生的成绩，并与最大成绩比较，得到每个学生的等级。
        char level;
        for (int i = 0; i < v.size(); i++) {
            Object obj = v.elementAt(i);
            // jdk 5.0之前：
            // Integer inScore = (Integer)obj;
            // int score = inScore.intValue();
            // jdk 5.0之后：
            int score = (int) obj;

            if (maxScore - score <= 10) {
                level = 'A';
            } else if (maxScore - score <= 20) {
                level = 'B';
            } else if (maxScore - score <= 30) {
                level = 'C';
            } else {
                level = 'D';
            }

            System.out.println("student-" + i + " score is " + score + ",level is " + level);

        }
    }
}
```

## 八：面向对象（下）

#### 文章目录

•01、关键字：static••1.1、static 的使用•1.2、类变量 vs 实例变量内存解析•1.3、static 修饰方法•1.4、自定义 ArrayUtil 的优化•1.5、static 的应用举例•1.6、static 的练习•1.7、单例(Singleton)设计模式•02、理解 main 方法的语法（了解)•03、类的成员之四：代码块•04、关键字：final•05、抽象类与抽象方法••5.1、抽象类应用•5.2、练习•5.3、创建抽象类的匿名子类对象•5.4、多态的应用：模板方法设计模式(TemplateMethod)•5.5、抽象类的练习•06、接口(interface)••6.1、概述•6.2、举例•6.3、接口的应用：代理模式(Proxy)•6.4、接口的应用：工厂模式•07、Java 8 中关于接口的改进•08、类的内部成员之五：内部类••8.1、匿名内部类•8.2、局部内部类的使用注意•其他

## 01、关键字：static

### 1.1、static 的使用

当我们编写一个类时，其实就是在描述其对象的属性和行为，而并没有产生实质上的对象，只有通过 new 关键字才会产生出对象，这时系统才会分配内存空间给对象，其方法才可以供外部调用。

我们有时候希望无论是否产生了对象或无论产生了多少对象的情况下，**某些特定的数据在内存空间里只有一份。**

例如所有的中国人都有个国家名称，每一个中国人都共享这个国家名称，不必在每一个中国人的实例对象中都单独分配一个用于代表国家名称的变量。

![null](https://i-blog.csdnimg.cn/blog_migrate/91ada234013c6114c5ca555b6b8c0fad.png)

```java
/*
 * static 关键字的使用
 * 
 * 1.static:静态的。
 * 2.static 可以用来修饰:属性、方法、代码块、内部类。
 * 
 * 3.使用 static 修饰属性:静态变量(或类变量)。
 *         3.1  属性:是否使用 static 修饰，又分为:静态属性 VS 非静态属性(实例变量)
 *            实例变量:我们创建了类的多个对象，每个对象都独立的拥有了一套类中的非静态属性。
 *                 当修改其中一个非静态属性时，不会导致其他对象中同样的属性值的修饰。
 *            静态变量:我们创建了类的多个对象，多个对象共享同一个静态变量。当通过静态变量去修改某一个变量时，
 *                 会导致其他对象调用此静态变量时，是修改过的。
 *         3.2 static 修饰属性的其他说明:
 *             ① 静态变量随着类的加载而加载。可以通过"类.静态变量"的方式进行调用。
 *             ② 静态变量的加载要早于对象的创建。
 *             ③ 由于类只会加载一次，则静态变量在内存中也只会存在一次。存在方法区的静态域中。
 * 
 *             ④         类变量        实例变量
 *             类        yes            no
 *             对象        yes            yes
 * 
 *         3.3 静态属性举例:System.out.Math.PI;
 *  
 */
public class StaticTest {
    public static void main(String[] args) {
        
        Chinese.nation = "中国";
        
        Chinese c1 = new Chinese();
        c1.name = "姚明";
        c1.age = 40;
        c1.nation = "CHN";
        
        Chinese c2 = new Chinese();
        c2.name = "马龙";
        c2.age = 30;
        c2.nation = "CHINA";
        
        System.out.println(c1.nation); 
        
        //编译不通过
//        Chinese.name = "张继科";
        
    }
}
//中国人
class Chinese{
    
    String name;
    int age;
    static String nation;
}
```

### 1.2、类变量 vs 实例变量内存解析

![null](https://i-blog.csdnimg.cn/blog_migrate/6a210c103f942bc13d287e2d6044ce25.png)

### 1.3、static 修饰方法

```java
/* 
 * 4.使用 static 修饰方法:静态方法
 *         ① 随着类的加载而加载，可以通过"类.静态方法"的方式调用
 *         ②             静态方法        非静态方法
 *             类        yes            no
 *             对象        yes            yes
 *         ③ 静态方法中，只能调用静态的方法或属性
 *           非静态的方法中，可以调用所有的方法或属性
 * 
 * 5.static 注意点:
 *      5.1  在静态的方法内，不能使用 this 关键字、super 关键字
 *   5.2 关于静态属性和静态方法的使用，大家从生命周期的角度去理解。
 *   
 * 6.开发中，如何确定一个属性是否需要声明 static 的？
 *      》 属性是可以被多个对象所共享的，不会随着对象的不同而不同的。
 *      》 类中的常量也常常声明为 static
 *   
 *   开发中，如何确定一个方法是否要声明为 static 的？
 *   》 操作静态属性的方法，通常设置为 static 的
 *   》 工具类中的方法，习惯上声明为 static 的。比如：Math、Arrays、Collections
 *      
 */
public class StaticTest {
    public static void main(String[] args) {
        
        Chinese.nation = "中国";
        
        Chinese c1 = new Chinese();
        
        //编译不通过
//        Chinese.name = "张继科";
        
        c1.eat();
        
        Chinese.show();
        //编译不通过
//        chinese.eat();
//        Chinese.info();
    }
}
//中国人
class Chinese{
    
    String name;
    int age;
    static String nation;
    
    public void eat(){
        System.out.println("中国人吃中餐");
        //调用非静态结构
        this.info();
        System.out.println("name : " + name);
        //调用静态结构
        walk();
        System.out.println("nation : " + Chinese.nation);
    }
    
    public static void show(){
        System.out.println("我是一个中国人！");
//        eat();
//        name = "Tom";
        //可以调用静态的结构
        System.out.println(Chinese.nation);
        walk();
    }
    
    public void info(){
        System.out.println("name : " + name + ",age : " + age);
    }
    
    public static void walk(){
        
    }
}
```

### 1.4、自定义 ArrayUtil 的优化

```java
/*
 * 自定义数组工具类
 */
public class ArrayUtil {

    // 求数组的最大值
    public static int getMax(int[] arr) {
        int maxValue = arr[0];
        for (int i = 1; i < arr.length; i++) {
            if (maxValue < arr[i]) {
                maxValue = arr[i];
            }
        }
        return maxValue;
    }

    // 求数组的最小值
    public static int getMin(int[] arr) {
        int minValue = arr[0];
        for (int i = 1; i < arr.length; i++) {
            if (minValue > arr[i]) {
                minValue = arr[i];
            }
        }
        return minValue;
    }

    // 求数组总和
    public static int getSum(int[] arr) {
        int sum = 0;
        for (int i = 0; i < arr.length; i++) {
            sum += arr[i];
        }
        return sum;
    }

    // 求数组平均值
    public static int getAvg(int[] arr) {
        int avgValue = getSum(arr) / arr.length;
        return avgValue;
    }

    //如下两个同名方法构成重载
    // 反转数组
    public static void reverse(int[] arr) {
        for (int i = 0; i < arr.length / 2; i++) {
            int temp = arr[i];
            arr[i] = arr[arr.length - i - 1];
            arr[arr.length - i - 1] = temp;
        }
    }
    
    public void reverse(String[] arr){
        
    }

    // 复制数组
    public static int[] copy(int[] arr) {
        int[] arr1 = new int[arr.length];
        for (int i = 0; i < arr1.length; i++) {
            arr1[i] = arr[i];
        }
        return null;
    }

    // 数组排序
    public static void sort(int[] arr) {
        for (int i = 0; i < arr.length - 1; i++) {
            for (int j = 0; j < arr.length - 1 - i; j++) {
                if (arr[j] > arr[j + 1]) {
//                    int temp = arr[j];
//                    arr[j] = arr[j + 1];
//                    arr[j + 1] = temp;
                    //错误的：
//                    swap(arr[j],arr[j+1]);
                    
                    swap(arr,j ,j+1);
                }
            }
        }
    }
    
    //错误的:交换数组中两个指定位置元素的值
//    public void swap(int i,int j){
//        int temp = i;
//        i = j;
//        j = temp;
//    }
    
    //正确的：
    private static void swap(int[] arr,int i,int j){
        int temp = arr[i];
        arr[i] = arr[j];
        arr[j] = temp;
    }

    // 遍历数组
    public static void print(int[] arr) {
        System.out.print("[");
        for (int i = 0; i < arr.length; i++) {
            System.out.print(arr[i] + ",");
        }
        System.out.println("]");
    }

    // 查找指定元素
    public static int getIndex(int[] arr, int dest) {
        //线性查找
        for (int i = 0; i < arr.length; i++) {

            if (dest==arr[i]) {
                return i;
            }

        }
        return -1;
    }

}
```

> 测试类

```java
public class ArrayUtilTest {

    public static void main(String[] args) {
//        ArrayUtil util = new ArrayUtil();
        int[] arr = new int[]{32,5,26,74,0,96,14,-98,25};
        int max = ArrayUtil.getMax(arr);
        System.out.println("最大值为:" + max);
        
        System.out.print("排序前:");
        ArrayUtil.print(arr);
        
        ArrayUtil.sort(arr);
        System.out.print("排序后:");
        ArrayUtil.print(arr);
        
//        System.out.println("查找:");
//        int index = util.getIndex(arr, 5);
//        if(index > 0){
//            System.out.println("找到了，索引地址:" + index);
//        }else{
//            System.out.println("没找到");
//        }
    }
}
```

### 1.5、static 的应用举例

```java
//static 关键字的应用
public class CircleTest {
    public static void main(String[] args) {
        
        Circle c1 = new Circle();
        
        Circle c2 = new Circle();
        
        Circle c3 = new Circle();
        
        System.out.println("c1 的 ID:" + c1.getId());
        System.out.println("c2 的 ID:" + c2.getId());
        System.out.println("c3 的 ID:" + c3.getId());
        
        System.out.println("创建圆的个数: " + Circle.getTotal());
        
    }
    
}

class Circle{
    
    private double radius;
    private int id;    //需要自动赋值
    
    public Circle(){
        id = init++;
        total++;
    }
    
    public Circle(double radius){
        this();
        //或
//        id = init++;
//        total++;
        this.radius = radius;
    }
    
    private static int total;//记录创建圆的个数
    private static int init = 1001;//static 声明的属性被所有对象所共享
    
    public double findArea(){
        return 3.14 * radius * radius;
    }

    public double getRadius() {
        return radius;
    }

    public void setRadius(double radius) {
        this.radius = radius;
    }

    public int getId() {
        return id;
    }

    public static int getTotal() {
        return total;
    }
    
}
```

### 1.6、static 的练习

```java
/*
 * 编写一个类实现银行账户的概念，包含的属性有“帐号”、“密码”、“存款余额”、
 * “利率”、“最小余额”，定义封装这些属性的方法。
 * 账号要自动生成。编写主类，使用银行账户类，输入、输出 3 个储户的上述信息。
 * 考虑：哪些属性可以设计成 static 属性。
 * 
 */
public class Account {
    
    private int id;    //账号
    private String pwd = "000000";    //密码
    private double balance; //存款余额
    
    private static double interestRate; //利率
    private static double minMoney = 1.0;  //最小余额
    private static int init = 1001;    //用于自动生成 id
    
    public Account(){    //账号自动生成
        id = init++;
    }
    
    public Account(String pwd,double balance){
        id = init++;
        this.pwd = pwd;
        this.balance = balance;
    }
    
    public String getPwd() {
        return pwd;
    }
    
    public void setPwd(String pwd) {
        this.pwd = pwd;
    }
    
    public static double getInterestRate() {
        return interestRate;
    }
    
    public static void setInterestRate(double interestRate) {
        Account.interestRate = interestRate;
    }
    
    public static double getMinMoney() {
        return minMoney;
    }
    
    public static void setMinMoney(double minMoney) {
        Account.minMoney = minMoney;
    }
    
    public int getId() {
        return id;
    }
    
    public double getBalance() {
        return balance;
    }

    @Override
    public String toString() {
        return "Account [id=" + id + ", pwd=" + pwd + ", balance=" + balance + "]";
    }
    
}
```

> **测试类**

```java
public class AccountTest {
    public static void main(String[] args) {
        
        Account acct1 = new Account();
        Account acct2 = new Account("qwerty",2000);
        
        Account.setInterestRate(0.012); 
        Account.setMinMoney(100);
        
        System.out.println(acct1);
        System.out.println(acct2);
        
        System.out.println(acct1.getInterestRate()); 
        System.out.println(acct1.getMinMoney());
    }
}
```

### 1.7、单例(Singleton)设计模式

设计模式是**在大量的实践中总结和理论化之后优选的代码结构、编程风格、以及解决问题的思考方式。**设计模免去我们自己再思考和摸索。就像是经典的棋谱，不同的棋局，我们用不同的棋谱。”套路”

所谓类的单例设计模式，就是采取一定的方法保证在整个的软件系统中，对**某个类只能存在一个对象实例**。并且该类只提供一个取得其对象实例的方法。如果我们要让类在一个虚拟机中只能产生一个对象，我们首先必须将类的**构造器的访问权限设置为 private**，这样，就不能用 new 操作符在类的外部产生类的对象了，但在类内部仍可以产生该类的对象。因为在类的外部开始还无法得到类的对象，**只能调用该类的某个静态方法以返回类内部创建的对象，静态方法只能访问类中的静态成员变量，所以，指向类内部产生的该类对象的变量也必须定义成静态的。**

> 1、**单例模式的饿汉式**

```java
/*
 * 单例设计模式:
 * 1.所谓类的单例设计模式，就是采取一定的方法保证在整个的软件系统中，对某个类只能存在一个对象实例
 *  
 * 2.如何实现？
 *   饿汉式    VS    懒汉式
 * 
 * 3.区分饿汉式和懒汉式。
 *        饿汉式：坏处:对象加载时间过长。
 *                 好处:饿汉式是线程安全的。
 * 
 *   懒汉式：好处:延迟对象的创建。
 *                坏处:目前的写法，会线程不安全。---》到多线程内容时，再修改
 */
public class SingletonTest {
    public static void main(String[] args) {
//        Bank bank1 = new Bank(); 
//        Bank bank2 = new Bank(); 
        
        Bank bank1 = Bank.getInstance();
        Bank bank2 = Bank.getInstance();
        
        System.out.println(bank1 == bank2);
        
    }
}

//单例的饿汉式
class Bank{
    
    //1.私有化类的构造器
    private Bank(){
        
    }
    
    //2.内部创见类的对象
    //4.要求此对象也必须声明为静态的
    private static Bank instance = new Bank();
    
    //3.提供公共的静态的方法，返回类的对象。
    public static Bank getInstance(){
        return instance;
    }
}
```

> 2、**单例模式的懒汉式**

```java
/*
 * 单例的懒汉式实现
 * 
 */
public class SingletonTest2 {
    public static void main(String[] args) {
        
        Order order1 = Order.getInstance();
        Order order2 = Order.getInstance();
        
        System.out.println(order1 == order2);
    }
}
class Order{
    //1.私有化类的构造器
    private Order(){
        
    }
    
    //2.声明当前类对象，没有初始化。
    //此对象也必须声明为 static 的
    private static Order instance = null;
    
    //3.声明 public、static 的返回当前类对象的方法
    public static Order getInstance(){
        if(instance == null){
            instance = new Order();            
        }
        return instance;
    }
}
```

> 3、**单例模式的优点**

由于单例模式只生成一个实例，**减少了系统性能开销**，当一个对象的产生需要比较多的资源时，如读取配置、产生其他依赖对象时，则可以通过在应用启动时直接产生一个单例对象，然后永久驻留内存的方式来解决。

![null](https://i-blog.csdnimg.cn/blog_migrate/66b80341eeac0ee7b29a73cd41a8090b.png)

> 4、单例(Singleton)设计模式-应用场景

•**网站的计数器**，一般也是单例模式实现，否则难以同步。•**应用程序的日志应用**，一般都使用单例模式实现，这一般是由于共享的日志文件一直处于打开状态，因为只能有一个实例去操作，否则内容不好追加。•**数据库连接池**的设计一般也是采用单例模式，因为数据库连接是一种数据库资源。•项目中，**读取配置文件的类**，一般也只有一个对象。没有必要每次使用配置文件数据，都生成一个对象去读取。•**Application**也是单例的典型应用•Windows 的 **Task Manager (任务管理器)**就是很典型的单例模式•Windows 的 **Recycle Bin(回收站)**也是典型的单例应用。在整个系统运行过程中，回收站一直维护着仅有的一个实例。

## 02、理解 main 方法的语法（了解)

由于 Java 虚拟机需要调用类的 main()方法，所以该方法的访问权限必须是 public，又因为 Java 虚拟机在执行 main()方法时不必创建对象，所以该方法必须是 static 的，该方法接收一个 String 类型的数组参数，该数组中保存执行 Java 命令时传递给所运行的类的参数。

又因为 main() 方法是静态的，我们不能直接访问该类中的非静态成员，必须创建该类的一个实例对象后，才能通过这个对象去访问类中的非静态成员，这种情况，我们在之前的例子中多次碰到。

```java
/*
 * main()方法的使用说明
 * 1.main()方法作为程序的入口;
 * 2.main()方法也是一个普通的静态方法
 * 3.main()方法也可以作为我们与控制台交互的方式。(之前，使用 Scanner)
 * 
 * 
 */
public class MainTest {
    public static void main(String[] args) {    //入口
        
        Main.main(new String[100]);
        
        MainTest test = new MainTest();
        test.show();
    }
    
    public void show(){
        
    }
}

class Main{
    public static void main(String[] args) {
        args = new String[100];
        for(int i = 0;i < args.length;i++){
            args[i] = "args_" + i;
            System.out.println(args[i]);
        }
    }
}
```

> **命令行参数用法举例**

```java
public class MainDemo {
    public static void main(String[] args) {
        
        for(int i = 0;i < args.length;i++){
            System.out.println("/*/*/*/"+ args[i]);
        }    
    }
}
```

> //运行程序 MainDemo.java

```java
javac MainDemo.java
java MainDemo “Tom” “Jerry” “Shkstart”
```

![null](https://i-blog.csdnimg.cn/blog_migrate/ad7f9d782b9b47f76c32455e48f3e653.png)

## 03、类的成员之四：代码块

```java
/*
 * 类的成员之四:代码块（或初始化块）
 * 
 * 1.代码块的作用：用来初始化类、对象的
 * 2.代码块如果有修饰的话，只能使用 static
 * 3.分类:静态代码块 vs 非静态代码块
 * 
 * 4.静态代码块
 *     》内部可以有输出语句
 *  》随着类的加载而执行,而且只执行一次
 *  》作用:初始化类的信息
 *  》如果一个类中，定义了多个静态代码块，则按照声明的先后顺序执行
 *  》静态代码块的执行，优先于非静态代码块的执行
 *  》静态代码块内只能调用静态的属性、静态的方法，不能调用非静态的结构
 * 
 * 5.非静态代码块
 *  >内部可以有输出语句
 *  >随着对象的创建而执行
 *  >每创建一个对象，就执行一次非静态代码块。
 *  >作用:可以在创建对象时，对对象的属性等进行初始化。
 *  >如果一个类中，定义了多个非静态代码块，则按照声明的先后顺序执行
 *  >非静态代码块内可以调用静态的属性、静态的方法，或非静态的属性、非静态的方法。
 *  
 * 对属性可以赋值的位置:
 *  ①默认初始化
 *  ②显式初始化
 *  ③构造器中初始化
 *  ④有了对象以后，可以通过"对象.属性"或"对象.方法"的方式，进行赋值。
 *  ⑤在代码块中赋值
 */
public class BlockTest {
    public static void main(String[] args) {
        
        String desc = Person.desc;
        System.out.println(desc);
        
        Person p1 = new Person();
        Person p2 = new Person();
        System.out.println(p1.age);
        
        Person.info();
    }
}

class Person{
    //属性
    String name;
    int age;
    static String desc = "我是一个青年";
    
    //构造器
    public Person(){
        
    }
    
    //static 的代码块
    static{
        System.out.println("hello,static block-1");
        //调用静态结构
        desc = "我是一个爱小说的人";
        info();
        //不能调用非静态结构
//        eat();
//        name = "Tom";
    }
    
    static{
        System.out.println("hello,static block-2");
    }
    
    //非 static 的代码块
    {
        System.out.println("hello,block-2");
    }
    {
        System.out.println("hello,block-1");
        //调用非静态结构
        age = 1;
        eat();
        //调用静态结构
        desc = "我是一个爱小说的人 1";
        info();
    }    
    
    //方法
    public Person(String name,int age){
        this.name = name;
        this.age = age;
    }
    
    public void eat(){
        System.out.println("吃饭");
    }

    @Override
    public String toString() {
        return "Person [name=" + name + ", age=" + age + "]";
    }
    public static void info(){
        System.out.println("我是一个快乐的人。");
    }
    
}
```

> **静态初始化块举例 1**

```java
//总结:由父类到子类，静态先行
class Root{
    static{
        System.out.println("Root 的静态初始化块");
    }
    {
        System.out.println("Root 的普通初始化块");
    }
    public Root(){
        System.out.println("Root 的无参数的构造器");
    }
}
class Mid extends Root{
    static{
        System.out.println("Mid 的静态初始化块");
    }
    {
        System.out.println("Mid 的普通初始化块");
    }
    public Mid(){
        System.out.println("Mid 的无参数的构造器");
    }
    public Mid(String msg){
        //通过 this 调用同一类中重载的构造器
        this();
        System.out.println("Mid 的带参数构造器，其参数值："
            + msg);
    }
}
class Leaf extends Mid{
    static{
        System.out.println("Leaf 的静态初始化块");
    }
    {
        System.out.println("Leaf 的普通初始化块");
    }    
    public Leaf(){
        //通过 super 调用父类中有一个字符串参数的构造器
        super("尚硅谷");
        System.out.println("Leaf 的构造器");
    }
}
public class LeafTest{
    public static void main(String[] args){
        new Leaf(); 
        //new Leaf();
    }
}
```

> **静态初始化块举例 2**

```java
class Father {
    static {
        System.out.println("11111111111");
    }
    {
        System.out.println("22222222222");
    }

    public Father() {
        System.out.println("33333333333");

    }

}

public class Son extends Father {
    static {
        System.out.println("44444444444");
    }
    {
        System.out.println("55555555555");
    }
    public Son() {
        System.out.println("66666666666");
    }

    public static void main(String[] args) { // 由父及子 静态先行
        System.out.println("77777777777");
        System.out.println("************************");
        new Son();
        System.out.println("************************");

        new Son();
        System.out.println("************************");
        new Father();
    }

}
```

> **总结：程序中成员变量赋值的执行顺序**

![null](https://i-blog.csdnimg.cn/blog_migrate/79677e94b5eeda2057c811f86d873746.png)

```java
/*
 * 对属性可以赋值的位置:
 *  ①默认初始化
 *  ②显式初始化 / ⑤在代码块中赋值
 *  ③构造器中初始化
 *  ④有了对象以后，可以通过"对象.属性"或"对象.方法"的方式，进行赋值。
 *  
 *  执行的先后顺序:① - ② / ⑤ - ③ - ④
 */
public class OrderTest {
    public static void main(String[] args) {
        Order order = new Order();
        System.out.println(order.orderId);
    }
}
class Order{
    
    int orderId = 3;
    {
        orderId = 4;
    }
    
}
```

## 04、关键字：final

```java
/*
 * final:最终的
 * 
 * 1.final可以用来修饰的结构:类、方法、变量
 * 
 * 2.final用来修饰一个类:此类不能被其他类所继承。
 *           比如:String类、System类、StringBuffer类
 * 3.final修饰一个方法:final标记的方法不能被子类重写。
 *           比如：Object类中的getClass()。 
 * 4.final用来修饰变量:此时的"变量"(成员变量或局部变量)就是一个常量。名称大写，且只能被赋值一次。
 *      4.1 final修饰属性，可以考虑赋值的位置有:显式初始化、代码块中初始化、构造器中初始化
 *   4.2 final修饰局部变量:
 *        尤其是使用final修饰形参时，表明此形参是一个常量。当我们调用此方法时，给常量形参赋一个实参。
 *      一旦赋值以后，就只能在方法体内使用此形参，但不能进行重新赋值。
 *      
 * static final 用来修饰:全局常量
 */
public class FinalTest {
    
    final int WIDTH = 0;
    final int LEFT;
    final int RIGHT;
//    final int DOWN;
    
    {
        LEFT = 1;
    }
    
    public FinalTest(){
        RIGHT = 2;
    }
    
    public FinalTest(int n){
        RIGHT = n;
    }
    
//    public void setDown(int down){
//        this.DOWN = down;
//    }
    
    public void dowidth(){
//        width = 20;    //width cannot be resolved to a variable
    }
    
    public void show(){
        final int NUM = 10;    //常量
//        num += 20;
    }
    
    public void show(final int num){
        System.out.println(num);
    }
    
    public static void main(String[] args) {
        
        int num = 10;
        
        num = num + 5;
        
        FinalTest test = new FinalTest();
//        test.setDown(5);
        
        test.show(10);
    }
}

final class FianlA{
    
}

//class B extends FinalA{     //错误，不能被继承。
//    
//}

//class C extends String{
//    
//}

class AA{
    public final void show(){
        
    }
}

//class BB extends AA{    // 错误，不能被重写。
//    public void show(){
//        
//    }
//}
```

> 1、**面试题1**

```java
public class Something {
    public int addOne(final int x) {
        return ++x; // return x + 1;
    }
}
```

> 2、**面试题2**

```java
public class Something {

    public static void main(String[] args) {
        Other o = new Other();
        new Something().addOne(o);
    }

    public void addOne(final Other o) {
        // o = new Other();
        o.i++;
    }
}

class Other {
    public int i;
}
```

## 05、抽象类与抽象方法

随着继承层次中一个个新子类的定义，类变得越来越具体，而父类则更一般，更通用。类的设计应该保证父类和子类能够共享特征。有时将一个父类设计得非常抽象，以至于它没有具体的实例，这样的类叫做**抽象类**。

![null](https://i-blog.csdnimg.cn/blog_migrate/f3f8b120baa400ac35f4c537125a39cd.png)

```java
/*
 * abstract 关键字的使用
 * 
 * 1.abstract:抽象的
 * 2.abstract 可以用来修饰的结构:类、方法
 * 3.abstract 修饰类:抽象类
 *     》 此类不能实例化
 *  》 抽象类中一定有构造器，便于子类实例化时调用(涉及:子类对象实例化全过程)
 *  》 开发中，都会提供抽象类的子类，让子类对象实例化，实现相关的操作
 * 
 * 4.abstract 修饰方法:抽象方法
 *  > 抽象方法，只有方法的声明，没有方法体。
 *  > 包含抽象方法的类，一定是一个抽象类。反之，抽象类中可以没有抽象方法
 *  > 若子类重写了父类中所有的抽象方法，此子类，
 *
 * abstract 使用上的注意点:
 * 1.abstract 不能用来修饰变量、代码块、构造器；
 * 
 * 2.abstract 不能用来修饰私有方法、静态方法、final 的方法、final 的类。
 * 
 */
public class AbstractTest {
    public static void main(String[] args) {
        //一旦 Person 类抽象了，就不可实例化
//        Person p1 = new Person();
//        p1.eat();
        
    }
}

abstract class Creature{
    public abstract void breath();
}

abstract class Person extends Creature{
    String name;
    int age;
    
    public Person(){
        
    }
    
    public Person(String name,int age){
        this.name = name;
        this.age = age;
    }
    
    //不是抽象方法
//    public void eat(){
//        System.out.println("人吃饭");
//    }
    
    //抽象方法
    public abstract void eat();
    
    public void walk(){
        System.out.println("人走路");
    }
}

class Student extends Person{
    public Student(String name,int age){
        super(name,age);
    }
    public void eat(){
        System.out.println("学生应该多吃有营养的。");
    }
    @Override
    public void breath() {
        System.out.println("学生应该呼吸新鲜的无雾霾空气");
    }
}
```

### 5.1、抽象类应用

> 抽象类是用来模型化那些父类无法确定全部实现，而是由其子类提供具体实现的对象的类。

![null](https://i-blog.csdnimg.cn/blog_migrate/2a5720ede6f6568ac23f86ab7e10815a.png)

> 问题：卡车(Truck)和驳船(RiverBarge)的燃料效率和行驶距离的计算方法完全不同。Vehicle 类不能提供计算方法，但子类可以。

```java
/* Java 允许类设计者指定：超类声明一个方法但不提供实现，该方法的实现由子类提  供。这样的方法称为抽象方法。有一个或更多抽象方法的类称为抽象类。
 * Vehicle 是一个抽象类，有两个抽象方法。
 * 注意：抽象类不能实例化 new Vihicle()是非法的
 */
public abstract class Vehicle{
    public abstract double calcFuelEfficiency();//计算燃料效率的抽象方法
    public abstract double calcTripDistance();//计算行驶距离的抽象方法
}
public class Truck extends Vehicle{
    public double calcFuelEfficiency(){ 
        //写出计算卡车的燃料效率的具体方法
    }
    public double calcTripDistance(){ 
        //写出计算卡车行驶距离的具体方法
    }
}
public class RiverBarge extends Vehicle{
    public double calcFuelEfficiency() { 
        //写出计算驳船的燃料效率的具体方法
    }
    public double calcTripDistance( )  {  
        //写出计算驳船行驶距离的具体方法
    }
}
```

### 5.2、练习

```java
/*
 * 编写一个 Employee 类，声明为抽象类，
 * 包含如下三个属性：name，id，salary。
 * 提供必要的构造器和抽象方法：work()。
 * 对于 Manager 类来说，他既是员工，还具有奖金(bonus)的属性。
 * 请使用继承的思想，设计 CommonEmployee 类和 Manager 类，
 * 要求类中提供必要的方法进行属性访问。
 * 
 */
public abstract class Employee {
    
    private String name;
    private int id;
    private double salary;
    
    public Employee(){
        super();
    }

    public Employee(String name, int id, double salary) {
        super();
        this.name = name;
        this.id = id;
        this.salary = salary;
    }
    
    public abstract void work();    
}
```

> Manager 类

```java
/*
 * 对于 Manager 类来说，他既是员工，还具有奖金(bonus)的属性。
 * 
 */
public class Manager extends Employee{

    private double bonus;    //奖金
    
    public Manager(double bonus) {
        super();
        this.bonus = bonus;
    }
    
    public Manager(String name, int id, double salary, double bonus) {
        super(name, id, salary);
        this.bonus = bonus;
    }


    @Override
    public void work() {
        System.out.println("管理员工，提高公司运行效率。");        
    }
}
```

> CommonEmployee 类

```java
public class CommonEmployee extends Employee {

    @Override
    public void work() {
        System.out.println("员工在一线车间生产产品。");
    }

}
```

> 测试类

```java
/*
 * 请使用继承的思想，设计 CommonEmployee 类和 Manager 类，
 */
public class EmployeeTest {
    public static void main(String[] args) {
        
        Employee manager = new Manager("库克",1001,5000,50000);
        
        manager.work();
        
        CommonEmployee commonEmployee = new CommonEmployee();
        commonEmployee.work();
    }
}
```

### 5.3、创建抽象类的匿名子类对象

```java
public class Num {

}

abstract class Creature{
    public abstract void breath();
}

abstract class Person extends Creature{
    String name;
    int age;
    
    public Person(){
        
    }
    
    public Person(String name,int age){
        this.name = name;
        this.age = age;
    }
    
    //不是抽象方法
//    public void eat(){
//        System.out.println("人吃饭");
//    }
    
    //抽象方法
    public abstract void eat();
    
    public void walk(){
        System.out.println("人走路");
    }
}

class Student extends Person{
    public Student(String name,int age){
        super(name,age);
    }
    public Student(){

    }
    public void eat(){
        System.out.println("学生应该多吃有营养的。");
    }
    @Override
    public void breath() {
        System.out.println("学生应该呼吸新鲜的无雾霾空气");
    }
}
```

> PersonTest 类

```java
/*
 * 抽象类的匿名子类
 * 
 */
public class PersonTest {
    public static void main(String[] args) {
        
        method(new Student());    //匿名对象
        
        Worker worker = new Worker(); 
        method1(worker);    //非匿名的类非匿名的对象
        
        method1(new Worker());    //非匿名的类匿名的对象
        
        System.out.println("*********************");
        
        //创建了一个匿名子类的对象:p
        Person p = new Person(){

            @Override
            public void eat() {
                System.out.println("吃东西");
            }

            @Override
            public void breath() {
                System.out.println("呼吸空气");
            }
            
        };
        method1(p);
        System.out.println("**********************"); 
        //创建匿名子类的匿名对象
        method1(new Person(){

            @Override
            public void eat() {
                System.out.println("吃零食");
            }

            @Override
            public void breath() {
                System.out.println("云南的空气");
            }
            
        });
    }
    
    public static void method1(Person p){
        p.eat();
        p.walk();
    }
    
    public static void method(Student s){
        
    }
}
class Worker extends Person{
    
    @Override
    public void eat() {
    }

    @Override
    public void breath() {
    }
}
```

### 5.4、多态的应用：模板方法设计模式(TemplateMethod)

抽象类体现的就是一种模板模式的设计，抽象类作为多个子类的通用模板，子类在抽象类的基础上进行扩展、改造，但子类总体上会保留抽象类的行为方式。

> 解决的问题：

当功能内部一部分实现是确定的，一部分实现是不确定的。这时可以把不确定的部分暴露出去，让子类去实现。
换句话说，**在软件开发中实现一个算法时，整体步骤很固定、通用，这些步骤已经在父类中写好了。但是某些部分易变，易变部分可以抽象出来，供不同子类实现。这就是一种模板模式。**

> 1、例 1

```java
/*
 * 抽象类的应用:模板方法的设计模式
 */
public class TemplateTest {
    public static void main(String[] args) {
        
        SubTemlate t = new SubTemlate();
        
        t.sendTime();
    }
}
abstract class Template{
    
    //计算某段代码执行所需花费的时间
    public void sendTime(){
        
        long start = System.currentTimeMillis();
        
        code();    //不确定部分，易变的部分
        
        long end = System.currentTimeMillis();
        
        System.out.println("花费的时间为:" + (end - start));
    }
    
    public abstract void code();
}

class SubTemlate extends Template{
    
    @Override
    public void code() {
        
        for(int i = 2;i <= 1000;i++){
            boolean isFlag = true;
            for(int j = 2;j <= Math.sqrt(i);j++){
                if(i % j == 0){
                    isFlag = false;
                    break;
                }
            }
            if(isFlag){
                System.out.println(i);
            }
        }
    }
}
```

> 2、例 2

```java
//抽象类的应用：模板方法的设计模式
public class TemplateMethodTest {

    public static void main(String[] args) {
        BankTemplateMethod btm = new DrawMoney();
        btm.process();

        BankTemplateMethod btm2 = new ManageMoney();
        btm2.process();
    }
}
abstract class BankTemplateMethod {
    // 具体方法
    public void takeNumber() {
        System.out.println("取号排队");
    }

    public abstract void transact(); // 办理具体的业务 //钩子方法

    public void evaluate() {
        System.out.println("反馈评分");
    }

    // 模板方法，把基本操作组合到一起，子类一般不能重写
    public final void process() {
        this.takeNumber();

        this.transact();// 像个钩子，具体执行时，挂哪个子类，就执行哪个子类的实现代码

        this.evaluate();
    }
}

class DrawMoney extends BankTemplateMethod {
    public void transact() {
        System.out.println("我要取款！！！");
    }
}

class ManageMoney extends BankTemplateMethod {
    public void transact() {
        System.out.println("我要理财！我这里有 2000 万美元!!");
    }
}
```

> 模板方法设计模式是编程中经常用得到的模式。各个框架、类库中都有他的影子，比如常见的有：

•数据库访问的封装•Junit 单元测试•JavaWeb 的 Servlet 中关于 doGet/doPost 方法调用•Hibernate 中模板程序•Spring 中 JDBCTemlate、HibernateTemplate 等

### 5.5、抽象类的练习

![null](https://i-blog.csdnimg.cn/blog_migrate/3e2e11684552c6ac28d8c7297ae7d732.png)



![null](https://i-blog.csdnimg.cn/blog_migrate/1d853f92a4d9bd888b0769f55b832394.png)

> 1、Employee 类

```java
/*
 * 定义一个 Employee 类，
 * 该类包含：private 成员变量 name,number,birthday，
 * 其中 birthday 为 MyDate 类的对象；
 * abstract 方法 earnings()；
 * toString()方法输出对象的 name,number 和 birthday。
 * 
 */
public abstract class Employee {
    private String name;
    private int number;
    private MyDate birthday;
    
    public Employee(String name, int number, MyDate birthday) {
        super();
        this.name = name;
        this.number = number;
        this.birthday = birthday;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public int getNumber() {
        return number;
    }

    public void setNumber(int number) {
        this.number = number;
    }

    public MyDate getBirthday() {
        return birthday;
    }

    public void setBirthday(MyDate birthday) {
        this.birthday = birthday;
    }

    public abstract double earnings();

    @Override
    public String toString() {
        return "name=" + name + ", number=" + number + ", birthday=" + birthday.toDateString() + "]";
    }
    
}
```

> 2、MyDate 类

```java
/*
 * MyDate 类包含:private 成员变量 year,month,day；
 * toDateString()方法返回日期对应的字符串：xxxx 年 xx 月 xx 日
 */
public class MyDate {
    private int year;
    private int month;
    private int day;
    
    public MyDate(int year, int month, int day) {
        super();
        this.year = year;
        this.month = month;
        this.day = day;
    }

    public int getYear() {
        return year;
    }

    public void setYear(int year) {
        this.year = year;
    }

    public int getMonth() {
        return month;
    }

    public void setMonth(int month) {
        this.month = month;
    }

    public int getDay() {
        return day;
    }

    public void setDay(int day) {
        this.day = day;
    }

    public String toDateString(){
        return year + "年" + month + "月" + day + "日";
    }
}
```

> 3、SalariedEmployee 类

```java
/*
 * 定义 SalariedEmployee 类继承 Employee 类，实现按月计算工资的员工处理。
 * 该类包括：private 成员变量 monthlySalary；实现父类的抽象方法 earnings(),
 * 该方法返回 monthlySalary 值；
 * toString()方法输出员工类型信息及员工的 name，number,birthday。
 * 
 */
public class SalariedEmployee extends Employee{
    private double monthlySalary;    //月工资

    public SalariedEmployee(String name,int number,MyDate birthday) {
        super(name,number,birthday);
    }
    
    public SalariedEmployee(String name, int number, MyDate birthday, double monthlySalary) {
        super(name, number, birthday);
        this.monthlySalary = monthlySalary;
    }

    @Override
    public double earnings() {
        return monthlySalary;        
    }

    @Override
    public String toString() {
        return "SalariedEmployee [" + super.toString() + "]";
    }    
}
```

> 4、HourlyEmployee 类

```java
/*
 * 参照 SalariedEmployee 类定义 HourlyEmployee 类，
 * 实现按小时计算工资的员工处理。该类包括：private 成员变量 wage 和 hour；
 * 实现父类的抽象方法 earnings(),该方法返回 wage*hour 值；
 * toString()方法输出员工类型信息及员工的 name，number,birthday。
 * 
 */
public class HourlyEmployee extends Employee{
    private int wage;    //每小时的工资
    private int hour;    //月工作的小时数
    
    public HourlyEmployee(String name, int number, MyDate birthday) {
        super(name, number, birthday);
    }

    public HourlyEmployee(String name, int number, MyDate birthday, int wage, int hour) {
        super(name, number, birthday);
        this.wage = wage;
        this.hour = hour;
    }

    @Override
    public double earnings() {
        return wage*hour;
    }

    public int getWage() {
        return wage;
    }

    public void setWage(int wage) {
        this.wage = wage;
    }

    public int getHour() {
        return hour;
    }

    public void setHour(int hour) {
        this.hour = hour;
    }
    
    public String toString(){
        return "HourlyEmployee[" + super.toString() + "]"; 
    }
}
```

> 5、PayrollSystem 类

```java
import java.util.Calendar;
import java.util.Scanner;
/*
 * 定义 PayrollSystem 类，创建 Employee 变量数组并初始化，
 * 该数组存放各类雇员对象的引用。利用循环结构遍历数组元素，
 * 输出各个对象的类型,name,number,birthday,以及该对象生日。
 * 当键盘输入本月月份值时，
 * 如果本月是某个 Employee 对象的生日，还要输出增加工资信息。
 * 
 */
public class PayrollSystem {
    public static void main(String[] args) {
        //方式一：
//        Scanner scanner = new Scanner(System.in);
//        System.out.println("请输入当月的月份：");
//        int month = scanner.nextInt();
        
        //方式二：
        Calendar calendar = Calendar.getInstance();
        int month = calendar.get(Calendar.MONTH);//获取当前的月份
//        System.out.println(month);//一月份：0
        
        Employee[] emps = new Employee[2];
        
        emps[0] = new SalariedEmployee("马良", 1002,new MyDate(1992, 2, 28),10000);
        emps[1] = new HourlyEmployee("博西", 2001, new MyDate(1991, 1, 6),60,240);
        
        for(int i = 0;i < emps.length;i++){
            System.out.println(emps[i]);
            double salary = emps[i].earnings();
            System.out.println("月工资为：" + salary);
            
            if((month+1) == emps[i].getBirthday().getMonth()){
                System.out.println("生日快乐！奖励 100 元");
            }
            
        }
    }
}
```

## 06、接口(interface)

### 6.1、概述

一方面，有时必须从几个类中派生出一个子类，继承它们所有的属性和方法。但是，Java 不支持多重继承。有了接口，就可以得到多重继承的效果。

另一方面，有时必须从几个类中抽取出一些共同的行为特征，而它们之间又没有 is-a 的关系，仅仅是具有相同的行为特征而已。例如：鼠标、键盘、打印机、扫描仪、摄像头、充电器、MP3 机、手机、数码相机、移动硬盘等都支持 USB 连接。

接口就是规范，定义的是一组规则，体现了现实世界中“如果你是/要…则必须能…”的思想。**继承是一个"是不是"的关系，而接口实现则是"能不能"的关系。**

**接口的本质是契约，标准，规范**，就像我们的法律一样。制定好后大家都要遵守。

![null](https://i-blog.csdnimg.cn/blog_migrate/da75a0ad9e05bf88c4d191d7a23de25f.png)

```java
/* 接口(interface)是抽象方法和常量值定义的集合。
 * 接口的特点：
 * 用 interface 来定义。
 * 接口中的所有成员变量都默认是由 public static final 修饰的。
 * 接口中的所有抽象方法都默认是由 public abstract 修饰的。
 * 接口中没有构造器。
 * 接口采用多继承机制。
 */
```

![null](https://i-blog.csdnimg.cn/blog_migrate/dfbb9a5437200f03e4588e9688ce87c8.png)

```java
/*
 * 接口的使用
 * 1.接口使用 interface 来定义。
 * 2.在 Java 中:接口和类是并列的两个结构
 * 3.如何去定义两个接口:定义接口中的成员
 *     》3.1 JDK7 及以前:只能定义全局常量和抽象方法
 *         》全局常量:public static final 的,但是书写中，可以省略不写。
 *         》抽象方法:public abstract 的
 * 
 *  》3.2 JDK8:除了全局常量和抽象方法之外，还可以定义静态方法、默认方法(略)。
 * 
 * 4.接口中不能定义构造器！意味着接口不可以实例化。
 * 
 * 5.Java 开发中，接口通过让类去实现(implements)的方式来使用。
 *   如果实现类覆盖了接口中的所有方法，则此实现类就可以实例化
 *   如果实现类没有覆盖接口中所有的抽象方法，则此实现类仍为一个抽象类
 * 
 * 6.Java 类可以实现多个接口 ---》弥补了 Java 单继承性的局限性
 *  格式:class AA extends BB implementd CC,DD,EE
 *  
 *  7.接口与接口之间是继承,而且可以多继承
 *  
 **********************************
 * 8.接口的具体使用，体现多态性
 *        接口的主要用途就是被实现类实现。（面向接口编程）
 * 9.接口，实际可以看作是一种规范
 * 
 * 面试题:抽象类与接口有哪些异同？
 *  
 */
public class InterfaceTest {
    public static void main(String[] args) {
        System.out.println(Flayable.MAX_SPEED);
        System.out.println(Flayable.MIN_SPEED);
    }
}
interface Flayable{
    
    //全局变量
    public static final int MAX_SPEED = 7900;    
    int MIN_SPEED = 1;//省略了 public static final 
    
    //抽象方法
    public abstract void fly();
    
    void stop();//省略了 public abstract 
    //Interfaces cannot have constructors
//    public Flayable(){
//        
//    }    
}
interface Attackable{
    void attack();
}

class Plane implements Flayable{

    @Override
    public void fly() {
        System.out.println("飞机通过引擎起飞");
        
    }

    @Override
    public void stop() {
        System.out.println("驾驶员减速停止");
    }
    
}
abstract class Kite implements Flayable{

    @Override
    public void fly() {
        
    }
}

class Bullet extends Object implements Flayable,Attackable,CC{

    @Override
    public void attack() {
        // TODO Auto-generated method stub
        
    }

    @Override
    public void fly() {
        // TODO Auto-generated method stub
        
    }

    @Override
    public void stop() {
        // TODO Auto-generated method stub
        
    }

    @Override
    public void method1() {
        // TODO Auto-generated method stub
        
    }

    @Override
    public void method2() {
        // TODO Auto-generated method stub
        
    }
}

//*********************************
interface AA{
    void method1();
}
interface BB{
    void method2();
}
interface CC extends AA,BB{
    
}
```

![null](https://i-blog.csdnimg.cn/blog_migrate/e1a9cba5e7092e46300113daf2f9ce6d.png)



![null](https://i-blog.csdnimg.cn/blog_migrate/d94c56f13d31fde626d5689dca4be24a.png)

### 6.2、举例

```java
/*
 * 接口的使用
 * 1.接口使用上也满足多态性
 * 2.接口，实际上就是定义了一种规范
 * 3.开发中，体会面向接口编程！
 * 
 */
public class USBTest {
    public static void main(String[] args) {
        
        Computer com = new Computer();
        //1.创建了接口的非匿名实现类的非匿名对象
        Flash flash = new Flash();
        com.transferData(flash); 
        //2. 创建了接口的非匿名实现类的匿名对象
        com.transferData(new Printer());
        //3. 创建了接口的匿名实现类的非匿名对象
        USB phone = new USB(){

            @Override
            public void start() {
                System.out.println("手机开始工作");
            }

            @Override
            public void stop() {
                System.out.println("手机结束工作");
            }
            
        };
        com.transferData(phone);
        //4. 创建了接口的匿名实现类的匿名对象
        com.transferData(new USB(){
            @Override
            public void start() {
                System.out.println("mp3 开始工作");
            }

            @Override
            public void stop() {
                System.out.println("mp3 结束工作");
            }
        });
    }
}

class Computer{
    
    public void transferData(USB usb){//USB usb = new Flash();
        usb.start();
        
        System.out.println("具体传输数据的细节");
        
        usb.stop();
    }
    
}

interface USB{
    //常量:定义了长、宽
    void start();
    
    void stop();
}
class Flash implements USB{

    @Override
    public void start() {
        System.out.println("U 盘开始工作");
    }

    @Override
    public void stop() {
        System.out.println("U 盘结束工作");
    }
}
class Printer implements USB{
    @Override
    public void start() {
        System.out.println("打印机开启工作");
    }

    @Override
    public void stop() {
        System.out.println("打印机结束工作");
    }
    
}
```

### 6.3、接口的应用：代理模式(Proxy)

代理模式是 Java 开发中使用较多的一种设计模式。代理设计就是为其他对象提供一种代理以控制对这个对象的访问。

![null](https://i-blog.csdnimg.cn/blog_migrate/cce5e36fbe966b5dcabd919f8708da73.png)

```java
/*
 * 接口的应用:代理模式
 * 
 * 
 */
public class NetWorkTest {
    public static void main(String[] args) {
        
        Server server = new Server();
//        server.browse();
        ProxyServer proxyServer = new ProxyServer(server);
        
        proxyServer.browse();
    }
}
interface NetWork{
    public void browse();
    
}
//被代理类
class Server implements NetWork{


    @Override
    public void browse() {
        System.out.println("真实的服务器来访问网络");
    }
}
//代理类
class ProxyServer implements NetWork{
    
    private NetWork work;
    
    public ProxyServer(NetWork work){
        this.work = work;
    }
    
    public void check(){
        System.out.println("联网前的检查工作");
    }

    @Override
    public void browse() {
        check();
        
        work.browse();
    }
    
}
```

> 应用场景：

•安全代理：屏蔽对真实角色的直接访问。•远程代理：通过代理类处理远程方法调用（RMI）•延迟加载：先加载轻量级的代理对象，真正需要再加载真实对象

比如你要开发一个大文档查看软件，大文档中有大的图片，有可能一个图片有 100MB，在打开文件时，不可能将所有的图片都显示出来，这样就可以使用代理模式，当需要查看图片时，用 proxy 来进行大图片的打开。

> 分类

•静态代理（静态定义代理类）•动态代理（动态生成代理类）•JDK 自带的动态代理，需要反射等知识

```java
public class StaticProxyTest {

    public static void main(String[] args) {
        Proxy s = new Proxy(new RealStar());
        s.confer();
        s.signContract();
        s.bookTicket();
        s.sing();
        s.collectMoney();
    }
}

interface Star {
    void confer();// 面谈

    void signContract();// 签合同

    void bookTicket();// 订票

    void sing();// 唱歌

    void collectMoney();// 收钱
}
//被代理类
class RealStar implements Star {

    public void confer() {
    }

    public void signContract() {
    }

    public void bookTicket() {
    }

    public void sing() {
        System.out.println("明星：歌唱~~~");
    }

    public void collectMoney() {
    }
}

//代理类
class Proxy implements Star {
    private Star real;

    public Proxy(Star real) {
        this.real = real;
    }

    public void confer() {
        System.out.println("经纪人面谈");
    }

    public void signContract() {
        System.out.println("经纪人签合同");
    }

    public void bookTicket() {
        System.out.println("经纪人订票");
    }

    public void sing() {
        real.sing();
    }

    public void collectMoney() {
        System.out.println("经纪人收钱");
    }
}
```

### 6.4、接口的应用：工厂模式

拓展：工厂设计模式.pdf

> 接口和抽象类之间的对比

| No.  | 区别点       | 抽象类                                                       | 接口                                        |
| ---- | ------------ | ------------------------------------------------------------ | ------------------------------------------- |
| 1    | 定义         | 包含抽象方法的类                                             | 主要是抽象方法和全局常量的集合              |
| 2    | 组成         | 构造方法、抽象方法、普通方法、常量、变量                     | 常量、抽象方法、(jdk8.0:默认方法、静态方法) |
| 3    | 使用         | 子类继承抽象类(extends)                                      | 子类实现接口(implements)                    |
| 4    | 关系         | 抽象类可以实现多个接口                                       | 接口不能继承抽象类，但允许继承多个接口      |
| 5    | 常见设计模式 | 模板方法                                                     | 简单工厂、工厂方法、代理模式                |
| 6    | 对象         | 都通过对象的多态性产生实例化对象                             |                                             |
| 7    | 局限         | 抽象类有单继承的局限                                         | 接口没有此局限                              |
| 8    | 实际         | 作为一个模板                                                 | 是作为一个标准或是表示一种能力              |
| 9    | 选择         | 如果抽象类和接口都可以使用的话，优先使用接口，因为避免单继承的局限 |                                             |

> 在开发中，常看到一个类不是去继承一个已经实现好的类，而是要么继承抽象类，要么实现接口。
> -【面试题】排错：

```java
interface A {
    int x = 0;
}
class B {
    int x = 1;
}
class C extends B implements A {
    public void pX() {
//        编译不通过，x 不明确
        System.out.println(x);
//        System.out.println(super.x); //1
//        System.out.println(A.x);//0
    }
    public static void main(String[] args) {
        new C().pX();
    }
}
```

> 排错 2：

```java
interface Playable {
    void play();
}
interface Bounceable {
    void play();
}
interface Rollable extends Playable, Bounceable {
    Ball ball= new Ball("PingPang"); //省略了 public static final
}
public class Ball implements Rollable {
    private String name;
    public String getName() {
        return name;
    }
    public Ball(String name) {
        this.name= name;
    }
    public void play() {
        ball = new Ball("Football"); //The final field Rollable.ball cannot be assigned    
        System.out.println(ball.getName());
    }
}
```

> 练习

![null](https://i-blog.csdnimg.cn/blog_migrate/be396bd6e141b15e790e9a08b425b6f0.png)

CompareObject 类

```java
/*
 * 定义一个接口用来实现两个对象的比较。
 * 
 */
public interface CompareObject {
    public int compareTo(Object o);
    //若返回值是 0,代表相等;若为正数，代表当前对象大；负数代表当前对象小
    
}
```

Circle 类

```java
/*
 * 定义一个 Circle 类，声明 redius 属性，提供 getter 和 setter 方法
 */
public class Circle {
    
    private Double radius;

    public Double getRadius() {
        return radius;
    }

    public void setRadius(Double radius) {
        this.radius = radius;
    }

    public Circle() {
        super();
    }

    public Circle(Double radius) {
        super();
        this.radius = radius;
    }
        
}
```

ComparableCircle 类

```java
/*
 * 定义一个 ComparableCircle 类，继承 Circle 类并且实现 CompareObject 接口。在 ComparableCircle 类中给出接口中方法 compareTo 的实现体，
 * 用来比较两个圆的半径大小。
 */
public class ComparableCircle extends Circle implements CompareObject{

    public ComparableCircle(double radius) {
        super(radius);
    }
    @Override
    public int compareTo(Object o) {
        if(this == o){
            return 0;
        }
        if(o instanceof ComparableCircle){
            ComparableCircle c = (ComparableCircle)o;
            //错误的写法
//            return (int)(this.getRedius() - c.getRedius());
            //正确的方式一：
//            if(this.getRadius() > c.getRadius()){
//                return 1;
//            }else if(this.getRadius() < c.getRadius()){
//                return -1;
//            }else{
//                return 0;
//            }
            //当属性 radius 声明为 Double 类型时，可以调用包装类的方法
            //正确的方式二：
            return this.getRadius().compareTo(c.getRadius());
        }else{
            return 0;
//            throw new RuntimeException("传入数据类型不匹配");
        }
    }
}
```

InterfaceTest 类

```java
/*
 * 定义一个测试类 InterfaceTest，创建两个 ComparableCircle 对象，
 * 调用 compareTo 方法比较两个类的半径大小。
 * 
 */
public class InterfaceTest {
    public static void main(String[] args) {
        
        ComparableCircle c1 = new ComparableCircle(3.4);
        ComparableCircle c2 = new ComparableCircle(3.6);
        
        int compareValue = c1.compareTo(c2);
        if(compareValue > 0){
            System.out.println("c1 对象大");
        }else if(compareValue < 0){
            System.out.println("c2 对象大");
        }else{
            System.out.println("两个一样的");
        }
        
        int compareValue1 = c1.compareTo(new String("AA"));
        System.out.println(compareValue1);
    }
}
```

## 07、Java 8 中关于接口的改进

Java 8 中，你可以为接口添加静态方法和默认方法。从技术角度来说，这是完全合法的，只是它看起来违反了接口作为一个抽象定义的理念。

> 静态方法：

使用 static 关键字修饰。可以通过接口直接调用静态方法，并执行其方法体。我们经常在相互一起使用的类中使用静态方法。你可以在标准库中找到像 Collection/Collections 或者 Path/Paths 这样成对的接口和类。

> 默认方法：

默认方法使用 default 关键字修饰。可以通过实现类对象来调用。我们在已有的接口中提供新方法的同时，还保持了与旧版本代码的兼容性。比如：java 8 API 中对 Collection、List、Comparator 等接口提供了丰富的默认方法。

> 例1

interface 类

```java
/*
 * JDK8:除了全局常量和抽象方法之外，还可以定义静态方法、默认方法(略)。
 * 
 * 
 */
public interface CompareA {

    //静态方法
    public static void method1() {
        System.out.println("CompareA:西安");
    }
    
    //默认方法
    public default void method2(){
        System.out.println("CompareA:深圳");
    }
    
    default void method3(){
        System.out.println("CompareA:杭州");
    }
}
```

SubClassTest 类

```java
public class SubClassTest {

    public static void main(String[] args) {
        SubClass s = new SubClass();
//        s.method1();
//        SubClass.method1();
//        知识点 1：接口中定义的静态方法，只能通过接口来调用。
        CompareA.method1();
//        知识点 2：通过实现类的对象，可以调用接口中的默认方法。
//        如果实现类重写了接口中的默认方法，调用时，仍然调用的是重写以后的方法
        s.method2();
//        知识点 3：如果子类(或实现类)继承的父类和实现的接口中声明了同名同参数的默认方法，
//        那么子类在没有重写此方法的情况下，默认调用的是父类中的同名同参数的方法。-->类优先原则
//        知识点 4：如果实现类实现了多个接口，而这多个接口中定义了同名同参数的默认方法，
//        那么在实现类没有重写此方法的情况下，报错。-->接口冲突。
//        这就需要我们必须在实现类中重写此方法
        s.method3();
        
    }
}
class SubClass extends SuperClass implements CompareA,CompareB{
    
    public void method2(){
        System.out.println("SubClass：上海");
    }
    
    public void method3(){
        System.out.println("SubClass：深圳");
    }
    
//    知识点 5：如何在子类(或实现类)的方法中调用父类、接口中被重写的方法
    public void myMethod(){
        method3(); //调用自己定义的重写的方法
        super.method3(); //调用的是父类中声明的
//        调用接口中的默认方法
        CompareA.super.method3();
        CompareB.super.method3();
    }
}
```

SuperClass 类

```java
public class SuperClass {
    public void method3(){
        System.out.println("SuperClass:北京");
    }
}
```

CompareB 类

```java
public interface CompareB {
    default void method3(){
        System.out.println("CompareB：上海");
    }
}
```

> 例2

```java
/*
 * 练习：接口冲突的解决方式
 */
interface Filial {// 孝顺的
    default void help() {
        System.out.println("老妈，我来救你了");
    }
}

interface Spoony {// 痴情的
    default void help() {
        System.out.println("媳妇，别怕，我来了");
    }
}

class Father{
    public void help(){
        System.out.println("儿子，救我媳妇！");
    }
}

class Man extends Father implements Filial, Spoony {

    @Override
    public void help() {
        System.out.println("我该就谁呢？");
        Filial.super.help();
        Spoony.super.help();
    }
    
}
```

## 08、类的内部成员之五：内部类

当一个事物的内部，还有一个部分需要一个完整的结构进行描述，而这个内部的完整的结构又只为外部事物提供服务，那么整个内部的完整结构最好使用内部类。

```java
/*
 * 类的内部成员之五:内部类
 * 
 * 1.Java中允许将一个类A声明在另一个类B中,则类A就是内部类,类B就是外部类.
 * 
 * 2.内部类的分类:成员内部类    VS    局部内部类(方法内、代码块内、构造器内)
 *         
 * 3.成员内部类
 *     》作为外部类的成员,
 *         - 调用外部类的结构
 *         - 可以被static修饰
 *         - 可以被4种不同的权限修饰
 * 
 *  》作为一个类，
 *      - 类内可以定义属性、方法、构造器等
 *      - 可以被final修饰，表示此类不能被继承。言外之意，不使用final，就可以被继承
 *      - 可以abstract修饰
 * 
 * 4.关注如下的3个问题
 *   》 如何实例化成员内部类的对象
 *   》 如何在成员内部类中区分调用外部类的结构
 *   》 开发中局部内部类的使用  见《InnerClassTest1.java》
 */
public class InnerClassTest {
    public static void main(String[] args) {
        
        //创建Dog实例(静态的成员内部类)
        Person.Dog dog = new Person.Dog();
        dog.show();
        
        //创建Bird实例(非静态的成员内部类)
//        Person.Bird bird = new Person.Bird();
        Person p = new Person();
        Person.Bird bird = p.new Bird();
        bird.sing();
        
        System.out.println();
        
        bird.display("喜鹊");
    }
}
class Person{
    String name = "李雷";
    int age;
    
    public void eat(){
        System.out.println("人，吃饭");
    }
    
    //静态成员内部类
    static class Dog{
        String name;
        int age;
        
        public void show(){
            System.out.println("卡拉是条狗");
//            eat();
        }
    }
    
    //非静态成员内部类
    class Bird{
        String name = "杜鹃";
        public Bird(){
            
        }
        
        public void sing(){
            System.out.println("我是一只猫头鹰");
            Person.this.eat();//调用外部类的非静态属性
            eat();
            System.out.println(age);
        }
        
        public void display(String name){
            System.out.println(name);    //方法的形参
            System.out.println(this.name);    //内部类的属性
            System.out.println(Person.this.name);    //外部类的属性
        }
    }
    public void method(){
        //局部内部类
        class AA{
            
        }
    }
    
    {
        //局部内部类
        class BB{
            
        }
    }
    
    public Person(){
        //局部内部类
        class CC{
            
        }
    }
}
```

> InnerClassTest1类

```java
public class InnerClassTest1 {
    
//    开发中很少见
    public void method(){
//        局部内部类
        class AA{
            
        }
    }
    
//    返回一个实现了Comparable接口的类的对象
    public Comparable getComparable(){
        
//        创建一个实现了Comparable接口的类:局部内部类
        //方式一：
//        class MyComparable implements Comparable{
//
//            @Override
//            public int compareTo(Object o) {
//                return 0;
//            }
//            
//        }
//        
//        return new MyComparable();
        
        //方式二：
        return new Comparable(){


            @Override
            public int compareTo(Object o) {
                return 0;
            }
            
        };
        
    }
}
```

### 8.1、匿名内部类

```java
/*
 * 1.匿名内部类不能定义任何静态成员、方法和类，只能创建匿名内部类的一个实例。
 * 一个匿名内部类一定是在new的后面，用其隐含实现一个接口或实现一个类。
 * 
 * 2.格式：
 *         new 父类构造器（实参列表）|实现接口(){
 *                 //匿名内部类的类体部分
 *         }
 * 
 * 3.匿名内部类的特点
 *         > 匿名内部类必须继承父类或实现接口
 *         > 匿名内部类只能有一个对象
 *         > 匿名内部类对象只能使用多态形式引用
 */
interface Product{
    public double getPrice();
    public String getName();
}
public class AnonymousTest{
    public void test(Product p){
        System.out.println("购买了一个" + p.getName() + "，花掉了" + p.getPrice());
    }
    public static void main(String[] args) {
        AnonymousTest ta = new AnonymousTest();
        //调用test方法时，需要传入一个Product参数，
        //此处传入其匿名实现类的实例
        ta.test(new Product(){
            public double getPrice(){
                return 567.8;
            }
            public String getName(){
                return "AGP显卡";
            }
        });
    }
}
```

### 8.2、局部内部类的使用注意

```java
public class InnerClassTest {
    
//    public void onCreate(){
//    
//    int number = 10;
//    
//    View.OnClickListern listener = new View.OnClickListener(){
//        
//        public void onClick(){
//            System.out.println("hello!");
//            System.out.println(number);
//        }
//        
//    }
//    
//    button.setOnClickListener(listener);
//    
//}

    /*
     * 在局部内部类的方法中(比如:show)如果调用局部内部类所声明的方法(比如：method)中的局部变量(比如：num)的话,
     * 要求此局部变量声明为final的。
     * 
     * jdk 7及之前版本：要求此局部变量显式的声明为final的
     * jdk 8及之后的版本：可以省略final的声明
     * 
     */
    public void method(){
        //局部变量
        int num = 10;
        
        class AA{
            
            public void show(){
//                num = 20;    //Local variable num defined in an enclosing scope must be final or effectively final
                System.out.println(num);
            }
        }
    }
}
```

## 九：常用类

#### 文章目录

•01、字符串相关的类••1.1、String类的概述•1.2、理解String的不可变性•1.3、String不同实例化方式的对比•1.4、String不同拼接操作的对比••1.4.1、String使用陷阱•1.5、String的一道面试题•1.6、JVM中涉及字符串的内存结构•1.7、String的常用方法1•1.8、String的常用方法2•1.9、String的常用方法3•1.10、String与基本数据类型包装类的转换•1.11、String与char[]之间的转换•1.12、String与byte[]之间的转换•1.13、面试中String算法考查的说明•1.14、StringBuffer和StringBuilder的介绍•1.15、StringBuffer的源码分析•1.16、StringBuffer中的常用方法•1.17、String、StringBuffer、StringBuilder效率对比•02、JDK 8之前的日期时间API••2.1、System类中获取时间戳的方法•2.2、Java中两个Date类的使用•03、JDK 8之前的日期时间API••3.1、SimpleDateFormat的使用•3.2、SimpleDateFormat的练习•3.3、Calendar日历类的使用•04、JDK8中日期时间API的介绍••4.1、LocalDate、LocalTime、LocalDateTime的使用•4.2、Instant类的使用•4.3、DateTimeFormatter的使用•4.4、其它日期时间相关API的使用••4.4.1、参考：与传统日期处理的转换•05、Java比较器••5.1、概述•5.2、Comparable自然排序举例•5.3、自定义类实现Comparable自然排序•5.4、使用Comparator实现定制排序•06、System类、Math类、BigInteger与BigDecimal••6.1、System类•6.2、Math类•6.3、BigInteger与BigDecimal•其他

## 01、字符串相关的类

### 1.1、String类的概述

```java
import org.junit.Test;

/**
 * String的使用
 */
public class StringTest {

    /**
     * String:字符串，使用一对“”引起来表示。
     * 1.String声明为final的，不可被继承
     * 2.String实现了Serializable接口：表示字符串是支持序列化的。
     *         实现了Comparable接口：表示String可以比较大小
     * 3.String内部定义了final char[] value用于存储字符串数据
     * 4.String:代表不可变的字符序列。简称：不可变性。
     *      体现：
     *
     */
    @Test
    public void Test1(){

    }
}
```

### 1.2、理解String的不可变性

```java
import org.junit.Test;

/**
 * String的使用
 */
public class StringTest {

    /**
     * String:字符串，使用一对“”引起来表示。
     * 1.String声明为final的，不可被继承
     * 2.String实现了Serializable接口：表示字符串是支持序列化的。
     *         实现了Comparable接口：表示String可以比较大小
     * 3.String内部定义了final char[] value用于存储字符串数据
     * 4.String:代表不可变的字符序列。简称：不可变性。
     *      体现：1.当对字符串重新赋值时，需要重写指定内存区域赋值，不能使用原有的value进行赋值。
     *           2.当对现有的字符串进行连接操作时，也需要重新指定内存区域赋值，不能使用原有的value进行赋值。
     *           3.当调用String的replace()方法修改指定字符或字符串时，也需要重新指定内存区域赋值，不能使用原有的value进行赋值。
     * 5.通过字面量的方式（区别于new）给一个字符串赋值，此时的字符串值声明在字符串常量池中。
     * 6.字符串常量池中是不会存储相同内容的字符串的。
     *
     */
    @Test
    public void Test1(){
        String s1 = "abc";  //字面量的定义方式
        String s2 = "abc";
        s1 = "hello";

        System.out.println(s1 == s2);//比较s1和s2的地址值

        System.out.println(s1);//hello
        System.out.println(s2);//abc

        System.out.println("*********************");

        String s3 = "abc";
        s3 += "def";
        System.out.println(s3);//abcdef

        System.out.println("**********************");

        String s4 = "abc";
        String s5 = s4.replace('a', 'm');
        System.out.println(s4);//abc
        System.out.println(s5);//mbc
    }
}
```

![null](https://i-blog.csdnimg.cn/blog_migrate/62abcf32902e51e42a33e875351541e9.png#pic_center)

### 1.3、String不同实例化方式的对比

> 1、String对象的创建

```java
String str = "hello";

//本质上this.value = new char[0];
String  s1 = new String(); 

//this.value = original.value;
String  s2 = new String(String original); 

//this.value = Arrays.copyOf(value, value.length);
String  s3 = new String(char[] a);

String  s4 = new String(char[] a,int startIndex,int count);
```

![null](https://i-blog.csdnimg.cn/blog_migrate/9264e5f985c15b2579891b0bcbf0d21c.png#pic_center)



![null](https://i-blog.csdnimg.cn/blog_migrate/f3f8474dc11dbf668bc84fdf763dd4ae.png#pic_center)

> **2、String str1 = “abc”;与String str2 = new String(“abc”);的区别？**

•字符串常量存储在字符串常量池，目的是共享•字符串非常量对象存储在堆中。

![null](https://i-blog.csdnimg.cn/blog_migrate/0498e74451a80abb2dd302084b6aab5a.png#pic_center)

> 3、**练习**

![null](https://i-blog.csdnimg.cn/blog_migrate/d2c7781d2afeebb088e862fb407b2406.png#pic_center)

```java
import org.junit.Test;

/**
 * String的使用
 */
public class StringTest {

    /**
     * String的实例化方式
     * 方式一：通过字面量定义的方式
     * 方式二：通过new + 构造器的方式
     *
     * 面试题：String s = new String("abc");方式创建对象，在内存中创建了几个对象？
     *      两个:一个是堆空间中new结构，另一个是char[]对应的常量池中的数据："abc"
     *
     */
    @Test
    public void test2(){
        //通过字面量定义的方式：此时的s1和s2的数据javaEE声明在方法区中的字符串常量池中。
        String s1 = "javaEE";
        String s2 = "javaEE";

        //通过new + 构造器的方式:此时的s3和s4保存的地址值，是数据在堆空间中开辟空间以后对应的地址值。
        String s3 = new String("javaEE");
        String s4 = new String("javaEE");

        System.out.println(s1 == s2);//true
        System.out.println(s1 == s3);//false
        System.out.println(s1 == s4);//false
        System.out.println(s3 == s4);//false

        System.out.println("***********************");
        Person p1 = new Person("Tom",12);
        Person p2 = new Person("Tom",12);

        System.out.println(p1.name.equals(p2.name));//true
        System.out.println(p1.name == p2.name);//true

        p1.name = "Jerry";
        System.out.println(p2.name);//Tom
    }
}
```

> Person类

```java
/**
 * @author subei
 * @create 2020-05-09 11:20
 */
public class Person {

    String name;
    int age;

    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public Person() {

    }
}
```

![null](https://i-blog.csdnimg.cn/blog_migrate/5d6c8d68d6973efe0ae624a6d9f1e6b4.png#pic_center)

### 1.4、String不同拼接操作的对比

```java
import org.junit.Test;

/**
 * String的使用
 */
public class StringTest {

    /**
     * 结论
     *     1.常量与常量的拼接结果在常量池。且常量池中不会存在相同内容的常量。
     *     2.只要其中有一个是变量，结果就在堆中
     *     3.如果拼接的结果调用intern()方法，返回值就在常量池中
     *
     */
    @Test
    public void test4(){
        String s1 = "javaEEhadoop";
        String s2 = "javaEE";
        String s3 = s2 + "hadoop";
        System.out.println(s1 == s3);//false

        final String s4 = "javaEE";//s4:常量
        String s5 = s4 + "hadoop";
        System.out.println(s1 == s5);//true

    }

    @Test
    public void test3(){
        String s1 = "javaEE";
        String s2 = "hadoop";

        String s3 = "javaEEhadoop";
        String s4 = "javaEE" + "hadoop";
        String s5 = s1 + "hadoop";
        String s6 = "javaEE" + s2;
        String s7 = s1 + s2;

        System.out.println(s3 == s4);//true
        System.out.println(s3 == s5);//false
        System.out.println(s3 == s6);//false
        System.out.println(s5 == s6);//false
        System.out.println(s3 == s7);//false
        System.out.println(s5 == s6);//false
        System.out.println(s5 == s7);//false
        System.out.println(s6 == s7);//false

        String s8 = s5.intern();//返回值得到的s8使用的常量值中已经存在的“javaEEhadoop”
        System.out.println(s3 == s8);//true
    }
}
```

#### 1.4.1、String使用陷阱

> 1、`String s1 = “a”;`

说明：在字符串常量池中创建了一个字面量为"a"的字符串。

> 2、`s1 = s1 + “b”;`

说明：实际上原来的“a”字符串对象已经丢弃了，现在在堆空间中产生了一个字符串s1+“b”（也就是"ab")。如果多次执行这些改变串内容的操作，会导致大量副本字符串对象存留在内存中，降低效率。如果这样的操作放到循环中，会极大影响程序的性能。

> 3、`String s2 = “ab”;`

说明：直接在字符串常量池中创建一个字面量为"ab"的字符串。

> 4、`String s3 = “a” + “b”;`

说明：s3指向字符串常量池中已经创建的"ab"的字符串。

> 5、`String s4 = s1.intern();`

说明：堆空间的s1对象在调用intern()之后，会将常量池中已经存在的"ab"字符串赋值给s4。

> 6、练习

![null](https://i-blog.csdnimg.cn/blog_migrate/cd65271f0f5633573d9d7a8277cb31c2.png#pic_center)

### 1.5、String的一道面试题

```java
/**
 * 一道面试题
 */
public class StringTest {
    String str = new String("good");
    char[] ch = { 't', 'e', 's', 't' };

    public void change(String str, char ch[]) {
        str = "test ok";
        ch[0] = 'b';
    }
    public static void main(String[] args) {
        StringTest ex = new StringTest();
        ex.change(ex.str, ex.ch);
        System.out.println(ex.str);//good
        System.out.println(ex.ch);//best
    }
}
```

### 1.6、JVM中涉及字符串的内存结构

![null](https://i-blog.csdnimg.cn/blog_migrate/b3e6b8ce029d87b1670c48a0f8128c11.png)



![null](https://i-blog.csdnimg.cn/blog_migrate/557d00ea041260a93d7ba9cf490e0728.png)



![null](https://i-blog.csdnimg.cn/blog_migrate/625bba8c6e4b344c71c1f59f6445be08.png)



![null](https://i-blog.csdnimg.cn/blog_migrate/9476fb3e7a7b3e572a8ef28cbd534719.png)



![null](https://i-blog.csdnimg.cn/blog_migrate/259625a732c61b52afa2ad71de24d2d8.png)



![null](https://i-blog.csdnimg.cn/blog_migrate/0fa858c735b74d8a003366ae2f3266cc.png)



![null](https://i-blog.csdnimg.cn/blog_migrate/f18024321917a0c312d6cdc9c8bed45b.png)



![null](https://i-blog.csdnimg.cn/blog_migrate/7add21dfdc28ea5f5cbe49f316fb9215.png)



![null](https://i-blog.csdnimg.cn/blog_migrate/b885576556023737bdcd2322e608556b.png#pic_center)



![null](https://i-blog.csdnimg.cn/blog_migrate/06248138a654aa7bcfd2bd694ae65abc.png)



![null](https://i-blog.csdnimg.cn/blog_migrate/39f0e773511a917823b3bdcb92413171.png)



![null](https://i-blog.csdnimg.cn/blog_migrate/6a0c206319b79a3b4639cc153e4453dd.png)

### 1.7、String的常用方法1

```java
import org.junit.Test;

public class StringMethodTest {

    /**
     * int length()：返回字符串的长度：return value.length
     * char charAt(int index)：返回某索引处的字符return value[index]
     * boolean isEmpty()：判断是否是空字符串：return value.length==0
     * String toLowerCase()：使用默认语言环境，将String中的所有字符转换为小写
     * String toUpperCase()：使用默认语言环境，将String中的所有字符转换为大写
     * String trim()：返回字符串的副本，忽略前导空白和尾部空白
     * boolean equals(Object obj)：比较字符串的内容是否相同
     * boolean equals IgnoreCase(String anotherString)：与equals方法类似，忽略大小写
     * String concat(String str)：将指定字符串连接到此字符串的结尾。等价于用“+”
     * int compareTo(String anotherString)：比较两个字符串的大小
     * String substring(int beginIndex)：返回一个新的字符串，它是此字符串的从beginIndex开始截取到最后的一个子字符串。
     * String substring(int beginIndex,int endIndex)：返回一个新字符串，它是此字符串从beginIndex开始截取到endIndex(不包含)的一个子字符串。
     */
    @Test
    public void test2(){
        String s1 = "HelloWorld";
        String s2 = "helloworld";
        System.out.println(s1.equals(s2));//false
        System.out.println(s1.equalsIgnoreCase(s2));//true
        
        String s3 = "abc";
        String s4 = s3.concat("def");
        System.out.println(s4);//abcdef

        String s5 = "abc";
        String s6 = new String("abe");
        System.out.println(s5.compareTo(s6));//-2   //涉及到字符串的排序

        String s7 = "周围好吵啊";
        String s8 = s7.substring(2);
        System.out.println(s7);
        System.out.println(s8);

        String s9 = s7.substring(0, 2);
        System.out.println(s9);
    }

    @Test
    public void Test1(){
        String s1 = "helloworld";
        System.out.println(s1.length());
        System.out.println(s1.length());
        System.out.println(s1.charAt(0));
        System.out.println(s1.charAt(9));
//        System.out.println(s1.charAt(10));
//        s1 = "";
        System.out.println(s1.isEmpty());

        String s2 = s1.toLowerCase();
        System.out.println(s1);//s1不可变的，仍然为原来的字符串
        System.out.println(s2);//改成小写以后的字符串

        String s3 = "   he  llo   world   ";
        String s4 = s3.trim();
        System.out.println("-----" + s3 + "-----");
        System.out.println("-----" + s4 + "-----");
    }

}
```

### 1.8、String的常用方法2

```java
import org.junit.Test;

public class StringMethodTest {

    /**
     * boolean endsWith(String suffix)：测试此字符串是否以指定的后缀结束
     * boolean startsWith(String prefix)：测试此字符串是否以指定的前缀开始
     * boolean startsWith(String prefix, int toffset)：测试此字符串从指定索引开始的子字符串是否以指定前缀开始
     *
     * boolean contains(CharSequence s)：当且仅当此字符串包含指定的 char 值序列时，返回 true
     * int indexOf(String str)：返回指定子字符串在此字符串中第一次出现处的索引
     * int indexOf(String str, int fromIndex)：返回指定子字符串在此字符串中第一次出现处的索引，从指定的索引开始
     * int lastIndexOf(String str)：返回指定子字符串在此字符串中最右边出现处的索引
     * int lastIndexOf(String str, int fromIndex)：返回指定子字符串在此字符串中最后一次出现处的索引，从指定的索引开始反向搜索
     *
     * 注：indexOf和lastIndexOf方法如果未找到都是返回-1
     */
    @Test
    public void test3(){
        String str1 = "helloworld";
        boolean b1 = str1.endsWith("rld");
        System.out.println(b1);

        boolean b2 = str1.startsWith("He");
        System.out.println(b2);

        boolean b3 = str1.startsWith("ll",2);
        System.out.println(b3);

        String str2 = "wor";
        System.out.println(str1.contains(str2));

        System.out.println(str1.indexOf("lo"));

        System.out.println(str1.indexOf("lo",5));

        String str3 = "hellorworld";

        System.out.println(str3.lastIndexOf("or"));
        System.out.println(str3.lastIndexOf("or",6));

        //什么情况下，indexOf(str)和lastIndexOf(str)返回值相同？
        //情况一：存在唯一的一个str。情况二：不存在str
    }
}
```

### 1.9、String的常用方法3

```java
import org.junit.Test;

public class StringMethodTest {

    /**
     * 替换：
     * String replace(char oldChar, char newChar)：返回一个新的字符串，它是通过用 newChar 替换此字符串中出现的所有 oldChar 得到的。
     * String replace(CharSequence target, CharSequence replacement)：使用指定的字面值替换序列替换此字符串所有匹配字面值目标序列的子字符串。
     * String replaceAll(String regex, String replacement)：使用给定的 replacement 替换此字符串所有匹配给定的正则表达式的子字符串。
     * String replaceFirst(String regex, String replacement)：使用给定的 replacement 替换此字符串匹配给定的正则表达式的第一个子字符串。
     *
     * 匹配:
     * boolean matches(String regex)：告知此字符串是否匹配给定的正则表达式。
     *
     * 切片：
     * String[] split(String regex)：根据给定正则表达式的匹配拆分此字符串。
     * String[] split(String regex, int limit)：根据匹配给定的正则表达式来拆分此字符串，最多不超过limit个，如果超过了，剩下的全部都放到最后一个元素中。
     *
     */
    @Test
    public void test4(){
        String str1 = "西藏布达拉宫欢迎您";
        String str2 = str1.replace('西','东');

        System.out.println(str1);
        System.out.println(str2);

        String str3 = str1.replace("北京", "南京");
        System.out.println(str3);

        System.out.println("*************************");
        String str = "12hello34world5java7891mysql456";
        //把字符串中的数字替换成,，如果结果中开头和结尾有，的话去掉
        String string = str.replaceAll("\\d+", ",").replaceAll("^,|,$", "");
        System.out.println(string);

        System.out.println("*************************");
        str = "12345";
        //判断str字符串中是否全部有数字组成，即有1-n个数字组成
        boolean matches = str.matches("\\d+");
        System.out.println(matches);
        String tel = "0571-4534289";
        //判断这是否是一个杭州的固定电话
        boolean result = tel.matches("0571-\\d{7,8}");
        System.out.println(result);

        System.out.println("*************************");
        str = "hello|world|java";
        String[] strs = str.split("\\|");
        for (int i = 0; i < strs.length; i++) {
            System.out.println(strs[i]);
        }
        System.out.println();
        str2 = "hello.world.java";
        String[] strs2 = str2.split("\\.");
        for (int i = 0; i < strs2.length; i++) {
            System.out.println(strs2[i]);
        }
    }
}
```

### 1.10、String与基本数据类型包装类的转换

```java
import org.junit.Test;

/**
 * 涉及到String类与其他结构之间的转换
 */
public class StringTest1 {

    /**
     * 复习
     *    String与基本数据类型、包装类之间的转换
     *
     *    String --> 基本数据类型、包装类：调用包装类的静态方法：parseXxx(str)
     *    基本数据类型、包装类 --> String:调用String重载的valueOf(xxx)
     */
    @Test
    public void test1(){
        String str1 = "123";
//        int num = (int)str1;//错误的
        int num = Integer.parseInt(str1);

        String str2 = String.valueOf(num);   //"123
        String str3 = num + "";

        System.out.println(str1 == str3);   //false
    }

}
```

### 1.11、String与char[]之间的转换

```java
import org.junit.Test;

/**
 * 涉及到String类与其他结构之间的转换
 */
public class StringTest1 {

    /**
     * String 与 char[]之间的转换
     *
     * String --> char[]:调用String的toCharArray()
     * char[] --> String:调用String的构造器
     */
    @Test
    public void test2(){
        String str1 = "abc123"; //题目： a21cb3

        char[] charArray = str1.toCharArray();
        for (int i = 0; i < charArray.length; i++) {
            System.out.println(charArray[i]);
        }

        char[] arr = new char[]{'h','e','l','l','o'};
        String str2 = new String(arr);
        System.out.println(str2);
    }
}
```

### 1.12、String与byte[]之间的转换

```java
import org.junit.Test;

import java.io.UnsupportedEncodingException;
import java.util.Arrays;

/**
 * 涉及到String类与其他结构之间的转换
 */
public class StringTest1 {

    /**
     * String 与 byte[]之间的转换
     *
     * 编码：String --> byte[]:调用String的getBytes()
     * 解码：byte[] --> String:调用String的构造器
     *
     * 编码：字符串 -->字节  (看得懂 --->看不懂的二进制数据)
     * 解码：编码的逆过程，字节 --> 字符串 （看不懂的二进制数据 ---> 看得懂）
     *
     * 说明：解码时，要求解码使用的字符集必须与编码时使用的字符集一致，否则会出现乱码。
     *
     */
    @Test
    public void test3() throws UnsupportedEncodingException {
        String str1 = "abc123重工";
        byte[] bytes = str1.getBytes();//使用默认的字符编码集,进行转换
        System.out.println(Arrays.toString(bytes));

        byte[] gbks = str1.getBytes("gbk");//使用gbk字符集进行编码。
        System.out.println(Arrays.toString(gbks));

        System.out.println("*****************************");

        String str2 = new String(bytes);//使用默认的字符集，进行解码。
        System.out.println(str2);

        String str3 = new String(gbks);
        System.out.println(str3);//出现乱码。原因：编码集和解码集不一致！

        String str4 = new String(gbks,"gbk");
        System.out.println(str4);//没有出现乱码。原因：编码集和解码集一致！
    }
}
```

### 1.13、面试中String算法考查的说明

> 1、模拟一个trim方法，去除字符串两端的空格。

```java
import org.junit.Test;

/*
 * 1.模拟一个trim方法，去除字符串两端的空格。
 * 
 */
public class StringExer {

    // 第1题
    public String myTrim(String str) {
        if (str != null) {
            int start = 0;// 用于记录从前往后首次索引位置不是空格的位置的索引
            int end = str.length() - 1;// 用于记录从后往前首次索引位置不是空格的位置的索引

            while (start < end && str.charAt(start) == ' ') {
                start++;
            }

            while (start < end && str.charAt(end) == ' ') {
                end--;
            }
            if (str.charAt(start) == ' ') {
                return "";
            }

            return str.substring(start, end + 1);
        }
        return null;
    }
    
    @Test
    public void testMyTrim() {
        String str = "   a   ";
        // str = " ";
        String newStr = myTrim(str);
        System.out.println("---" + newStr + "---");
    }
}
```

> 2、将一个字符串进行反转。将字符串中指定部分进行反转。比如“abcdefg”反转为”abfedcg”

```java
import org.junit.Test;

public class StringDemo {

    /**
     * 将一个字符串进行反转。将字符串中指定部分进行反转。比如“abcdefg”反转为”abfedcg”
     *
     * 方式一：转换为char[]
     */
    public String reverse(String str,int startIndex,int endIndex){

        if(str != null && str.length() != 0) {
            char[] arr = str.toCharArray();
            for (int x = startIndex, y = endIndex; x < y; x++, y--) {
                char temp = arr[x];
                arr[x] = arr[y];
                arr[y] = temp;
            }
            return new String(arr);
        }
        return null;
    }

    /**
     * 方式二：使用String的拼接
     */
    public String reverse2(String str, int startIndex, int endIndex) {
        if(str != null) {
            // 第一部分
            String reverStr = str.substring(0,startIndex);// ab
            // 第二部分
            for (int i = endIndex; i >= startIndex; i--) {
                reverStr += str.charAt(i);
            } // abfedc
            // 第三部分
            reverStr += str.substring(endIndex + 1);

            return reverStr;
        }
        return null;
    }

    //方式三：使用StringBuffer/StringBuilder替换String
    public String reverse3(String str, int startIndex, int endIndex) {
        StringBuilder builder = new StringBuilder(str.length());

        if(str != null) {
            //第一部分
            builder.append(str.substring(0, startIndex));

            //第二部分
            for (int i = endIndex; i >= startIndex; i--) {

                builder.append(str.charAt(i));
            }
            //第三部分
            builder.append(str.substring(endIndex + 1));

            return builder.toString();
        }
        return null;
    }

    @Test
    public void testReverse() {
        String str = "abcdefg";
        String str1 = reverse3(str, 2, 5);
        System.out.println(str1);// abfedcg

    }
}
```

> 3、获取一个字符串在另一个字符串中出现的次数。比如：获取“ ab”在“abkkcadkabkebfkabkskab” 中出现的次数

```java
import org.junit.Test;

public class StringDemo2 {
    /**
     * 获取一个字符串在另一个字符串中出现的次数。
     * 比如：获取“ ab”在“abkkcadkabkebfkabkskab” 中出现的次数
     *
     */

    /**
     * 获取subStr在mainStr中出现的次数
     * @param mainStr
     * @param subStr
     */
    public int getCount(String mainStr,String subStr){
        int mainLength = mainStr.length();
        int subLength = subStr.length();
        int count = 0;
        int index = 0;

        if(mainLength >= subLength){

            //方式一：
//            while((index = mainStr.indexOf(subStr)) != -1){
//                count++;
//                mainStr = mainStr.substring(index + subStr.length());
//            }
            //方式二：对方式一的改进
            while((index = mainStr.indexOf(subStr,index)) != -1){
                count++;
                index += subLength;
            }

            return count;
        }else{
            return 0;
        }
    }

    @Test
    public void testGetCount(){
        String mainStr = "abkkcadkabkebfkabkskab";
        String subStr = "ab";
        int count = getCount(mainStr,subStr);
        System.out.println(count);
    }

}
```

> 4、获取两个字符串中最大相同子串。比如：
>
> ```
> str1 = "abcwerthelloyuiodef“;str2 = “cvhellobnm”
> ```
>
> 提示：将短的那个串进行长度依次递减的子串与较长的串比较。

```java
import org.junit.Test;

import java.util.Arrays;

public class StringDemo3 {
    /**
     * 获取两个字符串中最大相同子串。比如：
     * str1 = "abcwerthelloyuiodef“;str2 = "cvhellobnm"
     * 提示：将短的那个串进行长度依次递减的子串与较长的串比较。
     */
    //前提：两个字符串中只有一个最大相同子串
    public String getMaxSameString(String str1,String str2){
        if(str1 != null && str2 != null){
            String maxStr = (str1.length() >= str2.length())? str1 : str2;
            String minStr = (str1.length() < str2.length())? str1 : str2;
            int length = minStr.length();

            for(int i = 0;i < length;i++){
                for(int x = 0,y = length - i;y <= length;x++,y++){
                    String subStr = minStr.substring(x,y);
                    if(maxStr.contains(subStr)){
                        return subStr;
                    }

                }
            }

        }
        return null;
    }

    // 如果存在多个长度相同的最大相同子串
    // 此时先返回String[]，后面可以用集合中的ArrayList替换，较方便
    public String[] getMaxSameString1(String str1, String str2) {
        if (str1 != null && str2 != null) {
            StringBuffer sBuffer = new StringBuffer();
            String maxString = (str1.length() > str2.length()) ? str1 : str2;
            String minString = (str1.length() > str2.length()) ? str2 : str1;

            int len = minString.length();
            for (int i = 0; i < len; i++) {
                for (int x = 0, y = len - i; y <= len; x++, y++) {
                    String subString = minString.substring(x, y);
                    if (maxString.contains(subString)) {
                        sBuffer.append(subString + ",");
                    }
                }
//                System.out.println(sBuffer);
                if (sBuffer.length() != 0) {
                    break;
                }
            }
            String[] split = sBuffer.toString().replaceAll(",$", "").split("\\,");
            return split;
        }

        return null;
    }

    @Test
    public void testGetMaxSameString(){
        String str1 = "abcwerthello1yuiodefabcdef";
        String str2 = "cvhello1bnmabcdef";
        String[] maxSameStrings = getMaxSameString1(str1, str2);
        System.out.println(Arrays.toString(maxSameStrings));

    }

}
```

> 5、对字符串中字符进行自然顺序排序。
>
> 提示：
>
> 1）字符串变成字符数组。
>
> 2）对数组排序，选择，冒泡，Arrays.sort();
>
> 3）将排序后的数组变成字符串。

```java
import org.junit.Test;
import java.util.Arrays;

/**
 *
 * 5.对字符串中字符进行自然顺序排序。"abcwerthelloyuiodef"
 * 提示：
 *         1）字符串变成字符数组。
 *         2）对数组排序，选择，冒泡，Arrays.sort(str.toCharArray());
 *         3）将排序后的数组变成字符串。
 *
 */

public class StringDemo4 {

    // 第5题
    @Test
    public void testSort() {
        String str = "abcwerthelloyuiodef";
        char[] arr = str.toCharArray();
        Arrays.sort(arr);

        String newStr = new String(arr);
        System.out.println(newStr);
    }
}
```

### 1.14、StringBuffer和StringBuilder的介绍

```java
/**
 * String、StringBuffer、StringBuilder三者的异同？
 *
 * String:不可变的字符序列；底层使用char[]存储
 * StringBuffer:可变的字符序列；线程安全的，效率低；底层使用char[]存储
 * StringBuilder:可变的字符序列；jdk5.0新增的，线程不安全的，效率高；底层使用char[]存储
 *
 */
```

### 1.15、StringBuffer的源码分析

```java
import org.junit.Test;

/**
 * 关于StringBuffer和StringBuilder的使用
 */
public class StringBufferBuilderTest {
    /**
     *
     * 源码分析：
     * String str = new String();//char[] value = new char[0];
     * String str1 = new String("abc");//char[] value = new char[]{'a','b','c'};
     *
     * StringBuffer sb1 = new StringBuffer();//char[] value = new char[16];底层创建了一个长度是16的数组。
     * System.out.println(sb1.length());//
     * sb1.append('a');//value[0] = 'a';
     * sb1.append('b');//value[1] = 'b';
     *
     * StringBuffer sb2 = new StringBuffer("abc");//char[] value = new char["abc".length() + 16];
     *
     * //问题1.System.out.println(sb2.length());//3
     * //问题2.扩容问题:如果要添加的数据底层数组盛不下了，那就需要扩容底层的数组。
     *        默认情况下，扩容为原来容量的2倍 + 2，同时将原有数组中的元素复制到新的数组中。
     *
     * 意义：开发中建议大家使用：StringBuffer(int capacity) 或 StringBuilder(int capacity)
     *
     */
    @Test
    public void test1(){
        StringBuffer sb1 = new StringBuffer("abc");
        sb1.setCharAt(0,'m');
        System.out.println(sb1);

        StringBuffer sb2 = new StringBuffer();
        System.out.println(sb2.length());   //0
    }
}
```

### 1.16、StringBuffer中的常用方法

```java
import org.junit.Test;

/**
 * 关于StringBuffer和StringBuilder的使用
 */
public class StringBufferBuilderTest {

    /**
     * StringBuffer的常用方法：
     *
     * StringBuffer append(xxx)：提供了很多的append()方法，用于进行字符串拼接
     * StringBuffer delete(int start,int end)：删除指定位置的内容
     * StringBuffer replace(int start, int end, String str)：把[start,end)位置替换为str
     * StringBuffer insert(int offset, xxx)：在指定位置插入xxx
     * StringBuffer reverse() ：把当前字符序列逆转
     * public int indexOf(String str)
     * public String substring(int start,int end):返回一个从start开始到end索引结束的左闭右开区间的子字符串
     * public int length()
     * public char charAt(int n )
     * public void setCharAt(int n ,char ch)
     *
     * 总结：
     *     增：append(xxx)
     *     删：delete(int start,int end)
     *     改：setCharAt(int n ,char ch) / replace(int start, int end, String str)
     *     查：charAt(int n )
     *     插：insert(int offset, xxx)
     *     长度：length();
     *     遍历：for() + charAt() / toString()
     *
     */
    @Test
    public void test2(){
        StringBuffer s1 = new StringBuffer("abc");
        s1.append(1);
        s1.append('1');
        System.out.println(s1);
//        s1.delete(2,4);
//        s1.replace(2,4,"hello");
//        s1.insert(2,false);
//        s1.reverse();
        String s2 = s1.substring(1,3);
        System.out.println(s1);
        System.out.println(s1.length());
        System.out.println(s2);
    }
}
```

### 1.17、String、StringBuffer、StringBuilder效率对比

```java
import org.junit.Test;

/**
 * 关于StringBuffer和StringBuilder的使用
 */
public class StringBufferBuilderTest {

    /**
     * 对比String、StringBuffer、StringBuilder三者的效率：
     * 从高到低排列：StringBuilder > StringBuffer > String
     *
     */
    @Test
    public void test3(){
        //初始设置
        long startTime = 0L;
        long endTime = 0L;
        String text = "";
        StringBuffer buffer = new StringBuffer("");
        StringBuilder builder = new StringBuilder("");
        //开始对比
        startTime = System.currentTimeMillis();
        for (int i = 0; i < 20000; i++) {
            buffer.append(String.valueOf(i));
        }
        endTime = System.currentTimeMillis();
        System.out.println("StringBuffer的执行时间：" + (endTime - startTime));

        startTime = System.currentTimeMillis();
        for (int i = 0; i < 20000; i++) {
            builder.append(String.valueOf(i));
        }
        endTime = System.currentTimeMillis();
        System.out.println("StringBuilder的执行时间：" + (endTime - startTime));

        startTime = System.currentTimeMillis();
        for (int i = 0; i < 20000; i++) {
            text = text + i;
        }
        endTime = System.currentTimeMillis();
        System.out.println("String的执行时间：" + (endTime - startTime));

    }
}
```

## 02、JDK 8之前的日期时间API

![null](https://i-blog.csdnimg.cn/blog_migrate/737757d57881d3ede6f48a88bc82fbc4.png)

### 2.1、System类中获取时间戳的方法

> `System`类提供的`public static long currentTimeMillis()`用来返回**当前时间与1970年1月1日0时0分0秒之间以毫秒为单位的时间差。**

•此方法适于计算时间差。•计算世界时间的主要标准有：•UTC(Coordinated Universal Time)•GMT(Greenwich Mean Time)•CST(Central Standard Time)

```java
import org.junit.Test;

/**
 * JDK 8之前日期和时间的API测试
 */
public class DateTimeTest {

    //1.System类中的currentTimeMillis()
    @Test
    public void test1(){
        long time = System.currentTimeMillis();
        //返回当前时间与1970年1月1日0时0分0秒之间以毫秒为单位的时间差。
        //称为时间戳
        System.out.println(time);
    }
}
```

### 2.2、Java中两个Date类的使用

```java
import org.junit.Test;

import java.util.Date;

/**
 * JDK 8之前日期和时间的API测试
 */
public class DateTimeTest {

    /**
     * java.util.Date类 ---> 表示特定的瞬间，精确到毫秒
     *            |---java.sql.Date类
     *
     * 1.两个构造器的使用
     *     >构造器一：Date()：创建一个对应当前时间的Date对象
     *     >构造器二：创建指定毫秒数的Date对象
     * 2.两个方法的使用
     *     >toString():显示当前的年、月、日、时、分、秒
     *     >getTime():获取当前Date对象对应的毫秒数。（时间戳）
     *
     * 3. java.sql.Date对应着数据库中的日期类型的变量
     *     >如何实例化
     *     >如何将java.util.Date对象转换为java.sql.Date对象
     *
     */
    @Test
    public void test2(){
        //构造器一：Date()：创建一个对应当前时间的Date对象
        Date date1 = new Date();
        System.out.println(date1.toString());   //Sat May 09 20:09:11 CST 2020

        System.out.println(date1.getTime());    //1589026216998

        //构造器二：创建指定毫秒数的Date对象
        Date date2 = new Date(1589026216998L);
        System.out.println(date2.toString());

        //创建java.sql.Date对象
        java.sql.Date date3 = new java.sql.Date(35235325345L);
        System.out.println(date3);  //1971-02-13

        //如何将java.util.Date对象转换为java.sql.Date对象
        //情况一：
//        Date date4 = new java.sql.Date(2343243242323L);
//        java.sql.Date date5 = (java.sql.Date) date4;
        //情况二：
        Date date6 = new Date();
        java.sql.Date date7 = new java.sql.Date(date6.getTime());
    }
}
```

## 03、JDK 8之前的日期时间API

### 3.1、SimpleDateFormat的使用

•`Date`类的API不易于国际化，大部分被废弃了，`java.text.SimpleDateFormat`类是一个不与语言环境有关的方式来格式化和解析日期的具体类。•它允许进行•格式化：日期—>文本•解析：文本—>日期

```java
import org.junit.Test;

import java.text.ParseException;
import java.text.SimpleDateFormat;
import java.util.Date;

/**
 * jdk 8 之前的日期时间的API测试
 * 1.System类中currentTimeMillis();
 * 2.java.util.Date和字类java.sql.Date
 * 3.SimpleDateFormat
 * 4.Calendar
 */
public class DateTime {
    /**
     * SimpleDateFormat的使用：SimpleDateFormat对日期Date类的格式化和解析
     * 1.两个操作
     * 1.1格式化：日期---》字符串
     * 1.2解析：格式化的逆过程，字符串---》日期
     *
     * 2.SimpleDateFormat的实例化
     */
    @Test
    public void testSimpleDateFormat() throws ParseException {
        //实例化SimpleDateFormat
        SimpleDateFormat sdf = new SimpleDateFormat();

        //格式化：日期---》字符串
        Date date = new Date();
        System.out.println(date);   //Sun May 10 16:34:30 CST 2020

        String format = sdf.format(date);
        System.out.println(format); //20-5-10 下午4:34

        //解析：格式化的逆过程，字符串---》日期
        String str = "19-12-18 上午11:43";
        Date date1 = sdf.parse(str);
        System.out.println(date1);  //Wed Dec 18 11:43:00 CST 2019

        //*************按照指定的方式格式化和解析：调用带参的构造器*****************
//        SimpleDateFormat sdf1 = new SimpleDateFormat("yyyyy.MMMMM.dd GGG hh:mm aaa");
        SimpleDateFormat sdf1 = new SimpleDateFormat("yyyyy.MMMMM.dd GGG hh:mm aaa");
        //格式化
        String format1 = sdf1.format(date);
        System.out.println(format1);    //02020.五月.10 公元 04:32 下午
        //解析:要求字符串必须是符合SimpleDateFormat识别的格式(通过构造器参数体现),
        //否则，抛异常
        Date date2 = sdf1.parse("02020.五月.10 公元 04:32 下午");
        System.out.println(date2);  //Sun May 10 16:32:00 CST 2020
    }
}
```

### 3.2、SimpleDateFormat的练习

> 1、练习1

```java
import org.junit.Test;

import java.text.ParseException;
import java.text.SimpleDateFormat;
import java.util.Date;

/**
 * jdk 8 之前的日期时间的API测试
 * 1.System类中currentTimeMillis();
 * 2.java.util.Date和字类java.sql.Date
 * 3.SimpleDateFormat
 * 4.Calendar
 */
public class DateTime {

    /**
     * 练习1：字符串"2020-09-08"转换为java.sql.Date
     *
     */
    @Test
    public void testExer() throws ParseException {
        String birth = "2020-09-08";

        SimpleDateFormat sdf1 = new SimpleDateFormat("yyyy-MM-dd");
        Date date = sdf1.parse(birth);
//        System.out.println(date);

        java.sql.Date birthDate = new java.sql.Date(date.getTime());
        System.out.println(birthDate);
    }
}
```

> 2、练习2

```java
    /**
     * 练习二："三天打渔两天晒网"   1990-01-01  xxxx-xx-xx 打渔？晒网？
     *
     *     举例：2020-09-08 ？ 总天数
     *
     *     总天数 % 5 == 1,2,3 : 打渔
     *     总天数 % 5 == 4,0 : 晒网
     *
     *     总天数的计算？
     *     方式一：( date2.getTime() - date1.getTime()) / (1000 * 60 * 60 * 24) + 1
     *     方式二：1990-01-01  --> 2019-12-31  +  2020-01-01 -->2020-09-08
     *
     */
```

### 3.3、Calendar日历类的使用

•`Calendar`是一个抽象基类，主用用于完成日期字段之间相互操作的功能。•获取`Calendar`实例的方法•使用`Calendar.getInstance()`方法•调用它的子类`GregorianCalendar`的构造器。•一个Calendar的实例是系统时间的抽象表示，通过`get(intfield)`方法来取得想要的时间信息。比如`YEAR、MONTH、DAY_OF_WEEK、HOUR_OF_DAY 、MINUTE、SECOND`•`public void set(intfield,intvalue)`•`public void add(intfield,intamount)`•`public final Date getTime()`•`public final void setTime(Date date)`•注意:•获取月份时：一月是0，二月是1，以此类推，12月是11•获取星期时：周日是1，周二是2，。。。。周六是7

```java
import java.util.Calendar;
import java.util.Date;

import org.junit.Test;

/**
 * jdk 8 之前的日期时间的API测试
 * 1.System类中currentTimeMillis();
 * 2.java.util.Date和字类java.sql.Date
 * 3.SimpleDateFormat
 * 4.Calendar
 */
public class DateTime {

    /**
     * Calendar日历类的使用
     */
    @Test
    public void testCalendar(){
        //1.实例化
        //方式一：创建其子类（GregorianCalendar）的对象
        //方式二：调用其静态方法getInstance()
        Calendar calendar = Calendar.getInstance();

//        System.out.println(calendar.getClass());    //class java.util.GregorianCalendar

        //2.常用方法
        //get()
        int days = calendar.get(Calendar.DAY_OF_MONTH);
        System.out.println(days);   //10
        System.out.println(calendar.get(Calendar.DAY_OF_YEAR)); //131,今天是这一年的131天

        //set()
        //calendar可变性
        calendar.set(Calendar.DAY_OF_MONTH,22);
        days = calendar.get(Calendar.DAY_OF_MONTH);
        System.out.println(days);   //22

        //add()
        calendar.add(Calendar.DAY_OF_MONTH,-3);
        days = calendar.get(Calendar.DAY_OF_MONTH);
        System.out.println(days);   //22-3 --》19

        //getTime():日历类---> Date
        Date date = calendar.getTime();
        System.out.println(date);   //Tue May 19 17:12:06 CST 2020

        //setTime():Date ---> 日历类
        Date date1 = new Date();
        calendar.setTime(date1);
        days = calendar.get(Calendar.DAY_OF_MONTH);
        System.out.println(days);   //10
    }
}
```

## 04、JDK8中日期时间API的介绍

> 1、新日期时间API出现的背景

如果我们可以跟别人说：“我们在1502643933071见面，别晚了！”那么就再简单不过了。但是我们希望时间与昼夜和四季有关，于是事情就变复杂了。JDK 1.0中包含了一个java.util.Date类，但是它的大多数方法已经在JDK 1.1引入Calendar类之后被弃用了。而Calendar并不比Date好多少。它们面临的问题是：

•可变性：像日期和时间这样的类应该是不可变的。•偏移性：Date中的年份是从1900开始的，而月份都从0开始。•格式化：格式化只对Date有用，Calendar则不行。•此外，它们也不是线程安全的；不能处理闰秒等。

```java
import org.junit.Test;
import java.util.Date;

/**
 * jdk 8中日期时间API的测试
 *
 */
public class JDK8DateTimeTest {

    @Test
    public void testDate(){
        //偏移量
        Date date1 = new Date(2020,9,8);
        System.out.println(date1);  //Fri Oct 08 00:00:00 CST 3920

        Date date2 = new Date(2020 - 1900,9 - 1,8);
        System.out.println(date2); //Tue Sep 08 00:00:00 CST 2020
    }
}
```

第三次引入的API是成功的，并且Java 8中引入的`java.time` API 已经纠正了过去的缺陷，将来很长一段时间内它都会为我们服务。

Java 8 吸收了Joda-Time 的精华，以一个新的开始为Java 创建优秀的API。新的`java.time` 中包含了所有关于**本地日期（LocalDate）、本地时间（LocalTime）、本地日期时间（LocalDateTime）、时区（ZonedDateTime）和持续时间（Duration）的类**。历史悠久的Date 类新增了`toInstant()` 方法，用于把Date 转换成新的表示形式。这些新增的本地化时间日期API 大大简化了日期时间和本地化的管理。

```java
java.time–包含值对象的基础包
java.time.chrono–提供对不同的日历系统的访问java.time.format–格式化和解析时间和日期java.time.temporal–包括底层框架和扩展特性java.time.zone–包含时区支持的类

说明：大多数开发者只会用到基础包和format包，也可能会用到temporal包。因此，尽管有68个新的公开类型，大多数开发者，大概将只会用到其中的三分之一。
```

### 4.1、LocalDate、LocalTime、LocalDateTime的使用

•`LocalDate、LocalTime、LocalDateTime` 类是其中较重要的几个类，它们的实例是**不可变的对象**，分别表示使用ISO-8601日历系统的日期、时间、日期和时间。它们提供了简单的本地日期或时间，并不包含当前的时间信息，也不包含与时区相关的信息。•`LocalDate`代表IOS格式（yyyy-MM-dd）的日期,可以存储生日、纪念日等日期。•`LocalTime`表示一个时间，而不是日期。•`LocalDateTime`是用来表示日期和时间的，**这是一个最常用的类之一**。•注：ISO-8601日历系统是国际标准化组织制定的现代公民的日期和时间的表示法，也就是公历。

```java
import org.junit.Test;

import java.time.LocalDate;
import java.time.LocalDateTime;
import java.time.LocalTime;

/**
 * jdk 8中日期时间API的测试
 */
public class JDK8DateTimeTest {

    /**
     * LocalDate、LocalTime、LocalDateTime的使用
     *
     */
    @Test
    public void test1(){
        //now():获取当前的日期、时间、日期+时间
        LocalDate localDate = LocalDate.now();
        LocalTime localTime = LocalTime.now();
        LocalDateTime localDateTime = LocalDateTime.now();

        System.out.println(localDate);
        System.out.println(localTime);
        System.out.println(localDateTime);

        //of():设置指定的年、月、日、时、分、秒。没有偏移量
        LocalDateTime localDateTime1 = LocalDateTime.of(2020, 10, 6, 13, 23, 43);
        System.out.println(localDateTime1);

        //getXxx()：获取相关的属性
        System.out.println(localDateTime.getDayOfMonth());
        System.out.println(localDateTime.getDayOfWeek());
        System.out.println(localDateTime.getMonth());
        System.out.println(localDateTime.getMonthValue());
        System.out.println(localDateTime.getMinute());

        //体现不可变性
        //withXxx():设置相关的属性
        LocalDate localDate1 = localDate.withDayOfMonth(22);
        System.out.println(localDate);
        System.out.println(localDate1);

        LocalDateTime localDateTime2 = localDateTime.withHour(4);
        System.out.println(localDateTime);
        System.out.println(localDateTime2);

        //不可变性
        LocalDateTime localDateTime3 = localDateTime.plusMonths(3);
        System.out.println(localDateTime);
        System.out.println(localDateTime3);

        LocalDateTime localDateTime4 = localDateTime.minusDays(6);
        System.out.println(localDateTime);
        System.out.println(localDateTime4);
    }
}
```

![null](https://i-blog.csdnimg.cn/blog_migrate/6c046f16220abf78ad2fbb63399480e9.png)

### 4.2、Instant类的使用

•`Instant`：时间线上的一个瞬时点。这可能被用来记录应用程序中的事件时间戳。•在处理时间和日期的时候，我们通常会想到年,月,日,时,分,秒。然而，这只是时间的一个模型，是面向人类的。第二种通用模型是面向机器的，或者说是连续的。在此模型中，时间线中的一个点表示为一个很大的数，这有利于计算机处理。在UNIX中，这个数从1970年开始，以秒为的单位；同样的，在Java中，也是从1970年开始，但以毫秒为单位。•`java.time`包通过值类型`Instan`t提供机器视图，不提供处理人类意义上的时间单位。`Instant`表示时间线上的一点，而不需要任何上下文信息，例如，时区。概念上讲，它只是简单的表示自1970年1月1日0时0分0秒（UTC）开始的秒数。因为`java.time`包是基于纳秒计算的，所以`Instant`的精度可以达到纳秒级。

> (1 ns = 10-9s) 1秒= 1000毫秒=106微秒=109纳秒

![null](https://i-blog.csdnimg.cn/blog_migrate/d87679710658d7baf645c86157ed4bbc.png)

> 时间戳是指格林威治时间1970年01月01日00时00分00秒(北京时间1970年01月01日08时00分00秒)起至现在的总秒数。

![null](https://i-blog.csdnimg.cn/blog_migrate/fb3e98c736a512ab007ab79b57c7dcdf.png)

```java
import org.junit.Test;

import java.time.*;

/**
 * jdk 8中日期时间API的测试
 */
public class JDK8DateTimeTest {

    /**
     * Instant的使用
     */
    @Test
    public void test2(){
        //now():获取本初子午线对应的标准时间
        Instant instant = Instant.now();
        System.out.println(instant);    //2020-05-10T09:55:55.561Z

        //添加时间的偏移量
        OffsetDateTime offsetDateTime = instant.atOffset(ZoneOffset.ofHours(8));//东八区
        System.out.println(offsetDateTime); //2020-05-10T18:00:00.641+08:00

        //toEpochMilli():获取自1970年1月1日0时0分0秒（UTC）开始的毫秒数  ---> Date类的getTime()
        long milli = instant.toEpochMilli();
        System.out.println(milli);  //1589104867591

        //ofEpochMilli():通过给定的毫秒数，获取Instant实例  -->Date(long millis)
        Instant instant1 = Instant.ofEpochMilli(1550475314878L);
        System.out.println(instant1);   //2019-02-18T07:35:14.878Z
    }
}
```

### 4.3、DateTimeFormatter的使用

> `java.time.format.DateTimeFormatter` 类：该类提供了三种格式化方法：

•预定义的标准格式。如：**`ISO_LOCAL_DATE_TIME;ISO_LOCAL_DATE;ISO_LOCAL_TIME`**•本地化相关的格式。如：`ofLocalizedDateTime(FormatStyle.LONG)`•**自定义的格式。如：`ofPattern(“yyyy-MM-dd hh:mm:ss”)`**

![null](https://i-blog.csdnimg.cn/blog_migrate/2bbfdac6fb516b91c551269cd291fdb5.png)

```java
import org.junit.Test;

import java.time.*;
import java.time.format.DateTimeFormatter;
import java.time.format.FormatStyle;
import java.time.temporal.TemporalAccessor;

/**
 * jdk 8中日期时间API的测试
 */
public class JDK8DateTimeTest {

    /**
     * DateTimeFormatter:格式化或解析日期、时间
     *     类似于SimpleDateFormat
     */
    @Test
    public void test3(){
        //方式一：预定义的标准格式。如：ISO_LOCAL_DATE_TIME;ISO_LOCAL_DATE;ISO_LOCAL_TIME
        DateTimeFormatter formatter = DateTimeFormatter.ISO_LOCAL_DATE_TIME;
        //格式化:日期-->字符串
        LocalDateTime localDateTime = LocalDateTime.now();
        String str1 = formatter.format(localDateTime);
        System.out.println(localDateTime);
        System.out.println(str1);//2020-05-10T18:26:40.234

        //解析：字符串 -->日期
        TemporalAccessor parse = formatter.parse("2020-05-10T18:26:40.234");
        System.out.println(parse);

        //方式二：
        //本地化相关的格式。如：ofLocalizedDateTime()
        //FormatStyle.LONG / FormatStyle.MEDIUM / FormatStyle.SHORT :适用于LocalDateTime
        DateTimeFormatter formatter1 = DateTimeFormatter.ofLocalizedDateTime(FormatStyle.LONG);
        //格式化
        String str2 = formatter1.format(localDateTime);
        System.out.println(str2);//2020年5月10日 下午06时26分40秒

        //本地化相关的格式。如：ofLocalizedDate()
        //FormatStyle.FULL / FormatStyle.LONG / FormatStyle.MEDIUM / FormatStyle.SHORT : 适用于LocalDate
        DateTimeFormatter formatter2 = DateTimeFormatter.ofLocalizedDate(FormatStyle.MEDIUM);
        //格式化
        String str3 = formatter2.format(LocalDate.now());
        System.out.println(str3);//2020-5-10


       //重点： 方式三：自定义的格式。如：ofPattern(“yyyy-MM-dd hh:mm:ss”)
        DateTimeFormatter formatter3 = DateTimeFormatter.ofPattern("yyyy-MM-dd hh:mm:ss");
        //格式化
        String str4 = formatter3.format(LocalDateTime.now());
        System.out.println(str4);//2020-05-10 06:26:40

        //解析
        TemporalAccessor accessor = formatter3.parse("2020-05-10 06:26:40");
        System.out.println(accessor);

    }
}
```

### 4.4、其它日期时间相关API的使用

•ZoneId：该类中包含了所有的时区信息，一个时区的ID，如Europe/Paris•ZonedDateTime：一个在ISO-8601日历系统时区的日期时间，如2007-12-03T10:15:30+01:00Europe/Paris。•其中每个时区都对应着ID，地区ID都为“{区域}/{城市}”的格式，例如：Asia/Shanghai等

```java
import org.junit.Test;

import java.time.*;
import java.util.Set;

/**
 * jdk 8中日期时间API的测试
 */
public class JDK8DateTimeTest {
    
    @Test
    public void test1(){
        //ZoneId:类中包含了所有的时区信息
        // ZoneId的getAvailableZoneIds():获取所有的ZoneId
        Set<String> zoneIds= ZoneId.getAvailableZoneIds();
        for(String s: zoneIds) {
            System.out.println(s);
        }
        // ZoneId的of():获取指定时区的时间
        LocalDateTime localDateTime= LocalDateTime.now(ZoneId.of("Asia/Tokyo"));
        System.out.println(localDateTime);
        
        //ZonedDateTime:带时区的日期时间
        // ZonedDateTime的now():获取本时区的ZonedDateTime对象
        ZonedDateTime zonedDateTime= ZonedDateTime.now();
        System.out.println(zonedDateTime);
        // ZonedDateTime的now(ZoneId id):获取指定时区的ZonedDateTime对象
        ZonedDateTime zonedDateTime1= ZonedDateTime.now(ZoneId.of("Asia/Tokyo"));
        System.out.println(zonedDateTime1);
    }
}
```

•Clock：使用时区提供对当前即时、日期和时间的访问的时钟。•持续时间：Duration，用于计算两个“时间”间隔•日期间隔：Period，用于计算两个“日期”间隔•TemporalAdjuster : 时间校正器。有时我们可能需要获取例如：将日期调整到“下一个工作日”等操作。•TemporalAdjusters : 该类通过静态方法(firstDayOfXxx()/lastDayOfXxx()/nextXxx())提供了大量的常用TemporalAdjuster 的实现。

```java
import java.time.Duration;
import java.time.LocalDateTime;
import java.time.LocalTime;

import org.junit.Test;

public class JDK8APITest {
    
    @Test
    public void test2(){
        //Duration:用于计算两个“时间”间隔，以秒和纳秒为基准
        LocalTime localTime= LocalTime.now();
        LocalTime localTime1= LocalTime.of(15, 23, 32);
        //between():静态方法，返回Duration对象，表示两个时间的间隔
        Duration duration= Duration.between(localTime1, localTime);
        System.out.println(duration);
        
        System.out.println(duration.getSeconds());
        System.out.println(duration.getNano());
        
        LocalDateTime localDateTime= LocalDateTime.of(2016, 6, 12, 15, 23, 32);
        LocalDateTime localDateTime1= LocalDateTime.of(2017, 6, 12, 15, 23, 32);
        
        Duration duration1= Duration.between(localDateTime1, localDateTime);
        System.out.println(duration1.toDays());
    }
}
import java.time.Period;
import org.junit.Test;

public class JDK8APITest {
    
    @Test
    public void test3(){
        //Period:用于计算两个“日期”间隔，以年、月、日衡量
        LocalDate localDate= LocalDate.now();
        LocalDate localDate1= LocalDate.of(2028, 3, 18);
        
        Period period= Period.between(localDate, localDate1);
        System.out.println(period);
        System.out.println(period.getYears());
        
        System.out.println(period.getMonths());
        System.out.println(period.getDays());
        
        Period period1= period.withYears(2);
        System.out.println(period1);
    }
}
```

#### 4.4.1、参考：与传统日期处理的转换

![null](https://i-blog.csdnimg.cn/blog_migrate/c9a767d7fc297f07599604456db710f2.png)

## 05、Java比较器

### 5.1、概述

Java中的对象，正常情况下，只能进行比较：`==` 或 `!=` 。不能使用 `>` 或`<`的，但是在开发场景中，我们需要对多个对象进行排序，言外之意，就需要比较对象的大小。 如何实现？使用两个接口中的任何一个：`Comparable` 或 `Comparator`

•Java实现对象排序的方式有两种：•自然排序：`java.lang.Comparable`•定制排序：`java.util.Comparator`

### 5.2、Comparable自然排序举例

```java
import org.junit.Test;
import java.util.Arrays;

public class CompareTest {

    /**
     * Comparable接口的使用举例：  自然排序
     * 1.像String、包装类等实现了Comparable接口，重写了compareTo(obj)方法，给出了比较两个对象大小的方式。
     * 2.像String、包装类重写compareTo()方法以后，进行了从小到大的排列
     * 3. 重写compareTo(obj)的规则：
     *    如果当前对象this大于形参对象obj，则返回正整数，
     *    如果当前对象this小于形参对象obj，则返回负整数，
     *    如果当前对象this等于形参对象obj，则返回零。
     *
     */
    @Test
    public void test1(){
        String[] arr = new String[]{"AA","CC","KK","MM","GG","JJ","DD"};

        Arrays.sort(arr);

        System.out.println(Arrays.toString(arr));
    }

}
```

### 5.3、自定义类实现Comparable自然排序

> 1、测试类

```java
import org.junit.Test;
import java.util.Arrays;

public class CompareTest {

    /**
     * 4.对于自定义类来说，如果需要排序，我们可以让自定义类实现Comparable接口，重写compareTo(obj)方法。
     *   在compareTo(obj)方法中指明如何排序
     */
    @Test
    public void test2(){
        Goods[] arr = new Goods[5];
        arr[0] = new Goods("lenovoMouse",34);
        arr[1] = new Goods("dellMouse",43);
        arr[2] = new Goods("xiaomiMouse",12);
        arr[3] = new Goods("huaweiMouse",65);
        arr[4] = new Goods("microsoftMouse",43);

        Arrays.sort(arr);

        System.out.println(Arrays.toString(arr));
    }

}
```

> 2、Goods类

```java
/**
 * 商品类
 */
public class Goods implements Comparable{

    private String name;
    private double price;

    public Goods() {
    }

    public Goods(String name, double price) {
        this.name = name;
        this.price = price;
    }

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public double getPrice() {
        return price;
    }

    public void setPrice(double price) {
        this.price = price;
    }

    @Override
    public String toString() {
        return "Goods{" +
                "name='" + name + '\'' +
                ", price=" + price +
                '}';
    }

    //指明商品比较大小的方式:按照价格从低到高排序,再按照产品名称从高到低排序
    @Override
    public int compareTo(Object o) {
//        System.out.println("**************");
        if(o instanceof Goods){
            Goods goods = (Goods)o;
            //方式一：
            if(this.price > goods.price){
                return 1;
            }else if(this.price < goods.price){
                return -1;
            }else{
//                return 0;
                return -this.name.compareTo(goods.name);
            }
            //方式二：
//           return Double.compare(this.price,goods.price);
        }
//        return 0;
        throw new RuntimeException("传入的数据类型不一致！");
    }
}
```

### 5.4、使用Comparator实现定制排序

```java
import org.junit.Test;
import java.util.Arrays;
import java.util.Comparator;

/**
 * 一、说明：Java中的对象，正常情况下，只能进行比较：==  或  != 。不能使用 > 或 < 的
 *          但是在开发场景中，我们需要对多个对象进行排序，言外之意，就需要比较对象的大小。
 *          如何实现？使用两个接口中的任何一个：Comparable 或 Comparator
 *
 * 二、Comparable接口与Comparator的使用的对比：
 *    Comparable接口的方式一旦一定，保证Comparable接口实现类的对象在任何位置都可以比较大小。
 *    Comparator接口属于临时性的比较。
 */
public class CompareTest {

    /**
     * Comparator接口的使用：定制排序
     *     1.背景：
     *     当元素的类型没有实现java.lang.Comparable接口而又不方便修改代码，
     *     或者实现了java.lang.Comparable接口的排序规则不适合当前的操作，
     *     那么可以考虑使用 Comparator 的对象来排序
     *     2.重写compare(Object o1,Object o2)方法，比较o1和o2的大小：
     *     如果方法返回正整数，则表示o1大于o2；
     *     如果返回0，表示相等；
     *     返回负整数，表示o1小于o2。
     */
    @Test
    public void test3(){
        String[] arr = new String[]{"AA","CC","KK","MM","GG","JJ","DD"};
        Arrays.sort(arr,new Comparator(){

            //按照字符串从大到小的顺序排列
            @Override
            public int compare(Object o1, Object o2) {
                if(o1 instanceof String && o2 instanceof  String){
                    String s1 = (String) o1;
                    String s2 = (String) o2;
                    return -s1.compareTo(s2);
                }
//                return 0;
                throw new RuntimeException("输入的数据类型不一致");
            }
        });
        System.out.println(Arrays.toString(arr));
    }

    @Test
    public void test4(){
        Goods[] arr = new Goods[6];
        arr[0] = new Goods("lenovoMouse",34);
        arr[1] = new Goods("dellMouse",43);
        arr[2] = new Goods("xiaomiMouse",12);
        arr[3] = new Goods("huaweiMouse",65);
        arr[4] = new Goods("huaweiMouse",224);
        arr[5] = new Goods("microsoftMouse",43);

        Arrays.sort(arr, new Comparator() {
            //指明商品比较大小的方式:按照产品名称从低到高排序,再按照价格从高到低排序
            @Override
            public int compare(Object o1, Object o2) {
                if(o1 instanceof Goods && o2 instanceof Goods){
                    Goods g1 = (Goods)o1;
                    Goods g2 = (Goods)o2;
                    if(g1.getName().equals(g2.getName())){
                        return -Double.compare(g1.getPrice(),g2.getPrice());
                    }else{
                        return g1.getName().compareTo(g2.getName());
                    }
                }
                throw new RuntimeException("输入的数据类型不一致");
            }
        });

        System.out.println(Arrays.toString(arr));
    }
```

> **Comparable接口与Comparator的使用的对比**：

•Comparable接口的方式一旦一定，保证Comparable接口实现类的对象在任何位置都可以比较大小。•Comparator接口属于临时性的比较。

## 06、System类、Math类、BigInteger与BigDecimal

### 6.1、System类

•`System`类代表系统，系统级的很多属性和控制方法都放置在该类的内部。该类位于`java.lang`包。•由于该类的构造器是`private`的，所以无法创建该类的对象，也就是无法实例化该类。其内部的成员变量和成员方法都是`static`的，所以也可以很方便的进行调用。•成员变量•`System`类内部包含`in、out`和`err`三个成员变量，分别代表标准输入流(键盘输入)，标准输出流(显示器)和标准错误输出流(显示器)。•成员方法•`native long currentTimeMillis()`：该方法的作用是返回当前的计算机时间，时间的表达格式为当前计算机时间和GMT时间(格林威治时间)1970年1月1号0时0分0秒所差的毫秒数。•`void exit(int status)`：该方法的作用是退出程序。其中status的值为0代表正常退出，非零代表异常退出。使用该方法可以在图形界面编程中实现程序的退出功能等。•`void gc()`：该方法的作用是请求系统进行垃圾回收。至于系统是否立刻回收，则取决于系统中垃圾回收算法的实现以及系统执行时的情况。String•`getProperty(String key)`：该方法的作用是获得系统中属性名为key的属性对应的值。系统中常见的属性名以及属性的作用如下表所示：

![null](https://i-blog.csdnimg.cn/blog_migrate/68110e6469479808967577982be8877f.png)



```java
import org.junit.Test;

/**
 * 其他常用类的使用
 * 1.System
 * 2.Math
 * 3.BigInteger 和 BigDecimal
 */
public class OtherClassTest {

    @Test
    public void test1() {
        String javaVersion = System.getProperty("java.version");
        System.out.println("java的version:" + javaVersion);

        String javaHome = System.getProperty("java.home");
        System.out.println("java的home:" + javaHome);

        String osName = System.getProperty("os.name");
        System.out.println("os的name:" + osName);

        String osVersion = System.getProperty("os.version");
        System.out.println("os的version:" + osVersion);

        String userName = System.getProperty("user.name");
        System.out.println("user的name:" + userName);

        String userHome = System.getProperty("user.home");
        System.out.println("user的home:" + userHome);

        String userDir = System.getProperty("user.dir");
        System.out.println("user的dir:" + userDir);

    }
}
```

### 6.2、Math类

> `java.lang.Math`提供了一系列静态方法用于科学计算。其方法的参数和返回值类型一般为`double`型。

•abs 绝对值•acos,asin,atan,cos,sin,tan 三角函数•sqrt 平方根•pow(double a,doble b) a的b次幂•log 自然对数•exp e为底指数•max(double a,double b)•min(double a,double b)•random() 返回0.0到1.0的随机数•long round(double a) double型数据a转换为long型（四舍五入）•toDegrees(double angrad) 弧度—>角度•toRadians(double angdeg) 角度—>弧度

### 6.3、BigInteger与BigDecimal

•`Integer`类作为`int`的包装类，能存储的最大整型值为`2^31 -1`，`Long`类也是有限的，最大为`2^63 -1`。如果要表示再大的整数，不管是基本数据类型还是他们的包装类都无能为力，更不用说进行运算了。•`java.math`包的`BigInteger`可以表示不可变的任意精度的整数。`BigInteger` 提供所有Java 的基本整数操作符的对应物，并提供`java.lang.Math` 的所有相关方法。另外，`BigInteger` 还提供以下运算：模算术、GCD 计算、质数测试、素数生成、位操作以及一些其他操作。•构造器•`BigInteger(String val)`：根据字符串构建`BigInteger`对象•常用方法

![null](https://i-blog.csdnimg.cn/blog_migrate/0004e4dfb3ff01bb8d280b20cbf7dafb.png)

•一般的Float类和Double类可以用来做科学计算或工程计算，但**在商业计算中，要求数字精度比较高，故用到`java.math.BigDecimal`类**。•BigDecimal类支持不可变的、任意精度的有符号十进制定点数。•构造器•`public BigDecimal(double val)`•`public BigDecimal(String val)`•常用方法•`public BigDecimal add(BigDecimal augend)`•`public BigDecimal subtract(BigDecimal subtrahend)`•`public BigDecimal multiply(BigDecimal multiplicand)`•`public BigDecimal divide(BigDecimal divisor, int scale, int roundingMode)`



```java
import org.junit.Test;

import java.math.BigDecimal;
import java.math.BigInteger;

/**
 * 其他常用类的使用
 * 1.System
 * 2.Math
 * 3.BigInteger 和 BigDecimal
 */
public class OtherClassTest {

    @Test
    public void test2() {
        BigInteger bi = new BigInteger("1243324112234324324325235245346567657653");
        BigDecimal bd = new BigDecimal("12435.351");
        BigDecimal bd2 = new BigDecimal("11");
        System.out.println(bi);
//         System.out.println(bd.divide(bd2));
        System.out.println(bd.divide(bd2, BigDecimal.ROUND_HALF_UP));
        System.out.println(bd.divide(bd2, 25, BigDecimal.ROUND_HALF_UP));

    }
}
```

