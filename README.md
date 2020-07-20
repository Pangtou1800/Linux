# Linux

## 第1章 开山篇

### 1.1 本套Linux课程的内容介绍

<dl>
<dt>基础篇</dt>
<dd>Linux入门</dd>
<dd>vm和Linux的安装</dd>
<dd>Linux目录结构</dd>
<dt>实操篇</dt>
<dd>远程登录（XShell XFtp）</dd>
<dd>Vi和Vim编辑器</dd>
<dd>开机、重启和用户注销登录</dd>
<dd>用户管理</dd>
<dd>实用指令</dd>
<dd>定时任务调度</dd>
<dd>磁盘分区、挂载</dd>
<dd>网络配置</dd>
<dd>进程管理</dd>
<dd>RPM和YUM</dd>
<dt>Linux之JavaEE定制篇</dt>
<dd>
<dl>
<dt>Linux搭建Java环境</dt>
<dd>·JDK安装</dd>
<dd>·Eclipse的安装</dd>
<dd>·Tomcat的安装</dd>
<dd>·MySQL的安装</dd>
</dl>
</dd>
<dt>Linux之大数据定制篇</dt>
<dd>
<dl>
<dt>Shell编程</dt>
<dd>1)概述</dd>
<dd>2)Shell脚本执行方式</dd>
<dd>3)Shell变量</dd>
<dd>4)运算符</dd>
<dd>5)条件判断</dd>
<dd>6)流程控制</dd>
<dd>7)函数</dd>
<dd>8)定时维护MySQL数据库</dd>
</dl>
</dd>
<dt>Linux之Python定制篇</dt>
<dd>Python专业开发平台-Ubuntu</dd>
<dd>Ubuntu下Python开发环境</dd>
<dd>APT软件管理和远程登录</dd>
</dl>

### 1.2 Linux的学习方向

    ·Linux运维工程师

    ·Linux嵌入式工程师

    ·Linux下开发项目
        > JavaEE
        > 大数据
        > Python
        > PHP
        > C/C++

### 1.3 Linux的应用领域

    ·个人桌面领域的应用

        传统薄弱环节

    ·服务器领域

        Linux免费、稳定、高效，在服务器领域是最强的

    ·嵌入式领域

        Linux运行稳定，对网络支持良好、成本低，而且可以根据需要进行裁剪。
        内核最小可以只有几百KB。

### 1.4 Linux高手进阶之路

    1. Linux环境下的基本操作命令，包括：

        ·文件操作命令（rm mkdir, chmod, chown）
        ·编辑工具使用（vi, vim）
        ·Linux用户管理（useradd, userdel, usermod）
        等

    2. Linux的各种配置

        ·环境变量配置
        ·网络配置
        ·服务配置

    3. Linux环境下搭建对应语言的开发环境

        ·大数据
        ·JavaEE
        ·Python

    4. 能编写Shell脚本，对Linux服务器进行维护
    5. 能进行安全设置，防止攻击，保障服务器正常运行，能对系统调优
    6. 深入理解Linux系统（对内核有研究），熟练掌握大型网站应用架构组成，并熟悉各个环节的部署和维护方法。

### 1.5 Linux的学习方法和建议

    1. 高效而愉快的学习
    2. 先建立一个整体框架，然后细节
    3. 不需要掌握所有的Linux指令，要学会查询手册和百度
    4. 先know how，再know why
    5. 计算机是一门“做中学”的学科，不必等到会了再做
    6. 适当地囫囵吞枣
    7. Linux不是编程，重点是实际操作，各种常用指令要玩得溜

## 第2章 Linux基础篇 Linux入门

### 2.1 Linux介绍

    1) Linux怎么读
        ·李纽克斯
        ·利尼克斯
        ·里纳克斯

    2) Linux是一款操作系统，现在很多企业级的项目都部署到Linux/Unix服务器上运行
        ·免费
        ·开源
        ·安全
        ·高效
        ·稳定
        ·处理高并发非常强悍

    3) Linux的创始人是林纳斯（Linus Torvalds）

    4) Linux的吉祥物是企鹅Tux
    
    5) Linux主要的发行版本
        ※Linux内核添加应用软件后构成一个发行版本

        ·CentOS
        ·RedHat
        ·Ubuntu
        ·Suse
        ·OpenSuse
        ·红旗Linux

    6) 目前主要的操作系统
        ·Windows
        ·Android
        ·Linux
        ·Mac
        ·IOS
        ·车载系统等

