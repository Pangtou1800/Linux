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

### 5.1 为什么要远程登录到Linux

    实际的开发环境情况基本如下：
        ·Linux服务器是开发小组共享的
        ·正式上线的项目是运行在公网的
        ·故而程序员需要远程登录到Linux系统进行项目管理或开发
        ·Linux服务器大多部署在远程机房
        ·远程登录客户端有XShell, Xftp等等，其他的远程工具也大同小异

### 5.2 远程登录Linux-XShell

    前提：需要Linux服务器开启sshd服务（22号端口）

### 5.3 安装XShell并简单使用

    建立连接：
        协议：SSH
        主机：ifconfig从Linux主机获得
        端口：22

    远程登录后，就可以使用指令远程操作Linux了

### 5.4 远程上传下载文件Xftp

    基于Windows，支持SFTP、FTP协议

    建立连接：
        协议：SFTP   ※不能使用FTP协议，因为FTP的默认端口号是21
        主机：ifconfig从Linux主机获得
        端口：22

    连接成功

## 第6章 Linux实操篇 vi和vim编辑器

### 6.1 vi和vim的基本介绍

    所有的Linux系统都会内置vi文本编辑器

    Vim具有程序编辑的能力，可以看做是Vi的增强版，可以主动的以字体颜色辨认语法的正确性，方便程序设计。
    代码补完、编译及错误跳转等方便编程的功能特别丰富，在程序员中间被广泛使用。

### 6.2 vi和vim的三种常见模式

    1.正常模式

        以vim打开文档一般就进入正常模式了。
        在正常模式里，可以用[上下左右]键移动光标，可以使用[删除字符]或[删除整行]来处理档案内容，
        也可以使用[复制、粘贴]来处理文件数据。

        在正常模式下，我们可以使用快捷键。

    2.插入模式（编辑模式）

        按下i, I, o, O, a, A, r, R等任何一个字母后会进入编辑模式，一般来说按i即可。

        在插入模式下，程序员可以输入内容

    3.命令行模式

        在这个模式中，可以提供相关的指令，完成读取、存盘、替换、离开vim、显示行号等的动作。

### 6.3 快速入门案例

    ·使用vim开发一个Hello.java程序

### 6.4 vi和vim三种模式的相互切换

    在命令行下：
            -- vim xxx -->
                            一般模式/正常模式
            <-- i 或者 a --                     -- : 或者 / -->
            --- ESC ------>                     <---- ESC ----
    编辑模式                                                    命令模式
                                                                :wq :q :q!

    wq：保存修改并退出
    q：在没有修改的情况下退出
    q!:不保存修改强制退出

### 6.5 vi和vim快捷键

    ·拷贝当前行 yy，拷贝当前行向下的5行 5yy，并粘贴　p
    ·删除当前行 dd，删除当前行向下的5行 5dd
    ·在文件中查找某个单词
        => 命令行模式下 /关键字 回车
           自动回到正常模式 n查找下一个
    ·设置文件的行号，取消文件的行号
        => 命令行模式下 :set nu 和 :set nonu
    ·编辑/etc/profile文件，使用快捷键到达文档的最末行[G]和最首行[gg]
    ·在一个文件中输入“Hello”，然后又撤销这个动作 u
    ·编辑/etc/profile文件，并把光标移动到第20行
        第一步：显示行号 :set nu
        第二步：输入20
        第三步：输入shift + g

## 第7章 Linux实操篇 开机、重启和用户登录注销

### 7.1 关机&重启指令

    基本介绍

        1. shutdown

            shutdown -h now : 立即关机
            shutdown -h 1 : 1分钟后关机
            shutdown -r now : 立即重启

        2. halt

            halt 直接使用，效果等价于关机
        

        3. reboot

            reboot 重启系统
        

        4. sync

            sync 把内存的数据同步到磁盘上

    注意细节
        
        当关机或重启时，都应该先执行一次sync指令，把内存的数据存入磁盘，防止数据丢失

### 7.2 用户登录和注销

    基本介绍

        1. 登录时尽量少用root账号登录，因为它是系统管理员，最大的权限，避免操作失误。

            可以利用普通用户登录，登录后再用“su - 用户名”命令来切换成系统管理员身份。

        2. 在提示符下输入logout即可注销用户

    使用细节

        1. logout注销指令在图形运行级别无效，在运行级别3下有效
        2. 运行级别的概念以后会有介绍

    

## 第8章 Linux实操篇 用户管理

### 8.1 基本介绍

    用户管理规则示意图

    Linux操作系统

                    home目录
                    /home/下有各个创建的用户对应的家目录，登录时会自动地进入到自己的家目录
    root   root组

    小明   组2      /home/xm

    小红   组3      /home/xh

    ·Linux系统是一个多用户多任务的操作系统，任何一个要使用系统资源的用户，都必须先向系统管理员申请一个账号，然后以这个账号的身份进入系统。

    ·Linux的用户需要至少属于一个组

### 8.2 添加用户

    基本语法：

        useradd [选项] 用户名

        1. 如果没有指定组，那么以用户名创建组，并将用户指定属于该组

        ※特别说明：cd（change directory），切换目录

    细节说明：

        1. 当用户创建成功后，会自动创建和用户名同名的家目录
        2. useradd -d 指定目录 新的用户名，给新创建的用户指定家目录

### 8.3 指定/修改密码

    基本语法：

        passwd 用户名

        ※  1.在工作中密码必须复杂一点
            2.在使用passwd指定密码时界面是看不到的

### 8.4 删除用户

    基本语法：

        userdel 用户名

        1. 删除用户而保留家目录

            默认行为

        2. 删除用户同时删除家目录

            userdel -r 用户名

    ※在删除用户时，一般会保留家目录

### 8.5 查询用户信息

    基本语法：

        id 用户名

            uid：用户ID
            gid：组ID

