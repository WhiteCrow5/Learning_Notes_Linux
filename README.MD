#### 常用指令

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
ls | grep a		#输出所有包含a字符的内容
 
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
```



24、