### 2.2 Unix是怎么来的

    70's 贝尔实验室
        Ken tompson, Dennis richres => Unix
    80's
        IBM => AIX
        SUN => Solaris
        HP  => HP UX
        Richard Stallman => 开源计划

### 2.3 Linux是怎么来的

    林纳斯响应GNU计划，与全世界的Linux爱好者共同开发

    Editor, FTP, DBMS, explorer, Desktop...
    GNU Shell
    Linux Kernal
    Hardware

### 2.4 Linux和Unix关系一览图

    Unix
    |
    ------------------------------------
    |       |               |           |
    BSD     Sun Solaris     IBM AIX     AT&T System V
    |                                   |
    FreeBSD                             Minix
                                        |
                                        GNU/Linux内核
                                        |
        -------------------------------------
        |       |           |       |       |
        Ubuntu  Redhat      SUNSE   Fedora  aliyun Linux
                |
                ---------
                |       |
                Redhat  CentOS

### 2.5 Linux和Windows比较

<table>
<tr>
<th>比较</th>
<th>Windows</th>
<th>Linux</th>
</tr>
<tr>
<td>免费与收费</td>
<td>收费且很贵</td>
<td>免费或少许费用</td>
</tr>
<tr>
<td>软件与支持</td>
<td>数量和质量优势，不过大部分软件收费<br>由微软官方提供支持和服务</td>
<td>
开源自由软件，用户可以修改定制和再发布<br>
由于基本免费没有资金支持，部分软件质量和体验欠缺<br>
由全球所有的Linux开发者和自由软件社区提供支持<br>
</td>
</tr>
<tr>
<td>安全性</td>
<td>经常打补丁安装系统更新，还是会中病毒木马</td>
<td>也有安全问题，但相对Windows肯定更加安全</td>
</tr>
<tr>
<td>使用习惯</td>
<td>普通用户基本都是纯图形界面操作，依靠鼠标和键盘完成一切操作，上手容易入门简单</td>
<td>
兼具图形界面操作和完全的命令行操作，可以只用键盘完成一切操作<br>
新手入门比较困难，需要一些学习和指导，一旦熟练之后效率极高</td>
</tr>
<tr>
<td>可定制性</td>
<td>封闭的，系统可定制性差</td>
<td>开源，可定制性非常强</td>
</tr>
<tr>
<td>应用场景</td>
<td>桌面操作系统主要使用Windows</td>
<td>
支撑百度、谷歌、淘宝等应用软件和服务的，是后台成千上万的Linux服务器主机<br>
世界上的大部分软件和服务器都是运行在Linux之上的<br>
</td>
</tr>
</table>

## 第3章 Linux基础篇 VM和Linux系统（CentOS）安装

### 3.1 安装VM和CentOS

    1. 先安装Virtual Machine, VM12
    2. 再安装Linux, CentOS
    3. 原理示意图

    |Windows           | 本机/母机
        |VM软件        |
            |虚拟机空间 |
                |CentOS| 子机

### 3.2 准备好VM和CentOS的安装包

### 3.3 VM的安装步骤

    1. 去BIOS里修改设置开启虚拟化设备支持

    2. 安装虚拟机软件（VM12）

### 3.4 CentOS安装步骤

    1. 创建虚拟机（空间）

    2. 开始安装系统（CentOS6.8）

    ※虚拟机的网络连接的三种形式：
        ·桥接模式
            Linux可以和其他的系统通信。
            但是可能造成IP冲突。

            张三                李四
            Windows             Windows
            192.168.0.10        192.168.0.20
                                    |Linux
                                    |192.168.0.30
            张三 <=> 李四
            张三 <=> 李四的虚拟机

        ·NAT模式（网络地址转换方式）
            Linux可以访问外网，甚至互联网，不会造成IP冲突

            张三                王五
            Windows             Windows
            192.168.0.10        192.168.0.40
                                192.168.100.200
                                    |Linux
                                    |192.168.100.50

            张三 =>X 王五的虚拟机
            张三 <=  王五的虚拟机

        ·主机模式
            Linux是一个独立的主机，不能访问外网

### 3.5 安装CentOS时的注意事项

    Ctrl+Alt释放鼠标光标

### 3.6 VMTools介绍

    ·可以直接粘贴命令在Windows和CentOS之间
    ·可以设置共享文件夹

