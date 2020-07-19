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

---

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

    4) Linux的吉祥物
        企鹅Tux
    
    5) Linux主要的发行版本
        ※Linux内核添加应用软件后构成一个发行版本

        ·CentOSE
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
