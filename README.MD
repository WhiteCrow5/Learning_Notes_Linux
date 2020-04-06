* [一、常用指令](#%E4%B8%80%E5%B8%B8%E7%94%A8%E6%8C%87%E4%BB%A4)
  * [1、ls](#1ls)
  * [2、pwd](#2pwd)
  * [3、cd](#3cd)
  * [4、mkdir](#4mkdir)
  * [5、touch](#5touch)
  * [6、cp](#6cp)
  * [7、mv](#7mv)
  * [8、rm](#8rm)
  * [9、vim](#9vim)
  * [10、&gt; &gt;&gt;](#10-)
  * [11、cat](#11cat)
  * [12、df](#12df)
  * [13、free](#13free)
  * [14、head](#14head)
  * [15、tail](#15tail)
  * [16、less](#16less)
  * [17、wc](#17wc)
  * [18、date](#18date)
  * [19、cal](#19cal)
  * [20、clear / ctrl \+ l](#20clear--ctrl--l)
  * [21、|](#21)
  * [22、hostname](#22hostname)
  * [23、id](#23id)
  * [24、whoami](#24whoami)
  * [25、ps](#25ps)
  * [26、top](#26top)
  * [27、du](#27du)
  * [28、find](#28find)
  * [29、service](#29service)
  * [30、kill / killall](#30kill--killall)
  * [31、ifconfig](#31ifconfig)
  * [32、reboot](#32reboot)
  * [33、shutdown](#33shutdown)
  * [34、uptime](#34uptime)
  * [35、uname](#35uname)
  * [36、netstat](#36netstat)
  * [37、man](#37man)
* [二、Vim](#%E4%BA%8Cvim)
  * [1、打开文件](#1%E6%89%93%E5%BC%80%E6%96%87%E4%BB%B6)
  * [2、进入编辑模式](#2%E8%BF%9B%E5%85%A5%E7%BC%96%E8%BE%91%E6%A8%A1%E5%BC%8F)
  * [2、退出文件](#2%E9%80%80%E5%87%BA%E6%96%87%E4%BB%B6)
  * [3、光标的移动](#3%E5%85%89%E6%A0%87%E7%9A%84%E7%A7%BB%E5%8A%A8)
  * [4、修改操作](#4%E4%BF%AE%E6%94%B9%E6%93%8D%E4%BD%9C)
  * [6、搜索/查找](#6%E6%90%9C%E7%B4%A2%E6%9F%A5%E6%89%BE)
  * [7、替换](#7%E6%9B%BF%E6%8D%A2)
  * [8、其他](#8%E5%85%B6%E4%BB%96)
* [三、自有服务](#%E4%B8%89%E8%87%AA%E6%9C%89%E6%9C%8D%E5%8A%A1)
  * [1、运行模式](#1%E8%BF%90%E8%A1%8C%E6%A8%A1%E5%BC%8F)
  * [2、用户和用户组](#2%E7%94%A8%E6%88%B7%E5%92%8C%E7%94%A8%E6%88%B7%E7%BB%84)
  * [3、网络设置](#3%E7%BD%91%E7%BB%9C%E8%AE%BE%E7%BD%AE)
  * [4、ssh服务](#4ssh%E6%9C%8D%E5%8A%A1)
  * [5、修改主机名](#5%E4%BF%AE%E6%94%B9%E4%B8%BB%E6%9C%BA%E5%90%8D)
  * [6、chkconfig](#6chkconfig)
  * [7、ntp服务](#7ntp%E6%9C%8D%E5%8A%A1)
  * [8、防火墙](#8%E9%98%B2%E7%81%AB%E5%A2%99)
  * [9、rpm](#9rpm)
  * [10、cron](#10cron)
* [四、权限管理](#%E5%9B%9B%E6%9D%83%E9%99%90%E7%AE%A1%E7%90%86)
  * [1、chown](#1chown)
  * [2、chgrp](#2chgrp)
  * [3、sudo](#3sudo)
* [五、网络](#%E4%BA%94%E7%BD%91%E7%BB%9C)
  * [1、ping](#1ping)
  * [2、netstat](#2netstat)
  * [3、traceroute](#3traceroute)
  * [4、arp](#4arp)
  * [5、tcpdump](#5tcpdump)
* [六、shell](#%E5%85%ADshell)
* [七、MySQL](#%E4%B8%83mysql)
  * [1、软件安装](#1%E8%BD%AF%E4%BB%B6%E5%AE%89%E8%A3%85)
  * [2、软件初始化](#2%E8%BD%AF%E4%BB%B6%E5%88%9D%E5%A7%8B%E5%8C%96)
  * [3、库操作](#3%E5%BA%93%E6%93%8D%E4%BD%9C)
  * [4、表操作](#4%E8%A1%A8%E6%93%8D%E4%BD%9C)
  * [5、记录操作](#5%E8%AE%B0%E5%BD%95%E6%93%8D%E4%BD%9C)
  * [6、备份](#6%E5%A4%87%E4%BB%BD)
  * [7、还原](#7%E8%BF%98%E5%8E%9F)
  * [8、远程管理工具](#8%E8%BF%9C%E7%A8%8B%E7%AE%A1%E7%90%86%E5%B7%A5%E5%85%B7)
* [八、项目部署](#%E5%85%AB%E9%A1%B9%E7%9B%AE%E9%83%A8%E7%BD%B2)
  * [1、LAMP](#1lamp)

#### 一、常用指令

##### 1、ls

```
# list 列出当前工作目录下的所有文件和文件夹的名称
ls
ls -l  [path]		#以详细列表的形式显示
ls -a  [path]		#显示所有文件
ls -la [path]		#以详细列表的形式显示所有文件
ls -lh [path]		#以更加易读的方式显示出文件大小
```



##### 2、pwd

```
# print working directory 打印当前工作目录
pwd
```



##### 3、cd

```
# change directory 切换当前工作目录
cd [path]
cd .
cd ..		#返回到父目录
cd 			#切换到用户主目录
cd ~		#切换到用户主目录
cd / 		#切换到根目录
```



##### 4、mkdir

```
# make directory 创建目录
mkdir [path]
nkdir -p [path]	#实现多层一次性创建
```



##### 5、touch

```
# 创建文件
touch [file]
```



##### 6、cp

```
# copy 复制文件或文件夹
cp [src] [dest]
cp -r [src] [dest]	#递归处理，将指定目录下的所有文件与子目录一并处理
```



##### 7、mv

```
# move 移动、剪切
move [src] [dest]
```



##### 8、rm

``` 
# remove 移除、删除
rm [opt] [file]
rm -f [file]	#无需提示 force
rm -r [file]	#删除文件夹下的所有文件，需要一一确认
rm -rf [file]	#删除文件夹下的所有文件，无需提示
```



##### 9、vim

```
# 内置的文本编辑器
vim [file]
```



##### 10、> >>

```
# 输出重定向
[command] > [file]	#覆盖原先文件内容
[command] >> [file]	#原先文件内容末尾追加
```



##### 11、cat

```
# 查看文件内容
cat [file]

# 对文件进行合并
cat [file2] [file2] > [newfile]
```



##### 12、df

```
# 查看磁盘空间
df
df -h	以更加易读的方式显示存储空间
```



##### 13、free

```
# 查看内存情况
free
free -m	以MB为单位
free -g	以GB为单位
```



##### 14、head

```
# 查看文件的前n行 默认10
head -n [file]
```



##### 15、tail

```
# 查看文件的后n行 默认10
tail -n [file]
tail -f [file]	查看一个文件的动态变化，一般用于查看系统日志
```



##### 16、less

```
# 查看文件，以较少的内容输出，可以使用辅助功能键
less a	#空格键向下翻页 B键项上翻页 上下键移动一行，回车向下移动一行
```



##### 17、wc

```
# 统计文件内容信息
wc -l [file]	#行数
wc -w [file]	#单词数
wc -c [file]	#字节数
```



##### 18、date

```
# 表示操作时间和日期
date						#2020年 03月 22日 星期日 17:31:25 CST(当地时间)
date +%F 					#2020-03-22
date "+%Y-%m-%d"			#2020-03-22
date "+%F %T"				#2020-03-22 17:40:20
date "+%Y-%m-%d %H:%M:%S"	#2020-03-22 17:40:20
date -d "-1 day" "+%F %T"	#2020-03-21 17:40:20
```



##### 19、cal

```
# 用来操作日历
cal		#查看当前月份的日历(第一天是周日)
cal -3	#查看上一个月+本月+下一个月的日历
cal -y	#查看本年的日历
cal -m	#查看当前月份的日历(第一天是周一)
```



##### 20、clear / ctrl + l

```
# 清空终端显示内容
clear
ctrl + L
```



##### 21、|

```
# 管道一般可用于“过滤”，“特殊”，“扩展处理”
ls | grep a		#过滤出所有包含a字符的内容
```



##### 22、hostname

```
# 操作服务器主机名
hostname 		#输出完整的主机名
hostname -f		#输出当前主机名中的FQDN(Fully Qualified Domain Name全限定域名)
```



##### 23、id

```
# 查看用户的基本信息(用户id，用户组id，附加id...)
id				#显示当前用户信息
id [username]	#显示指定用户信息

"""
验证用户信息 		/etc/passwd
验证用户组信息		/etc/group
"""
```



##### 24、whoami

```
# 显示当前登录的用户名，一般用户shell脚本，一般用户获取当前操作的用户名，用于记录日志
whoami
```



##### 25、ps

```
# 用户查看当前服务器的进程信息
ps
ps -e	#列出全部进程
ps -f	#显示全部的列
ps -ef | grep [processname] #搜索指定进程
```



##### 26、top

```
# 查看服务器进程占的资源
top		#动态显示
	M	#将结果按照内存使用从大到小的顺序排列
	P	#将结果按照CPU使用从大到小的顺序排列
```



##### 27、du

```
# 查看目录的大小
du
du -s	#summary 显示汇总的大小
du -h	#以更可读的方式显示大小
```



##### 28、find

```
# 查找文件
find [path] [opt] [value]
find -name [file]	#按照文件名搜索
find -type f	#搜索文件
find -type d	#搜索文件夹
```



##### 29、service

```
# 用于控制一些软件的服务，启动/停止/重启
servive [服务名] start/stop/restart
```



##### 30、kill / killall

```
# 杀死进程
kill [PID]
killall [processname]
```



##### 31、ifconfig

```
# 用于操作网卡的相关指令
ifconfig
```



##### 32、reboot

```
# 重新启动计算机
reboot		#立即重启
reboot -w	#模拟重启，将重启写入日志
```



##### 33、shutdown

```
# 关机
shutdown -h now 	#立即关机
shutdown -h [time]	#定时关机
shutdown -c 		#取消关机
```



##### 34、uptime

```
# 输出计算机的持续在线时间
uptime
```



##### 35、uname

```
# 获取操作系统名称
uname
uname -a	#获取所有信息
```



##### 36、netstat 

```
# 查看网络连接状态
netstat	
netstat -t	#只列出tcp协议的连接
netstat -n	#列出ip地址+端口
netstat -l	#过滤出state列中值为Listen的连接
netstat -p	#显示出PID值
```



##### 37、man

```
# manual 帮助手册
man [command]	#查看命令帮助，按q退出
```



#### 二、Vim

##### 1、打开文件

```
# 打开文件
vim [filepath]
# 打开指定的文件，并把光标移动到指定行
vim [+number] [filename]
# 打开指定的文件，并且高亮显示关键词
vim [+/keywords] [filepath]
# 同时打开多个文件
vim [filepath1] [filepath2] [filepath3]...
```



##### 2、进入编辑模式

```
# 在光标所在字符前开始插入
i
# 在光标所在字符后开始插入
a
# 在光标所在行的下面另起一新行插入
o
# 在光标所在行的行首还是插入，行首有空格则在空格之后插入
I
# 在光标所在行的行尾开始插入
A
# 在光标所在行的上面另起一行插入
O
# 删除光标所在行并开始插入
S
```



##### 2、退出文件

```
# 进入末行模式
:
# 退出末行模式
Esc 
# 退出
:q(quit)
# 保存
:w(write)
# 另存为
:w [path]
# 强制退出
:q!
# 保存退出(若无修改，文件修改时间不会被修改)
:x
# 保存退出(文件修改时间会被更改)
:wq
```



##### 3、光标的移动

```
# 移动到行首
shift + 6	或者	^
# 将光标移动到行尾
shift + 4	或者	$
# 光标移动到首行
gg
# 光标移动到末行
shift + g	或者	G
# 向上翻页
ctrl + b(back)	或者	PgUp
# 向下翻页
ctrl + f(forward)		或者	PgDn
# 移动指定行/列数
[number] + 方向键
# 移动到指定行
:[number]	
```



##### 4、修改操作

```
# 复制number行
[number]yy
# 可视化复制
ctrl + v	-->	方向键移动选中需要复制区块	-->	yy
# 粘贴
p(paste)

# 剪切/删除光标所在行（删除后下一行上移）
dd	
# 剪切/删除所在行光标之后的内容
shift + d	或者 D
# 剪切/删除光标所在行及下一行
dd 方向下键
# 剪切/删除光标所在行及上一行
dd 方向上键

# 撤销
u(undo)
#恢复
ctrl + r
```



##### 6、搜索/查找

```
# 进入末行模式
/[keywords]	按N/n切换上/查找的内容
# 取消高亮
:nohl(nohighlight)
```



##### 7、替换

```
# 替换光标所在行搜索到的第一个内容
:s/[old]/[new]
# 替换光标所在行搜索到的全部内容
# 替换每一行搜索到的第一个内容
:%s/[old]/[new]
# 替换每一行搜索到的全部内容
:%s/[old]/[new]/g
```



##### 8、其他

```
# 显示行号
:set nu
# 取消显示
:set nonu
# 查看当前打开的所有文件名称	%a表示当前打开的文件	#表示上一个打开的文件
:files
# 切换文件
:open [filename]
# 切换到下一个文件
:bn
# 切换到上一个文件
:bp
# 代码着色（默认开启）
:syntax on
# 取消代码着色
:syntax off
# 使用计算器
编辑模式 --> crtl + R --> =
# 文件加密
:X
```



#### 三、自有服务

##### 1、运行模式

```
# 修改运行模式为命令行模式
vim etc/inittab	-->	3
```



##### 2、用户和用户组

```
# 存储用户的关键信息
/etc/passwd
# 存储用户组的关键信息
/etc/group
# 存储用户的密码信息
/etc/shadow

# 添加用户，同时创建同名的home目录和用户组
useradd [option] [username]
	-g	指定用户的用户主组，可以是ID或组名
	-G	指定用户的用户附加组，可以是ID或组名
	-u	自定义uid，系统默认从500之后开始分配uid
	
# 修改用户
usermod [option] [username]
	-g	指定用户的用户主组，可以是ID或组名
	-G	指定用户的用户附加组，可以是ID或组名
	-u	自定义uid，系统默认从500之后开始分配uid
	-l	修改用户名

# 设置密码
passwd [username]

# 删除用户
userdel [username]
	-r	删除用户的同时删除家目录
	
# 切换用户
su [username]

# 添加用户组
groupadd [option] [groupname]
	-g	选择自己设置一个自定义的用户组ID数字，默认500开始
	
# 用户组编辑
groupmod [option] [groupname]
	-g	选择自己设置一个自定义的用户组ID数字
	-n	设置新的用户组名称
	
# 用户组删除
groupdel [groupname]
```



##### 3、网络设置

```
# 网卡配置路径
/etc/sysconfig/network-scripts

# 各种快捷方式路径
/etc/init.d

# 创建快捷方式
ln -s [originpath] [shortcutpath]

# 重启所有网卡
service network restart
/etc/init.d/network restart

# 关闭某个网卡
ifdown [networkname]

# 开启某个网卡
ifup [networkname]
```



##### 4、ssh服务

```
# 配置文件所在路径
/etc/ssh/ssh_config
/etc/init.d/sshd

# 启动/停止/重启
service sshd start/stop/restart

# 软件
Xshell、SecureCRT、PuTTY、FileZilla、PSCP
```



##### 5、修改主机名

```
# 查看主机名
hostname
hostname -f(FQDN、全限定域名)

# 临时修改主机名
hostname [newname]
# 永久设置主机名（需要重启）
/etc/sysconfig/network
# 修改linux服务器的hosts文件，设置FQDN
/etc/hosts
```



##### 6、chkconfig

```
# 开机启动服务查询(0-6对应开机级别)
chkconfig --list

# 删除服务
chkconfig --del [servicename]

# 添加服务
chkconfig --add [servicenameche]

#设置服务在某个级别下开启或关闭
chkconfig --level 35 [servicenameche] on/off
```



##### 7、ntp服务

```
# 主要是用于对计算机的时间同步管理操作
# 手动同步
ntpdate [ip] 

# 启动ntpd服务自动同步
service ntpd start
/etx/init.d/ntpd start
chkconfig --level 35 ntpd on
```



##### 8、防火墙

```
# 开启/关闭/重启防火墙
service iptables start/stop/restart
/etc/init.d/iptables start/stop/restart

# 查看防火墙状态
service iptables status

# 查看规则
iptables -L -n

# 置防火墙 
iptables -A INPUT -p tcp --dport 80 -j ACCEPT	#允许访问80端口
/etc/init.d/iptables save	#将防火墙规则保存到/etc/init.d/iptables
```



##### 9、rpm

```
# 查询所有安装的软件
rpm -qa		

# 卸载软件（存在依赖关系时，不能被卸载）
rmp -e [software]

# 强制卸载软件
rpm -e [software] --npdeps

# 安装软件
rpm -ivh [path]

# 查看块状设备的信息
lsblk

# 解挂操作
umount [path]

# 挂载光盘(原始路径均在 /dev/ 下)
mount [device origin path] [mount path]
```



##### 10、cron

```
# 计划任务
crontab [option]
	-l	#list, 列出指定用户的计划任务列表
	-e	#edit, 编辑指定用户的计划任务列表
		#分(0-59) 时(0-23) 日(1-31) 月(1-12) 周(0-6) 命令	
		#*(所有数字) -(做区间) /(每/个) ,(多个取值)
		0 0 * * * * reboot
		* * * * * date+"%F %T" >> /root/rt.txt
	-u	#user， 指定的用户名，不指定则表示当前用户
	-r	#remove， 删除指定用户的计划任务列表
	
# 黑名单配置文件
/etc/cron.deny

# 白名单配置文件（优先级高于黑名单）
/etc/cron.allow
```



#### 四、权限管理

```
# owner、group、others
# read、write、execute
读权限：
	对于文件夹：读权限影响用户是否能够列出目录结构
	对于文件：读权限影响用户是否可以查看文件内容
写权限：
	对于文件夹：写权限影响用户是否能够创建/删除/复制到/移动到文档
	对于文件：写权限影响用户是否可以编辑文件
执行权限：
	对于文件：执行权限影响用户是否可以执行文件

# 查看权限
ls -l [path]
ll

# 设置权限（仅root或owner可用）
chmod [option] [model] [document]
	-R: 递归设置权限（选项）
	-u: 所有者身份
	-g:	给所有者同组用户设置
	-o:	给其他用户设置权限
	-a: 给所有人设置权限
	-+:	增加权限
	--:	减少权限
	-=:	确定权限
	-r:	可读
	-w:	可写
	-x:	执行
chmod u+x, g+rx, o+r [filename]
chmod u=x, g=rx, o=r [filename]
chmod a=--- [filename]

# 数字权限 r=4, w=2, x=1，尽量不要出现2和3
chmod 777 [filename]

# 使用root用户创建文件夹，权限默认为 drwxr-xr-x
# 在Linux中，如果要删除一个文件，不是看文件有没有对应的权限，而是看文件所在目录有没有写权限
```



##### 1、chown

```
属主：所属的用户
属组：所属的用户组
# 更改文档的所属用户
chown -R [username] [document]
# 更改文档的所属用户和所属用户组
chown -R [username:groupname] [document]
```



##### 2、chgrp

```
# 更改文档的所属用户组
chgrp -R [groupname] [path]
```



##### 3、sudo

``` 
# 配置
visudo 

# 给某个用户增加命令权限
test ALL=(ALL) [commandPath]

# 查询特殊权限
sudo -l
```



#### 五、网络

##### 1、ping

```
# 检测当前主机与目标主机之间的连通性
ping www.baidu.com
```



##### 2、netstat

```
# 查看网络连接信息
netstat
netstat -tnlp
netstat -an
```



##### 3、traceroute

```
# 查找当前主机与目标主机之间所有的网关
traceroute www.baidu.com
```



##### 4、arp

```
# 地址解析协议（Address Resolution Protocol）根据IP地址获取MAC地址的协议
# 查询地址
arp -a
# 删除缓存地址
arp -d
```



##### 5、tcpdump

```
# 用来抓包
tcpdump [protocol] [port]
tcpdump [protocol] [port] [host]
tcpdump -i [networ]
```



#### 六、shell

```
# Linux中shell的位置，bash(Bourne shell)
/bin/bash

# 修改shell解释器，用户不能登录
usermod -s /sbin/nologin [username]

代码规范：
#!/bin/bash		指定告知系统当前这个脚本要使用的shell解释器

文件命名规范：
文件名.sh

输出的内容包含字母和符号，则需要用引号包括起来。纯数字可包可不包
#-------tese.sh-------#
#!bin/bash
echo "hello world"
#---------------------#

执行：
chmod +x test.sh
./test.sh
或者
chmod +x test.sh
/bin/bash test2.sh

#变量定义，变量名等号左右不能有空格，双引号能够识别变量，单引号不能
class_name="white"

#变量使用，变量的使用必须在变量名前面加上$符号
echo $class_name

#只读变量
readonly [variable name]

#获取输入
read -p [tip message] [variable name]

#删除变量
unset [variable name]

#条件语句
if[condition];then command; fi

if condition
then
	command1
	command2
	...
fi

if condition
then 
	command1
	command2
	...
else
	command
fi

if condition
then
	command1
elif condition
then
	command2
else
	command...
fi

#算术运算符(借助expr工具)
val=`expr $a + $b`

#关系运算符
$a -eq $b
$a -ne $b
$a -gt $b
$a -lt $b
$a -ge $b
$a -le $b

#逻辑运算符
!false
$a -o $b
$a -a $b

#字符串运算符
$a = $b
$a != $b
-z $a	#判断字符串长度是否为0，为0返回true
-n $a	#判断字符串长度是否为0，不为0返回true

#文件测试运算符
-b $file	#是否为块设备文件，是返回true
-c $file	#是否为字符设备文件，是返回true
-d $file	#是否为目录，是返回true
-f $file	#是否为普通文件
-p $file	#是否为有名管道
-r $file	#是否为可读
-w $file	#是否为可写
-x $file	#是否为可执行
-s $file	#检测文件是否为空
-e $file	#检测文件（目录）是否存在

#附带选项
$1 $2	#第一个输入参数 第二个输入参数
```



#### 七、MySQL

##### 1、软件安装

```
#源码包 安装ncurses
#解包
tar -zxvf filename.tar.gz
tar -jxvf filename.tar.bz2
	-z、 --gzip、 --ungzip	#通过gzip指令处理文件
	-x、--extract、--get		#从文件中还原文件
	-v	#显示操作过程
	-f、--file	#指定一个文件
	-j	#支持bzip2解压文件
	
#配置(config/configure/bootstrap) --> 编译(make/bootstrap) --> 安装(make install/bootstrapd install)

--prefix=path	#指定安装路径
--with-PACKAGE=包所在路径	#需要依赖的路径
--without-PACKAGE

./configure --prefix=/usr/local/ncurses
make && make install

#二进制包 安装lynx
rpm -qa | grep keywords
rpm -e keywrods [nodeps]
rpm -ivh path
rpm -Uvh path
rpm -qf path	#查询指定文件属于哪个包
	
#yum
yum list
yum search
yum [-y] install path
yum [-y] update
yum [-y] remove

yum install mysql
```



##### 2、软件初始化

```
#启动mysqld	默认3306端口
service mysqld start

#初始化
mysql_secure_installation

#进入mysql
mysql -u username -p password

#退出
exit
```



##### 3、库操作

```
#显示数据库
SHOW DATABASES;

#创建数据库
CREATE DATABASE 库名;

#删除数据操
DROP DATABASE 库名;

#使用数据库
USE	库名;
```



##### 4、表操作

```
#显示表
show tables;

#创建表(varchar char int)
create table 表名
(
列名1 数据类型[NOT NULL AUTO_INCREMENT],
列名2 数据类型,
列名3 数据类型,
...,
primary key
);

#查看表结构
desc 表名;

#删除表
drop table 表名;
```



##### 5、记录操作

``` 
#增
INSERT INTO [TABLENAME] VALUES (V1,V2,V3,...);
INSERT INTO [TABLENAME](COL1, COL2,...) VALUES (V1,V2,V3,...);

#改
UPDATE [TABLENAME] SET COL1 = [NEWVALUE] WHERE COL=VALUE;

#查
SELECT COL1, COL2... FROM [TABLENAME] WHERE [CONDITION]

#删
DELETE FROM [TABLENAME] WHERE COL=VALUE
```



##### 6、备份

```
#全量备份（数据+结构）
mysqldump -uroot -proot -A > newpath
#指定库备份（数据+结构）
mysqldump -uroot -proot 库名 > newpath
#多个库备份（数据+结构）
mysqldump -uroot -proot --databases db1 db2 > newpath
```



##### 7、还原

```
#还原全部数据库
mysql -uroot -proot < path
mysql> source path

#还原单个数据库(指定数据库)
mysql> use 库名
mysql> source path

#设置mysql连接字符集
mysql> set names utf8
```



##### 8、远程管理工具

```
#C/S结构软件：navicat
```



#### 八、项目部署

##### 1、LAMP

```
# linux + apache + mysql + php

#安装php
yum stall php

#启动apache
service httpd start
```

