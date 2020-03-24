



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
```