### 8.6 切换用户

    介绍：

        在操作Linux时，如果当前用户的权限不够，可以通过su - 指令，切换到高权限用户

    基本语法：

        su - 切换用户名

    细节：

        1. 从权限高的用户切换到权限低的用户不需要输密码，反之则需要
        2. exit 返回到原来的用户

### 8.7 查看当前用户/登录用户

    基本语法：

        whoami/who am I

### 8.8 用户组

    介绍：

        类似于角色，系统可以对有共性的多个用户进行统一的管理

    新增组：

        groupadd 组名

    删除组：

        groupdel 组名

    新增用户时直接加上组：

        useradd -g 用户组 用户名

    修改用户的组：

        usermod -g 用户组 用户名

### 8.9 用户和组的相关文件

    1. /etc/passwd文件

    

        用户配置文件，记录用户的各种信息
        含义：
            用户名: 口令: 用户标识号: 组标识号: 注释性描述: 主目录: 登录Shell

    2. /etc/shadow文件

        口令/密码配置文件
        含义：
            登录名:加密口令:最后一次修改时间:最小时间间隔:最大时间间隔:警告时间:不活动时间:失效时间:标志

    3. /etc/group文件

        组配置文件，记录Linux包含的组的信息
        含义：
            组名:口令:组标识号:组内用户列表
        

## 第9章 Linux实操篇 实用指令

### 9.1 指定运行级别

    基本介绍：

    

        0：关机
        1：单用户（找回丢失密码）
        2：多用户无网络服务
        3：多用户有网络服务 ☆最多使用
        4：保留
        5：图形界面
        6：重启

        常用运行级别是3和5，要修改默认的运行级别可以修改配置文件

    系统运行级别配置文件：
        /etc/inittab
            id:5:initdefault
        命令：init 0|1|2|3|4|5|6

### 9.2 切换到指定的运行级别

        init 运行级别

        如： init 3

    场景：如何找回丢失的root密码？

        思路：进入到 单用户模式，然后修改root密码
        原因：因为单用户模式root不需要密码就可以登录
        步骤:
            1.开机界面时进入菜单画面
            2.e
            3.向下一次，选中kernel/vmlinuz-......
            4.e
            5.在....rhgb quiet后输入 [ 1]  ※运行级别
            6.回车
            7.b
            8.此时就以单用户模式启动了Linux，passwd root指令修改密码即可

        前提：必须在可以物理接触Linux电脑的场合才能实施，远程无法操作

### 9.3 帮助指令

    介绍

        当我们对某个指令不熟悉时，我们可以使用Linux提供的帮助指令来了解这个指令的使用方法。

    ·man 获得帮助信息

        man 命令或配置文件

        例如： man ls

    ·help 获得Shell内置命令的帮助信息

        help 命令

        例如：help cd

### 9.4 文件目录类

    ·pwd指令

        功能：
            显示当前工作目录的绝对路径

        语法：

            pwd

    ·ls指令

        功能：
            显示目录内容

        语法：

            ls [选项] 目录|文件

        常用选项：
            -a 显示当前目录所有的文件和目录，包括隐藏的
            -l 以列表的方式显示信息

    ·cd指令

        功能：
            改变当前工作目录

        语法：

            cd 目标路径

        常用参数：
            绝对路径和相对路径
            cd ~ 或者 cd（无参）  回到用户的家目录
            cd.. 回到上级目录

    ·mkdir指令

        功能：
            创建目录
        

        语法：

            mkdir [选项] 要创建的目录

        常用选项：
            -p 创建多级目录

    ·rmdir指令

        功能：
            删除空目录

        语法：

            rmdir [选项] 要删除的空目录

        使用细节：
            目录下有文件是无法删除，要使用 rm -rf 目标目录 来删除非空目录

    ·touch指令

        功能：
            创建一个空文件

        语法：

            touch 文件名 [文件名2|...]

        细节：
            可以一次性创建多个文件

    ·cp指令 ☆

        功能：
            cp指令拷贝文件到指令目录

        语法：

            cp [选项] source dest

        常用选项：
            -r 递归复制整个文件夹

        细节：
            使用\cp 来取消覆盖时确认提示

    ·rm指令

        功能：
            移除文件或目录
        

        语法：

            rm [选项] 要删除的文件或目录

        常用选项：
            -r 递归删除整个文件夹
            -f 强制删除不提示

    ·mv指令

        功能：
            移动文件或重命名

        语法：

            mv oldFileName newFileName 重命名
            mv /folder/movefile /targetFolder 移动文件夹
            mv /folder/oldfile /targetFolder/newfile 移动并重命名

    ·cat指令

        功能：
            查看文件内容 ※只能浏览不能修改

        语法：

            cat [选项] 要查看的文件

        常用选项：
            -n 显示行号

        说明：
            在指令最后添加 | more 使文件内容分页显示（管道命令）

    ·more指令

        功能：
            一个基于vi编辑器的文本过滤器，它以全屏幕的方式按页显示文本文件的内容。
            more指令中内置了若干快捷键

        语法：

            more 要查看的文件

        快捷键：
            q 退出
            回车 换行
            space 换页
            Ctrl+B 前一页
            Ctrl+F 向下滚动一屏
            = 输出当前的行号
            :f 输出文件名和当前的行号

    ·less指令

        功能：
            less指令用来分屏查看文件内容，它的功能与more指令类似，但是比more指令更加强大，支持各种显示终端。
            less指令在显示文件内容时，并不是一次将整个文件加载之后才显示，而是根据显示需要加载内容，在显示大型文件时有较高的效率。

        语法：

            less 要查看的文件

        快捷键：
            q 退出
            space 向下翻页
            [pagedown] 向下翻页
            [pageup] 向上翻页
            /字符串 向下查找字符串，n:向下，N:向上
            ?字符串 向下查找字符串，n:向下，N:向上

    ·输出重定向（>）和追加（>>）指令

        功能：
            >指令：输出重定向，将原来的文件内容覆盖
            >>指令：追加，不会覆盖原来文件的内容，而是追加到尾部

        语法：

            1. ls -l > a.txt 将指令结果覆盖写入a.txt中，如果该文件不存在就创建
            2. ls -l >> a.txt 将指令结果追加写入a.txt中，如果该文件不存在就创建
            3. cat a.txt > b.txt a的内容覆盖到b中
            4. cat a.txt >> b.txt a的内容追加到b中
            5. echo "AAA" >> a.txt
            6. cal > today.txt 将当前日历信息写入文件

    ·echo指令

        功能：
            输出内容到控制台

        语法：

            echo [选项] [输出内容]

            例如：echo $PATH 输出PATH环境变量的值

    ·head指令

        功能：
            显示文件开头部分内容，默认情况下显示前10行内容
        

        语法：

            head 文件名
            head -n 5 文件名

    ·tail指令

        功能：
            显示文件尾部部分内容，默认情况下显示最后5行内容

        语法：

            tail 文件名
            tail -n 5 文件名
            tail -f 文件 ※实时跟踪文档的所有更新， Ctrl + C退出

    ·ln指令

        功能：
            软连接，也叫符号链接，类似于Windows里的快捷方式，主要存放了其他文件的路径

        语法：

            ln -s 源文件或目录 软连接名

        细节：
            在软连接里使用pwd查看，显示的仍然是软连接的目录
            在删除软连接时不要带上/

    ·history指令

        功能：
            查看已经执行过的历史命令，也可以执行历史指令

        语法：

            history [n]

        选项：
            显示最近执行过的n条指令

        补充：
            ![n] 执行history中编号为n的指令