### 3.7 VMTools安装和使用

    ·安装
        1.进入CentOS
        2.点击VM菜单的install vmware tools
        3.centOS会弹出一个vm的安装包
        4.点击右键解压，得到一个安装文件
        5.进入该vm解压的目录
        6.安装./vmware-install.pl
        7.全部使用默认设置
        8.重启虚拟机生效（reboot）

    ·使用VMTools来设置Windows和Linux的共享文件夹
        在Windows中创建文件夹
        菜单->vm->setting
        启用共享文件夹，选择刚才创建的文件夹路径
        默认在CentOS的/mnt/hgfs/路径下

## 第4章 Linux基础篇 Linux的目录结构

    Linux只有一个根目录

### 4.1 基本介绍

    Linux的文件系统是采用级层式的树状目录结构，在此结构中的最上层是根目录"/"，然后在此目录下再创建其他的目录。
    深刻理解Linux树状文件目录是非常重要的。

    记住一句经典的话：在Linux世界里，一切皆文件。

    /
    |
    ---------------------------------------------------------------------------------
    |       |       |       |       |       |       |       |       |       |       |
    /root   /bin    /boot   /dev    /etc    /home   /var    /lib    /usr    /media  ..
    |                                                               |
    ---------------------------------           -------------------------
    |               |               |           |           |           |
    /root/Desktop   /root/Maildir   ... ...     /usr/bin    /usr/lib    ...

### 4.2 具体的目录结构

    ·/bin[重点] (/usr/bin, /usr/local/bin)
        是Binary的缩写，这个目录存放着最经常使用的命令

    ·/sbin(/usr/sbin, /usr/local/sbin)
        s就是super的意思，这里存放着系统管理员使用的系统管理程序
    
    ·/home[重点]
        存放普通用户的主目录，在Linux中每个用户都有一个自己的目录，一般该目录是以用户的账号命名的
    
    ·/root[重点]
        该目录为系统管理员，也称作超级权限者的用户主目录

    ·/lib
        系统开机所需要最基本的动态连接共享库，其作用类似于Windows里的DLL文件。
        几乎所有的应用程序都需要用到这些共享库。

    ·/lost+found
        这个目录一般情况下是空的，当系统非法关机之后，这里就存放了一些文件

    ·/etc[重点]
        所有的系统管理所需要的配置文件和子目录

    ·/usr[重点]
        这是一个非常重要的目录，用户的很多应用程序和文件都放在这个目录下，类似于Windows下面的Program Files目录
    
    ·/boot[重点]
        存放的是启动Linux时使用的一些核心文件，包括一些连接文件以及镜像文件

    ·/proc
        这个目录是一个虚拟的目录，它是系统内存的映射，访问这个目录来获取系统信息

    ·/src
        service的缩写，该目录存放一些服务启动之后需要提取的数据

    ·/sys
        这是Linux 2.6内核的一个很大的变化。
        该目录下安装了2.6内核中新出现的一个文件系统sysfs

    ·/tmp
        这个目录是用来存放一些临时文件的

    ·/dev
        类似于Windows的设备管理器，把所有的硬件用文件的形式存储

    ·/media[重点]
        Linux系统会自动识别一些设备，例如U盘、光驱等等，当时别后，Linux会把识别的设备挂载到这个目录下。

    ·/mnt[重点]
        系统提供该目录是为了让用户临时挂载别的文件系统的
        我们可以将外部的存储挂载在/mnt/上，然后进入该目录就可以查看里面的内容了

    ·/opt
        这是给主机额外安装软件所摆放的目录。（安装之前）
        如安装Oracle数据库就可以放到该目录下，默认为空

    ·/usr/local[重点]
        这是另一个给主机额外安装软件所安装的目录。（安装之后）
        一般是通过编译源码方式安装的程序

    ·/var[重点]
        这个目录中存放着不断扩充着的东西，习惯将经常被修改的目录存放在这个目录下。
        包括各种日志文件

    ·/selinux(Security-enhanced Linux)
        SELinux是一种安全子系统，它能控制程序只能访问特定文件。

### 4.3 Linux目录总结

    1.Linux的目录中有且只有一个根目录

    2.Linux的各个目录存放的内容是规划好的，不要乱放文件

    3.Linux是以文件的形式来管理我们的设备，因此Linux系统中，一切皆为文件

    4.Linux的各个文件目录下存放什么内容，大家必须有一个认识

    5.学习后，你应该有一颗Linux目录树

## 第5章 Linux实操篇 远程登录Linux服务器