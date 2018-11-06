# Linux是什么?
+ linux系统是一款广泛应用于服务器的操作系统
## Linux有哪些部分?
+ Linux根据分为Garlan和Shaw提出的操作系统分层结构分为4个子系统
   1. 用户进程:运行在Linux  操作最高层的一个庞大的核和软件，一个用户程序在操作系统之上运行时，它相当   于一个进程
   2. 系统调用接口:通过实现系统调用操作系统内核中特定的过程来实现特定的服务
   3. Linux内核:内核式操作系统的灵魂，包括内核抽象核对硬件资源（如cpu)的间接访问，它负责管理磁盘上的文件、内存，负责启动系统并运行程序，负责从网络上接收和发送数据包等等
   4. 硬件控制器:所有Linux安装时所需的物理设备
### Linux用在那些个地方?
1. 充当服务器(如apache)
2. 数据库(如MySQL)
3. 博客系统(workpress)
4. 作为嵌入式操作系统安装在计算机硬件上比如router和CPU等等



# Windows和linux的区别
1. linux是开源软件，而windows不是
2. linux运行程序的空间与系统相对独立，即便软件运行崩溃也不像windows会经常死机
3. linux实现了真正意义上的多用户系统
4. windows系统的中文支持功能很强大，不像linux会出现中文乱码
5. apt的存在使得linux系统的更新变得普遍快捷和简单,相比于漏洞永远来的比补丁快的windows。。。。
6. linux不会中木马。。流氓软件之类的。。原因我还没细查。。。。
7. windows的应用软件数量，兼容性等等等等。。。是linux没法比的
8. windows上手性高于linux，原因都懂得。。。
––––––––
**上述内容总结(~摘抄~)于道客粑粑**

# Linu的文件操作命令
## 新建文件
1. 新建文件夹命令：`mkdir'`文件夹名称
2. 创建文档就用：`vi 文件名`,然后就可以编辑文档了，退出的时候依次按ESC -> : ->x  就退出并保存了，':wq '保存后退出。：`x`同`wq`.`:q! –`不保存内容， 强制退出。
## 删除文件
1. 删除文件夹：`rm[选项]'`文件夹名称。如`rm -r test`
2. 删除文件：`rm `文件名'。如：`rm test.txt`
# 修改文件
1. vi命令。`vi 文件名`这样就可以打开一个文件，再点击i就可以进入编辑了。其实编辑命令还有：o，a。我这里比较熟悉i的使用：退出点击esc键，就进入命令模式。
+ 一些常见的命令，如下：
   +  x:删除当前字符。
   +  dd：删除当前行。
   +  2dd：删除文件的当前行和后一行。
   +  u:恢复前一步操作。
   +  p:复制之前删除的行。
   +  yy:复制光标所在的整行。
   +  2yy:复制2行，举一反三 3yy。
   +  p:粘贴到光标的后面。