### 9.5 时间日期类

    ·date指令

        功能1：
            显示当前日期
        

        语法：

            date
            date "+%Y%m%d"
            date "+%Y-%m-%d %H:%M:%S"

        功能2：
            设置日期

        语法：

            date -s 字符串时间

            ex. date -s "2020-7-24 20:10:20"

    ·cal指令

        功能：
            以日历的方式显示时间
        

        语法：

            cal [选项]

            ※没有选项时显示本月日历
        
        常用选项
            cal -y
            cal 2020

### 9.5 搜索查找类

    ·find指令

        功能：
            从指定目录向下递归地遍历其各个子目录，将满足条件的文件或者目录显示在终端。

        语法：

            find 搜索范围 [选项]

        选项：
            -name 查询对象名        按照指定的文件名查找模式查找文件 ※可以使用通配符
            -user 用户名            查找属于指定用户名所有文件
            -size [+|-| ]文件大小   按照指定的文件大小查找文件  

    ·locate指令    

        功能：
            locate指令可以快速定位文件路径。
            locate指令利用事先建立的系统中所有文件名称及路径的locate数据库实现快速定位指定的文件。
            Locate无需遍历整个文件系统，查询速度较快。
            但是问了保证查询的准确度，管理员必须定时更新Locate时刻。

        语法：

            locate 搜索文件

        特别说明：
            locate指令基于数据库进行查询，所以第一次运行前，必须使用
                updatedb指令
            创建lcoate数据库。

    ·grep指令和管道符号

        功能：
            grep过滤查找，管道符，“|”，表示将前一个指令的处理输出结果传递给后面的命令处理。

        语法：

            grep [选项] 查找内容 源文件

        常用选项：
            -n 显示行号

            -i 忽略字母大小写

### 9.6 压缩和解压缩类

    ·gzip/gunzip指令

        功能：
            gzip压缩文件为.gz文件
            gunzip解压.gz文件

        语法：

            gzip 文件名
            gunzip .gz文件

        特别说明：
            gzip/gunzip指令执行后原文件会被删除

    ·zip/unzip指令

        功能：
            zip用于压缩文件，unzip用于解压缩，在项目打包发布中很有用。

        语法：

            zip [选项] xxx.zip 要压缩的目录或文件
            unzip [选项] xxx.zip
        
        常用选项：
            -r 递归压缩整个目录
            -d (unzip使用) 指定解压后的存放目录

    ·tar指令

        功能：
            tar是打包指令，最后打包好的是.tar.gz文件

        语法：

            tar [选项] xxx.tar.gz 打包的内容

        常用选项：
            -c 产生.tar打包文件
            -v 显示详细信息
            -f 指定压缩后的文件名
            -z 打包同时压缩
            -x 解包.tar文件
            -C 指定为目录模式

        案例：

            1. 压缩多个文件，将/home/a1.txt和/home/a2.txt

                tar -zcvf a.tar.gz /home/a1.txt /home/a2.txt
            

            2. 压缩home下的aaa文件夹

                tar -zcvf aaa.tar.gz /home/aaa

            3. 解压a.tar.gz到当前目录

                tar -zxcf a.tar.gz

            4. 解压a.tar.gz到/home/a

                tar -zxcf a.tar.gz -C /home/a

        前提：
            指定解压到的目录必须事先存在

## 第10章 Linux实操篇 组管理和权限管理 ☆

### 10.1 Linux组的基本介绍

    在Linux中的每个用户必须属于一个组，不能独立于组外。
    在Linux中每个文件都有所有者、所在组、其他组的概念。

    1.所有者
    2.所在组
    3.其他组
    4.改变用户所在的组

### 10.2 文件/目录的所有者

    一般为文件的创建者。谁创建了该文件，就自然成为该文件的所有者。

    ·查看文件的所有者

        语法：

            ls -ahl

        实例：
            创建一个组Polic，再创建一个用户Tom，将Tom归入Polic组
            然后使用Tom来创建一个文件OK.txt

    ·修改文件的所有者

        语法：

            chown 用户名 文件名

        实例：
            使用root创建一个文件Apple.txt，修正其所有者为Tome

        注意：
            修改用户之后文件所在组并不会发生变化

    

    ·修改文件所在的组

        语法：

            chgrp 组名 文件名

        实例：
            使用root创建一个文件Orange.txt，修正其所在组为Police

### 10.3 其他组

    除文件的所有者和所在组的用户外，系统的其他用户都是文件的其他组。

### 10.4 权限的基本介绍

    ls -lh 中显示的内容如下：

        -rw-r--r--. 1 Tome    root         14 7月  25 20:10 Apple.txt

        - 文件的类型：
            - 普通文件  d 目录  l 连接文件  c 字符设备【键盘，鼠标】  b 块文件【硬盘】

         rw- 文件所有者拥有的权限
            r-- 文件所在组的用户拥有的权限
               r-- 文件的其他组的用户的权限
                        r 读权限  w 写权限  x 可执行  - 没有权限
                    1 如果是文件，表示硬链接的数量；如果是目录，则表示子目录的个数
                      Tome 文件所有者
                              root 文件所在组
                                           14 文件大小（目录统一是4096）
                                              7月  25 20:10 文件最后的修改时间
                                                            Apple.txt 文件名

    1.第0位确定文件类型
    2.第1-3位表示所有者权限
    3.第4-6位表示所在组的用户的权限
    4.第7-9位表示其他组的用户的权限

### 10.5 rwx权限详解

    ·rwx作用到文件

        [r]代表可读
        [w]代表可写，可以修改，但不代表可以删除该文件。
            删除一个文件的前提条件是对该文件所在的目录有写权限。
        [x]代表可执行

    ·rwx租用到目录

        [r]代表可读，ls查看目录内容
        [w]代表可写，可以修改，目录内创建+删除+重命名
        [x]代表可以进入该目录

    ※rwx可以用数字来表示r: 4 w:2 x:1, 故rwx:7

### 10.6 修改权限

    基本说明：
        通过chmod指令，可以修改文件或者目录的权限

    语法1：

        + - =变更权限

        u:所有者  g:所在组  o:其他人  a:所有人（u,g,o的总和）
        chmod u=rwx,g=rx,o=x 文件目录名  为各目标指定权限
        chmod o+w 文件目录名 为各目标增加权限
        chmod a-x 文件目录名 为各目标减少权限

    案例1：
        给abc这个文件 所有者读写执行权限，组读和执行权限，其他人读写权限
            chmod u=rwx,g=rx,o=rw abc
        给abc这个文件 所有者减少执行权限，组增加写权限
            chmod u-x,g+w abc

    语法2：
        r=4, w=2, x=1
        通过数字变更权限
        chmod 751  =>  chmod u=wrx,g=rx,o=x

    案例2：
        将abc的权限修改为rwxr-x--x
            chomd 751 abc

### 10.7 修改文件所有者（增强）

    语法：
        chown newowner file 改变文件的所有者
        chown newowner:newgroup file 改变文件的所有者和所在组

    常用选项：
        -R 如果是目录，递归修改目录下所有子目录和文件的所有者

### 10.8 实践：警察和土匪

    组：police, bandit
    警察：jack, jerry
    土匪: xh, xq

    1.创建组
        groupadd police
        groupadd bandit
    2.创建用户
        useradd -g police jack
        useradd -g police jerry
        useradd -g bandit xh
        useradd -g bandit xq
        ※为所有用户指定密码，用于登录
            passwd jack
            ...
    3.jack创建一个文件，自己可以读写，本组人可以读，其他组人没有任何权限
        chmod 640 jack01.txt
    4.jack修改该文件，让其他组人可以读，本组人可以读写
        chomd g=rw,o=r jack01.txt
    5.xh投靠警察，看看是否可以读写
        jack: chmod 750 /home/jack 把自己的家文件开放本组的访问权限（x需要开放）
        root: usermod -g police xh
        xh：需要重新登入，组权限才会生效

## 第11章 Linux实操篇 定时任务调度

### 11.1 crond任务调度

    contab进行任务调度

    ·如果只是简单的任务，可以不用写脚本，直接在crontab中加入任务即可
    ·如果任务比较复杂，主要编写脚本（Shell）

### 11.2 概述

    任务调度：
        指系统在某个特定的时间执行的特定的命令或程序
    任务调度分类：
        1.系统工作
            有些重要的工作必须周而复始地执行，比如病毒扫描
        2.个别用户工作
            个别用户可能希望执行某些工作，比如数据库备份

### 11.3 基本语法

    语法
        crontab [选项]

    常用选项
        -e 编辑crontab定时任务
        -l 查询crontab任务
        -r 删除当前用户所有的crontab任务

    保存退出后调度任务就会生效    

    service crond restart 重启任务调度进程

### 11.4 快速入门案例

    任务要求：
        设置个人任务调度 crontab -e
        接着输入任务调度到文件
            如：*/1 * * * * ls -l /etc/ > /tmp/to.txt
            意思：每小时每分钟执行 ls -l /etc/ > /tmp/to.txt 命令

### 11.5 参数细节说明

    ·5个占位符的说明：

        * 一个小时中的第几分钟 0-59
          * 一天中的第几个小时 0-23
            * 一个月中的第几天 1-31
              * 一年当中的第几个月 1-12
                * 一周当中的星期几 0-7（0和7都代表星期日）

    

    ·特殊符号的说明：

        * 任何时间。

            比如第一个*就代表一小时中每分钟都执行一次。
        , 代表不连续的时间。
            比如“0 8, 12, 16 * * *”命令，代表每天的8时0分，12时0分，16时0分执行一次。

        - 代表连续的范围

            比如“0 5 * * 1-6”命令，代表在周一到周六的凌晨5时0分执行命令。
        */n 代表每隔多久执行一次。
            比如“*/10 * * * *”命令，代表每隔10分钟执行一次命令。

        ※几号和星期几最好不要同时出现，容易引起混乱