## 查看文件：
1. 查看目录下的所有文件又2种命令：`ll` 和`ls`。 `ll`会列出该文件下的所有文件信息，包括隐藏的文件，而`ls只列出显式文件名。
2. 查看某个文件内容也有2种：`cat` 和 `vi` 。`cat`主要有三大功能:
1. 一次显示整个文件：`$ cat filenam`
2. 从键盘创建一个文件：`$ cat` > `filenae`
3. 只能创建新文件,不能编辑已有文件、将几个文件合并为一个文件： `$cat file1 file2 > file`.
   + vi实际上是文件编辑命令，但是也可以查看文件。

# 什么是开源软件?
>开源软件，英文表示是open source software，简称为OSS，直接的字面意思是公开源代码的软件。软件既然连源代码都公开，因此开源软件具备可以免费使用和公布源代码的主要特征。
简单来说，"开源软件"就是源代码开放的软件,因为源代码开放了，只需要稍做修改就可以嵌入到产品中去.


# 根据可提供资源项目开源社区类别
目前开源社区主要分三类：
1. 第一类是提供开源项目协同开发/发布平台、开源资源、交流论坛，这类社区以共创软件联盟为代表，包括武汉Linux协会、LinuxForum。
2. 第二类是提供开源资源、交流论坛、维护自主项目，主要huihoo、Opentop等。
3. 第三类是引进国外开源项目、提供开源资讯、交流论坛，这类社区以信息汇聚、技术交流为主，人气较旺、水平较低，是知识传播、人才汇聚、项目培育的良好平台，其中包括JavaUnion、LinuxSir、Java.com.cn等。
# 根据所需资源提供者分类
1. 第一类是公司或组织。这类社区一般有特定项目，具有可持续、稳定性好、资源丰富等特点，包括北京软件协会支持的共创软件联盟Cosoft、具有公司背景的LinuxAid等，这些社区也因为其信息量，往往能够吸引到足够的网民支持。
2. 第二类是松散团队。 这类社区人气旺盛、发展迅速，但稳定性、持续性较差，包括JavaUnion、Huihoo等，有些社区一旦缺乏管理核心团队或者核心团队无暇顾及网站的时候，立刻就会流失大量用户，不利于社区的发展。
3.第三类是个人。 国内绝大部分社区是靠个人兴趣在维护，这些社区以交流论坛为主、随时可能消失，可以用前扑后续、层出不穷来描述，包括chinajavaworld、linuxSir等，一旦社区的负责人个人失去兴趣，立刻就会消失，不利于培养长期的开源项目。
#常见开源社区
1. [共创软件联盟（http://cosoft.org.cn/html"goto"）
2. [武汉自由软件协会]（http://www.clinux.org"goto"）
3. 开源中国社区（http://oss.org.cn）
4. [LUPA]（http://www.lupaworld.com"goto"）
5. [ChinaUnix.net]（http://chinaunix.net"goto"）
6. [程序员大本营]（http://www.csdn.net"goto"）
7. [Linux中国]（http://www.linux-cn.com"goto"）
8. [Linux人社区]（http://www.linux-ren.org"goto"）
9. [LinuxFans社区]（http://www.linuxfans.org)
10. [LinuxSir社区]（http://www.linuxsir.org）
11. [Linux伊甸园] （http://www.linuxeden.com"goto"）
12. [红联Linux门户]（http://www.linuxdiyf.com"goto"）
13. [红旗Linux技术社区[l]（http://www.redflag-linux.com"goto"）
14. [Linux技术中坚站论坛]（http://www.chinalinuxpub.com"goto"）
15. [UPLinux]（http://bbs.uplinux.com"goto"）
16. [Matrix]（http://www.matrix.org.cn"goto"）
17. [PHPChina]（http://bbs.phpchina.com"goto"）
18. [灰狐动力]（http://www.huihoo.com"goto"）
19. [JAVA中文站]（http://www.java-cn.com"goto"）
20. [JAVA世界中文论坛]（http://bbs.chinajavaworld.com"goto")
21. [Java研究组织]（http://www.javaresearch.org"goto")
22. [EasyWine论坛]（http://www.easywine.org"goto"）
23. [OpenDesktop.net] （http://www.opendesktop.net"goto"）
>上述内容引自CSDN
[饶了我吧，做超链接好累。。](https://blog.csdn.net/bb331/article/details/2665909"come here")

# 开源软件有什么优劣势?
开源了就意味着大家都可以提高改进代码，有利于软件的自我完善和发展
劣势就是不对开源代码具有掌控意义和享有知识产权，就盈利性而言没啥好说的。
***
## 真没啥好说的。。。

## 版本控制的存在意义
# 备份用
代码需要备份，程序员每做一步功能性的更新和迭代，都需要备份一次，而在版本控制工具中你不需要再复制和粘贴，产生大量的代码冗余，只需要提交一次到服务器中就可以。
# 改需求 
另外当需求需要更改时，比如感觉还是以前写的功能好，需要回到以前某个时间点上，只需要找一找那次提交的状态码，一条命令就可以回到那个时间点，而这个场景在实际开发中是经常遇到的。这时的版本控制工具就类似时间机器，可以让你的代码和网站很方便地返回去。
# 协调开发
这个功能算是版本控制器的主要功能，开发一般很少有像ruby语言一样，一个人做一套系统，大部分的公司的开发团队少则十几个人，多则上百。当多个人共同开发一套系统的时候，你改一部分，我改一部分，肯定有代码冲突的地方，当多个人同时改了一个文件，这么多人，每个人改哪一块了？最终以谁的代码为准？如何处理这种场景下的代码冲突？这就是版本控制的协调开发作用。使用git以多个左尖号来标注冲突的代码，凡是有改动的，均会以这种方式来注明。解决git冲突的办法就是把有尖号这一行删除，保留想要的代码块。

# git的操作
## 克隆
$ git clone 地址
 
## 列出所有本地分支
$ git branch
 
## 创建本地分支
$ git branch 名字
 
## 主分支更新
$ git pull
 
## 切换到指定分支
$ git checkout liuyanan
 
## 将master主分支合并到当前分支
$ git merge master
 
## 添加指定文件到暂存区
$ git add [file1] [file2]...
 
## 添加指定目录到暂存区，包括子目录
$ git add [dir]
 
## 添加当前目录的所有文件到暂存区
$ git add all
 
## 查看状态
$ git status
 
## 提交暂存区到仓库区
$ git commit -m [message]
 
## 提交暂存区的指定文件到仓库区
$ git commit [file1] [file2] ... -m [message]
 
## 推送
$ git push origin liuyanan
 
## 删除工作区文件，并且将这次删除放入暂存区
$ git rm [file1] [file2] ...
 
## 停止追踪指定文件，但该文件会保留在工作区
$ git rm --cached [file]
 
## 改名文件，并且将这个改名放入暂存区
$ git mv [file-original] [file-renamed]
 
## 隐藏修改的文件 切换分支时使用
$ git stash
 
## 查看工作现场
$ git stash list
 
## 清空工作现场
$ git stash clear
 
## 恢复工作现场
$ git stash apply stash@{num}
 
## 回到上一次git版本
$ git reset --hard FETCH_HEAD
––––––
**转载自eddieHOO的CSDN博客**

## git和github的关系
1. git是一个版本管理工具，是可以在你电脑不联网的情况下，只在本地使用的一个版本管理工具，其作用就是可以让你更好的管理你的程序，比如你原来提交过的内容，以后虽然修改了，但是通过git这个工具，可以把你原来提交的内容重现出来，这样对于你后来才意识到的一些错误的更改，可以进行还原

2. 关于github，这是一个网站，就是每个程序员自己写的程序，可以在github上建立一个网上的仓库，你每次提交的时候可以把代码提交到网上，这样你的每次提交，别人也都可以看到你的代码，同时别人也可以帮你修改你的代码

3. 总结来说，git可以认为是一个软件，能够帮你更好的写程序，github则是一个网站，这个网站可以帮助程序员之间互相交流和学习。


# ARM架构处理器都有哪些
+ 最早的Acorn开发的ARM1 Sample
+ 改进的ARM2产能型
+ bulabulabula...一直到ARM6于1991年释出，苹果电脑使用ARM610作为Apple Newton PDA的基础
+ strongARM
+ ARMv4
+ ARMv5te
+ ARM925T
+ ARM7TDMI
。。。。
+ **一直到最新的cortex–A76。。。**


# 处理器的架构有哪些?有什么特点?
+ intel,AMD:X86-64(主流处理器架构，可以全面兼容以前x86-32架构的应用)
= IBM:Power–PC
+ intel,Hp:IA-64(放弃了X64的架构，无法很好地进行与32位系统的兼容)
+ IBM,SUN,Hp:RISC(无法与时俱进日暮西山的架构。。。)
+ intel:Core微架构(功耗上大幅降低，拥有双核心、64bit指令集、4发射的超标量体系结构和乱序执行机制等技术，使用65nm制造工艺生产，支持36bit的物理寻址和48bit的虚拟内存寻址，支持 Intel 所有的扩展指令集。)
+ ARM:ARM架构(是一个32位精简指令集（RISC）处理器架构，其广泛地使用在许多嵌入式系统设计。由于节能的特点，ARM处理器非常适用于移动通讯领域，符合其主要设计目标为低能耗特性)
# 为什么路由器可以由Linux实现?
+  路由器是一种嵌入式设备，具有三层结构
+ **硬件基础**
1. 最底层的是微控制器芯片加外围器件组成的硬件系统
2. 中间层是操作系统，是衔接硬件部分和应用程序的过渡层，它既可以完成对底层硬件的基本操作，又能为上层应用程序提供运行环境支持。下面提及我们可以使用uClinux实现这一点
+ **软件基础**
 3. 最上层是应用程序层，实现针对性应用的程序代码部分，比如路由设置等功能程序部分。
##那么，为毛可以实现?##
   1. 首先IP路由的原理设计涉及IP数据报文的转发，通过Linux主机与目的主机直接相连，可以简单直接地实现IP数据报文从一个主机到另一个主机的传递。
   2. 另外路由器算法及路由解决方案不仅可以应用于路由器上，也可以应用于Linux主机上，借助了Linux的网络管理功能，这时主机嵌入了路由器的功能，进行配置即可发送报文，实现路由的功能。
   3. Linux具有几乎全部的网络协议和网络接口。另外比如uclinux是专门为了微控制领域而设计的Linux系统，针对 uclinux内核的二进制代码和源代码都是经过了重新编写，以紧缩和裁剪基本的代码。这就使得uClinux的内核同标准的Linux内核相比非常之小，但是它仍保持了Linux操作系统的主要的优点，如稳定性、强大的网络功能和出色的文件系统支持等，使得路由器的功能便于实现

# 路由器桌面端和路由器端的区别
+ 桌面端安装了较多的图像桌面管理软件
+ 服务器端主要的系统资源为服务保留，应用较少，保证快速高效实现服务

# 操作系统存在的意义
+ 操作系统的第一层含义，它其实是一种驱动程序。让人们不需要关心一些硬件细节，就可以使用硬件。
+ 操作系统的第二层含义，它其实是为了共享使用硬件资源；为使用者指定一些规范，让不同的使用者可以共享使用硬件。
+ 操作系统的第三层含义，就是为了更方便的利用硬件资源；为使用者提供尽可能方便的接口来使用与利用硬件资源。

# 关于计算机分层自己(~抄别人~)的理解
+ 首先计算机层次结构分为软硬件两大部分，按功能下分为七层，零到六级分别为硬联逻辑层，微程序层，传统机器层，操作系统层，汇编语言层，高级语言层和应用语言层。
+ 计算机不同的层次体现了不同的抽象级别，规定了低层向高层服务，仅与前后两个级别交互的原则，确保了
高层直接面向逻辑层，无需与复杂结构的物理层交互。
## 抽象层
+ 操作系统和硬件之间的级别称为hardware abtraction layer
+ 每向上一层呈现一个更高的抽象性
+ 每一层仅关注下一层的接口，不需要了解其内部机制
+ 比方说操作系统看见的硬件是一个硬件抽象层，它不了解硬件的特性及电气布局等等物理性质
+ 通俗说各管各的事，然后考虑怎么把自己办好的事打包交给下一个层次，实现了资源的高效利用(~为什么高效我可不懂~)
## 计算机网络协议分层那些玩意儿
+ 二话不说先来背背背:
1. 物理层:PDU为bit
2. 数据链路层:PDU为frame
3. 网络层:PDU为packet
4. 传输层:PDU为segment
5. 会话层:PDU为section pdu
6. 表示层:PDU为presetation pdu
7. 应用层:PDU为application pdu
 
# uart串口通信的结构
+ 采用模块化层次结构的设计思想，分为数据发送、接收和波特率发生器控制模块三大模块，其中
   + 发送模块实现数据由并行输入到串行输出
   + 接收模块实现数据由串行输入到并行输出
   + 波特率发生器模块控制产生UART时钟频率。
   
# 为什么QT可以跨平台使用?
和java一样，针对每一种OS平台，QT都有一套对应的底层类库，而接口是完全一致的。
因此只要是在QT库上开发的程序，放在任何一种平台下都可以编译运行（前提条件是：程序中没有使用某OS特有的机能）。
也就是说在OS和应用层之间，增加了一个平台层来保证可移植性。
# 为什么VS不能跨平台使用?
+ 布吉岛。。。
~VS2010明明就可以跨平台开发的。。~

# C语言的编译步骤
1. 预处理(preprocessing)
将所有#include的头文件及宏定义替换成其真正的内容
text.c–tect.i
2. 编译(compilation)
将经过预处理后的程序转化为特定汇编码(assembly code)
3. 汇编(assemble)
将上一步的汇编码转化为机器码(machine code)
4. 链接(linking)
将多个目标文以及所需的库文件(.so等)链接成最终可执行文件(executable file)

# 常见的C语言的编译器
1. Visual C/C++6.0/–Microsoft Visual C++
2. Visual Studio–Microsoft Visual Studio
3. win–tc
4. Code::Blocks
5. Turb C
6. gcc
7. DEV C++
8. C–Free
9. Borland C++,WaTCom C++,Borland C++ Builder,GNU DJGPP C++,Lcc win32 C Compiler3.1,High C,My tc...
10. souceinsight

# 主函数的返回值返回什么?
+ return有带参数和不带参数之分.
return带参数的就是返回值.
不带参数的就是结束当前程序块
+ **一般返回值为0的时候代表的是程序的一种正常状态，而返回值为1的时候则代表程序运行遇到问题失败。**
利用程序的返回值，我们可以控制要不要执行下一个程序。
+ 这一块真不好懂,个人觉得简单说返回的是程序的运行状态之类的，吧。。。。同时返回值应当也由系统的运行状态决定(别打我)

# 主函数的参数如何确定
* ***每一个C程序的执行都是在系统的支持下进行的，main函数是系统执行相就的程序得到“调用”，从系统命令行中得到相应的参数***
+ *main函数有两个参数，其中第一个参数的类型为整型，用于指出命令行中字符串的个数；第二个参数是一个字符指针数组，分别指向命令行中各个字符串，其一般形式为：*
+ `main(int argc, char *argv[ ];`其中，变量的名字可以根据程序人员的爱好进行改变，但参数的数目及各参数的类型是不可改变的，如有一个程序文件为file_cpy.exe，如果执行时，命令行为：`file_cpy s_f d_f<CR>`，则参数argc得到值3，而argv[0]、argv[1]、argv[2]分别指向字符串“file_cpy”、“s_f”、“d_f”。