### 11.6 几个应用实例

    1. 每隔1分钟，就将当前的日期信息，追加到/tmp/mydate文件中

        1) 先编写一个Shell文件 myTask1.sh
            date >> /tmp/mydate
        2) 给myTask1.sh一个可执行权限
        3) crontab -e
        4) */1 * * * * /home/myTask1.sh
        5) 保存退出

    

    2. 每隔1分钟，把当前日期和日历都写到/tmp/mydate文件中

    3.每天凌晨2:00将MySQL数据库备份到MySQL.db.bak文件中
        1) 先编写一个Shell文件 myTask3.sh
            /usr/local/mysql/bin/mysqldump -u root -p root testdb > /tmp/MySQL.db.bak
        2) 给myTask3.sh一个可执行权限
        3) crontab -e
        4) 0 2 * * * /home/myTask3.sh
        5) 保存退出

## 第12章 Linux实操篇 Linux磁盘分区、挂载

### 12.1 分区基础知识

    分区的两种模式：

        ·mbr分区
            1.最多支持四个主分区
            2.系统只能安装在主分区
            3.扩展分区要占一个主分区
            4.MBR最大支持2TB，但拥有最好的兼容性

        ·gtp分区
            1.支持无限多个主分区（但操作系统可能有限制，比如Windows下最多128个分区）
            2.最大支持18EB的容量（E>P>T>G）
            3.Windows7 64位之后都支持gtp分区模式

    Windows下的磁盘分区：

        |Disk                                                |
        |主分区 Primary Partition|扩展分区 Extended Partition |
                                 |逻辑分区1|逻辑分区2|...     |

### 12.2 Linux分区

    原理介绍：

        1.对Linux来说无论有几个分区，分给哪一个目录使用，它归根结底就只有一个根目录，
            一个独立且唯一的文件结构，Linux中每个分区都是用来组成整个文件系统的一部分。

        2.Linux采用了一种叫“载入”的处理方法。
            它的整个文件系统中包含了一整套的文件和目录，且将一个分区和一个目录联系起来。
            这使要载入的一个分区将使它的存储空间在一个目录下获得。

            mount 挂载
            umount 卸载

            磁盘            Linux
                            /
                            |-----------   ...
            分区1 ------->  boot/       |
                                        |
            分区2 ----------------->  mnt/

### 12.3 硬盘说明

    1.Linux硬盘分IDE硬盘和SCSI硬盘，目前基本上是SCSI硬盘

    2.对于IDE硬盘，驱动器标识符号为“hdx~”，其中“hd”表名分区所在的设备类型，这里指IDE硬盘。
        “x”为盘号（a为基本盘，b为基本从属盘，c为辅助主盘，d为辅助从属盘。
        “~"代表分区，前四个分区用数字1~4表示，它们是主分区或扩展分区，从5开始是逻辑分区。
        例：hda3表示为第一个IDE硬盘上的第三个主分区或扩展分区
            hdb2就表示第二个IDE硬盘上的第二个主分区或扩展分区

    3.对于SCSI硬盘则标识为“sdx~”，SCSI硬盘用“sd”来表示区分所在设备类型，其余和IDE相同。

### 12.3 查看当前系统的分区情况

    语法
        lsblk -f

        NAME   FSTYPE LABEL UUID                                 MOUNTPOINT
        情况   类型          唯一标识分区，格式化后生成             挂载点
        sda                                                      
        ├─sda1 ext4         978f776c-462d-4ce6-ae7f-13b39abec695 /boot
        ├─sda2 swap         a70fff76-c0b8-4163-b406-ffc055946c01 [SWAP]
        └─sda3 ext4         99e3f6df-65f7-444d-ae4e-16c66e33fd86 /

    

    语法
        lsblk

        NAME   MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
        sda      8:0    0   20G  0 disk 
        ├─sda1   8:1    0  200M  0 part /boot
        ├─sda2   8:2    0    2G  0 part [SWAP]
        └─sda3   8:3    0 17.8G  0 part /
        sr0     11:0    1 1024M  0 rom                  ←光驱

### 12.4 挂载的经典案例

    案例：
        为系统增加一块硬盘（2G sdb1到 /home/newdisk）

    

    准备工作：
        为虚拟机增加一块硬盘

        NAME   MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
        sr0     11:0    1 1024M  0 rom  
        sda      8:0    0   20G  0 disk 
        ├─sda1   8:1    0  200M  0 part /boot
        ├─sda2   8:2    0    2G  0 part [SWAP]
        └─sda3   8:3    0 17.8G  0 part /
        sdb      8:16   0    2G  0 disk 　　　　　　　　　←尚未分区

    步骤：
        1.分区
            fdisk [选项] device  - Partition table manipulator for Linux
              fdisk /dev/sdb
                m  print help menu
                n  add a new partition
                    p  primary partition  
                    1  prtition number
                    Enter  first cylinder(default)
                    Enter  last cylinder(default)
                w  write table to disk and exit

                d  删除分区
                p  显示磁盘分区

        NAME   MAJ:MIN RM  SIZE RO TYPE MOUNTPOINT
        sr0     11:0    1 1024M  0 rom  
        sda      8:0    0   20G  0 disk 
        ├─sda1   8:1    0  200M  0 part /boot
        ├─sda2   8:2    0    2G  0 part [SWAP]
        └─sda3   8:3    0 17.8G  0 part /
        sdb      8:16   0    2G  0 disk 
        └─sdb1   8:17   0    2G  0 part 　　　　　　　　　←分区完成

        NAME   FSTYPE LABEL UUID                                 MOUNTPOINT
        sr0                                                      
        sda                                                      
        ├─sda1 ext4         978f776c-462d-4ce6-ae7f-13b39abec695 /boot
        ├─sda2 swap         a70fff76-c0b8-4163-b406-ffc055946c01 [SWAP]
        └─sda3 ext4         99e3f6df-65f7-444d-ae4e-16c66e33fd86 /
        sdb                                                      
        └─sdb1  　　　　　                        　　　　←但是没有格式化

        2.格式化
            mkfs [-t fstype] filesys  - build a Linux file system
              mkfs -t ext2 /dev/sdb1
        
        NAME   FSTYPE LABEL UUID                                 MOUNTPOINT
        sr0                                                      
        sda                                                      
        ├─sda1 ext4         978f776c-462d-4ce6-ae7f-13b39abec695 /boot
        ├─sda2 swap         a70fff76-c0b8-4163-b406-ffc055946c01 [SWAP]
        └─sda3 ext4         99e3f6df-65f7-444d-ae4e-16c66e33fd86 /
        sdb                                                      
        └─sdb1 ext2         4797ae2c-95a0-4214-aa3a-0d65ce110ccb 
                                                        ↑格式化完成，没有挂载

        3.挂载
            a. 创建目录/home/newdisk
            b. 挂载sdb1到/home/newdisk
                mount [选项] device dir
                  mount /dev/sdb1 /home/newdisk

        NAME   FSTYPE LABEL UUID                                 MOUNTPOINT
        sr0                                                      
        sda                                                      
        ├─sda1 ext4         978f776c-462d-4ce6-ae7f-13b39abec695 /boot
        ├─sda2 swap         a70fff76-c0b8-4163-b406-ffc055946c01 [SWAP]
        └─sda3 ext4         99e3f6df-65f7-444d-ae4e-16c66e33fd86 /
        sdb                                                      
        └─sdb1 ext2         4797ae2c-95a0-4214-aa3a-0d65ce110ccb /home/newdisk
                                                                    ↑挂载完成

            ※但此时是临时挂载，重启机器后挂载关系就消失了

        4.设置永久（自动）挂载
            a. vim /etc/fstab
            b. 将挂载关系记录
                /dev/sdb1   /home/newdisk   ext4    defaults    0   0
            c. mount -a 即可生效

### 12.5 卸载分区

    语法:
        umount 设备名|目录

### 12.6 磁盘情况查询

    功能1：
        查询系统整体磁盘使用情况

    语法:
        df -lh  - report file system disk space usage

        Filesystem      Size  Used Avail Use% Mounted on
        /dev/sda3        18G  3.1G   14G  19% /
        tmpfs           2.0G   84K  2.0G   1% /dev/shm
        /dev/sda1       190M   39M  142M  22% /boot
        /dev/sdb1       2.0G  3.0M  1.9G   1% /home/newdisk

    功能2：
        查询指定目录的磁盘占用情况

    语法：
        du -ach 目录  - estimate file space usage

    常用选项：
        -s 指定目录占用大小汇总
        -h 带计量单位
        -a 含文件
        --max-depth=1 子目录深度
        -c 列出明细的同时，增加汇总值

### 12.7 磁盘情况：工作实用指令

    1.统计/home目录下文件的个数
        ls -l /home | grep "^-" | wc -l

            wc  - print newline, word, and byte counts for each file

    2.统计/home目录下目录的个数
        ls -l /home | grep "^d" | wc -l

    3.统计/home目录下包含子文件的个数
        ls -lR /home | grep "^-" | wc -l

    4.统计/home目录下包含子文件的个数
        ls -lR /home | grep "^d" | wc -l
        
    5.树状图显示/home目录
        ·yum install tree安装“tree”指令
        ·tree /home

## 第13章 Linux实操篇 网络配置

### 13.1 Linux网络配置原理图（含虚拟机）

                    NAT模式

    Linux                       Windows
    网卡：192.168.229.128 <-->  网卡1 -> vmnet8(虚拟网卡) 192.168.229.1
                                ↕
                                网卡2 -> 真实网卡 192.168.0.108 <- 网关 -> 连接外网

### 13.2 查看网络IP和网关

    VMWare → 编辑 → 虚拟网络编辑器 即可查看网络

    → NAT设置 即可查看网关

    ※VMnet8即对应了虚拟机的IP段

    ·查看Windows下VMnet8网络配置
        1.使用ipconfig指令查看
        2.界面查看 控制面板 → 网络和Internet

### 13.3 ping测试主机之间的连通性

### 13.4 Linux网络环境配置

    1.自动获取

        通过登录界面来设置

            系统 → 首选项 → 网络连接 → 编辑 → 自动连接 √ 应用即可

        ※Linux会在启动后自动获取IP，缺点是每次获取的IP地址可能不一样，不适用于服务器

    2.指定固定IP

        直接修改配置文件来指定IP，并可以连接到外网
        
        ·编辑 /etc/sysconfig/network-scripts/ifcfg-eth0 (网卡eth0的配置文件)

            DEVICE=eth0
            TYPE=Ethernet
            UUID=c6f69b11-a38c-4716-a4b8-c30034a6862a
            ONBOOT=yes                  ←指定启动时连接
            NM_CONTROLLED=yes
            BOOTPROTO=static            ←以静态方式获取IP
            DEFROUTE=yes
            IPV4_FAILURE_FATAL=yes
            IPV6INIT=no
            NAME="System eth0"
            IPADDR=192.168.229.128      ←IP地址
            GATEWAY=192.168.229.1       ←网关
            DNS1=192.168.229.1          ←DNS，与网关指定相同值即可
            HWADDR=00:0C:29:4D:35:47
            PEERDNS=yes
            PEERROUTES=yes
            LAST_CONNECT=1595852657

            补充说明：
                DEVICE  - 接口名（设备网卡）
                HWADDR  - MAC地址
                TYPE    - 网络类型，通常是Ethernet
                UUID    - 随机ID
                ONBOOT  - 系统启动时接口是否有效
                BOOTPROTO  - IP的配置方法
                             [none|static|bootp|dhcp]
                             [引导时不使用协议|静态分配IP|BOOTP协议|DHCP协议]
                IPADDR  - IP地址
                GATEWAY - 网关
                DNS1    - 域名解析器

        ·service network restart 重启网络服务

## 第14章 Linux实操篇 进程管理 ☆

### 14.1 进程的基本介绍

    1. 在Linux中，每个执行的程序都称为一个进程。每一个进程都分配一个ID号。

    

    2. 每一个进程都会对应一个父进程，而这个父进程可以复制多个子进程。

    3.进程可以以两种方式存在，前台与后台。
        前台就是指用户目前屏幕上可以进行操作的。
        后台进程则是实际在执行，但是屏幕上无法看到的进程。

    4.一般系统的服务都是以后台进程的方式存在，而且都会常驻在系统中，直到关机才结束。

### 14.2 显示系统执行的进程

    语法：
        ps [选项]  - report a snapshot of the current processes

    常用选项：
        -a 显示当前终端所有的进程信息
        -u 以便于阅读的方式显示进程信息
        -x 显示后台进程运行的参数

        ※添加 | grep xxx 来进行过滤

    各项说明：
        USER    用户名
        PID     进程编号
        %CPU    当前进程占用CPU的情况
        %MEM    当前进程占用内存的情况
        VSZ     占用虚拟内存的情况
        RSS     使用物理内存的情况
        TTY     使用的终端
        STAT    当前进程运行的状态
                （S： Sleep，s：进程是会话的先导进程，N：比普通优先级更低的优先级，
                 R: Run，Z：僵死进程，T：被跟踪或被停止等）
        START   启动时间
        TIME    占用CPU的总计时间
        COMMAND 进程启动时的命令行指令

    示例1：查看sshd服务

        ps -aux | grep sshd

    示例2：查看父进程

        ps -ef | grep 

        各项说明（BSD风格）：
            UID     用户ID
            PID     进程编号
            PPID    父进程编号
            C       CPU执行计算的优先级因子
                    数值越大，表明进程是CPU密集型运算，执行优先级会降低
                    数值越小，表名进程是I/O密集型运算，执行优先级会提高
            STIME   进程启动的时间
            TTY     使用的终端
            TIME    CPU时间
            CMD     启动进程时的指令

### 14.3 终止进程kill和killall

    介绍：

        若是某个进程执行到一半需要终止时，或是已经消耗了很大的系统资源时，可以考虑终止该进程。
        使用kill命令来完成此任务。

    语法：
        kill [选项] 进程号  - 通过进程号杀死进程
        killall 进程名称  - 通过名称杀死进程，也支持通配符。在系统因负载过大而缓慢时很有用。

    常用选项：
        -9 强制终止

    示例：

        1.踢掉非法登录的jack用户
            ps -aux | grep sshd
            找到jack的远程登录进程号3472

    root       2469  0.0  0.0  66288  1212 ?        Ss   19:28   0:00 /usr/sbin/sshd
    root       2820  0.0  0.1 102132  4172 ?        Ss   19:33   0:00 sshd: root@pts/0 
    root       3468  0.7  0.0 102132  4036 ?        Ss   20:06   0:00 sshd: jack [priv]
    jack       3472  0.5  0.0 102132  1928 ?        S    20:06   0:00 sshd: jack@pts/1 
    root       3498  0.0  0.0 103340   872 pts/0    S+   20:06   0:00 grep sshd

            kill 3472
        
        2.终止远程登录服务，在适当的时间重新启动它
            kill 2469
            之后将无法建立新的远程连接

        3.终止多个启动中的gedit编辑器
            killall gedit

        4.强制终止一个终端
            ps -aux | grep bash
            通过启动时间来找到想要杀掉的终端进程号

    root       2824  0.0  0.0 108564  1940 pts/0    Ss   19:34   0:00 -bash
    xh         3576  0.0  0.0 108352  1772 pts/1    Ss+  20:14   0:00 /bin/bash
    xh         3594  0.0  0.0 108352  1776 pts/2    Ss+  20:15   0:00 /bin/bash
    root       3610  0.0  0.0 103340   876 pts/0    S+   20:16   0:00 grep bash

            kill -9 3576

### 14.4 查看进程树

    语法：
        pstree [选项] 可以更加直观地看到父子进程关系

    常用选项：
        -p 显示进程的PID
        -u 显示进程所述用户

### 14.5 服务（Service）管理

    介绍：

        服务本质上就是一个进程，只不过是在后台运行。
        通常会监听某个端口，等待其他程序的请求，比如MySQL、sshd、防火墙等。
        因此我们又称其为守护进程，是Linux中非常重要的知识点。

    管理指令：
        serivce 服务名 [start|stop|restart|reload|status]

        ※在CentOS 7.0以后，service → systemctl

    示例：

        查看防火墙的状态（iptables）

        service iptables status

        ※通过telnet指令检查Linux的某个端口是否在监听
            DOS: telnet ip 端口
             （出现SSH...提示后表示端口可以连接）

### 14.6 查看服务名

    1.setup -> 系统服务 -> 按空格来启动或关闭

    2.查看/etc/init.d/目录下文件

    永久设置服务自启动

### 14.7 再说运行级别

    开机后的流程：
        开机 -> BIOS -> /boot -> init进程1 -> 从/etc/inittab获取运行级别 -> 运行对应服务

    介绍：

        每个服务对应每个运行级别都会设置是否自启动

    指令
        chkconfig --list  查看服务
            chkconfig --list | grep sshd
        chkconfig 服务名 --list  查看指令服务
        chkconfig --level 5 服务名 on/off  设置服务在指定级别下是否自启动
                                            （不指定level修改所有级别）

### 14.8 动态监控进程

    介绍：

        top和ps命令很相似，它们都用来显示正在执行的进程。
        不同的是top在执行一段时间之后可以更新正在执行的进程。

    语法：
        top [选项]

    选项说明：
        -d 秒数  指定top命令每隔几秒更新，默认3秒
        -i       使top不显示任何闲置或僵死进程
        -p       通过指定进程ID来仅仅监视某个进程的状态

    

    交互操作：
        P  按CPU使用率排序（默认）
        M  按内存使用率排序
        N  按PID排序
        q  退出
        u 用户名  监控某用户的进程
        k PID    杀死某进程

    top - 19:36:27 up 9 min,  1 user,  load average: 0.00, 0.06, 0.06
    当前时间      开机经过时间  用户数    负载均衡（均值超过0.7就算高负载）
    Tasks:   1 total,   0 running,   1 sleeping,   0 stopped,   0 zombie
    各任务总和
    Cpu(s):  0.0%us,  0.1%sy,  0.0%ni, 99.9%id,  0.0%wa,  0.0%hi,  0.0%si,  0.0%st
    CPU使用率   用户    系统             空闲
    Mem:   4039504k total,   395320k used,  3644184k free,    20120k buffers
    内存使用状态
    Swap:  2097148k total,        0k used,  2097148k free,   142088k cached
    虚拟内存使用状态
    PID USER      PR  NI  VIRT  RES  SHR S %CPU %MEM    TIME+  COMMAND                                     
    2465 root      20   0 66288 1212  476 S  0.0  0.0   0:00.01 sshd

### 14.9 查看系统网络情况 ☆

    语法：
        netstat [选项]

    常用选项：
        -an 按一定顺序排列输出
        -p  显示哪个进程在调用

    示例：

        1. 查看所有的网络服务

            netstat -anp | more

        2. 查看某一进程相关服务

            netstat -anp | grep sshd

## 第15章 Linux实操篇 RPM和YUM

### 15.1 RPM包的管理

    介绍：

        一种用于互联网下载包的打包及安装工具，它包含在某些Linux分发版中，生成. RPM扩展名的文件。
        RPM是Redhat Package Manager(红帽软件包管理工具)的缩写，类似Windows的setup.exe。

    简单查询指令：
        rpm -qa | grep xxx  查询已安装的rpm列表

        [root@hadoop1 ~]# rpm -qa | grep firefox
        firefox-52.8.0-1.el6.centos.x86_64          ← .rpm后缀名被省略了

        软件名 - 版本号  .适用的操作系统.系统位数（i686、i386表示32位，noarch表示通用）

        rpm -q 软件包名  查询包是否已安装

        [root@hadoop1 ~]# rpm -q firefox
        firefox-52.8.0-1.el6.centos.x86_64

        rpm -qi 软件包名  查询软件包详细信息

        rpm -ql | more 软件包名  查询软件包的安装路径和所有安装文件

        rpm -qf 文件路径  查询文件属于哪个安装包

        [root@hadoop1 ~]# rpm -qf /etc/passwd
        setup-2.8.14-23.el6.noarch

    卸载rpm包：
        rpm -e RPM包名

        细节：
            如果其他包依赖于删除对象包，则会提示
            removing these packages would break dependencies: 
                foo is needed by bar-1.0-1

            此时，可以使用rpm -e --nodeps foo可以删除（依赖包将无法使用）

    安装rpm包：
        rpm -ivh RPM包名

        参数说明：
            -i install 安装
            -v verbose 提示
            -h hash 进度条

        示例：
            演示安装firefox浏览器
                1)先找到firefox的安装包（使用CentOS安装盘的/media/下的安装包）
                    /media/CentOS_6.10_Final/Packages/
                2)拷贝安装包到/opt/目录下
                    cp firefox-52.8.0-1.el6.centos.x86_64.rpm /opt/
                3)来到/opt/目录下，进行安装
                    rpm -ivh firefox-52.8.0-1.el6.centos.x86_64.rpm

### 15.2 YUM包的管理

    介绍：

        Yum是一个Shell前端软件包管理器。基于RPM包管理，能够从指定的服务器自动下载RPM包并安装。
        可以自动处理依赖关系，并且一次性安装所有的依赖软件包。
        使用yum的前提是可以联网。

    基本指令：
        ·查询yum服务器是否有想要安装的软件
            yum list | grep xxx
        ·安装指定的yum包
            yum install xxx

            ※默认会安装最新版本

## 第16章 Linux之JavaEE定制篇 搭建JavaEE环境

### 16.1 概述

    Linux           |        Windows
                    |
    JavaEE          |           
                    |
    ·Jdk            |
    ·Tomcat     <------->    IE访问Web页面
    ·MySQL          |
    ·Eclipse        |

    ※讲解中都使用预先准备好的安装包进行安装

### 16.2 安装Jdk

    1.使用xftp5连接到远程机器，把准备好的软件上传到/opt/目录下
        ·jdk-7u79-linux-x64.gz
        ·eclipse-jee-mars-2-linux-gtk-x86_64.tar.gz
        ·apache-tomcat-7.0.70.tar.gz
        ·mysql-5.6.14.tar.gz

    2.解压缩到/opt
    3.配置环境变量vim /etc/profile
        JAVA_HOME=/opt/jdk1.7.0_79
        PATH=$PATH:$JAVA_HOME/bin  ※注意要带上$PATH:，不然只有PATH
        EXPORT JAVA_HOME PATH

        需要注销一次用户使环境变量生效（？）

    

    4. 在任何目录下使用java和javac测试是否成功

### 16.3 安装Tomcat

    1.解压缩到/opt
        tar -zxvf apache-tomcat-7.0.70.tar.gz
    2.进入tomcat的bin目录，启动start.sh
        （service tomcat start）
    3.编辑iptables，防火墙放行8080端口
        vim /etc/sysconfig/iptables
        -A INPUT -m state --state NEW -m tcp -p tcp --dport 8080 -j ACCEPT
