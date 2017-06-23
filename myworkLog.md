# 2017年6月16日
>Linux 历史
>> 在1991年，林纳斯·托瓦兹开始在MINIX上开发Linux内核，为MINIX写的软件也可以在Linux内核上使用。后来使用GNU软件代替MINIX的软件，因为使用从GNU系统来的源代码可以自由使用，这对Linux的发展是有益。使用GNU GPL协议的源代码可以被其他项目所使用，只要这些项目使用同样的协议发布。为了让Linux可以在商业上使用，林纳斯·托瓦兹决定更改他原来的协议（这个协议会限制商业使用），以GNU GPL协议来代替。之后许多开发者致力融合GNU元素到Linux中，做出一个有完整功能的、自由的操作系统。

>> Linux的第一个版本在1991年9月被大学FTP server管理员Ari Lemmke发布在Internet上，最初Torvalds称这个内核的名称为“Freax”，意思是自由（“free”）和奇异（“freak”）的结合字，并且附上“X”这个常用的字母，以配合所谓的类Unix的系统。但是FTP服务器管理员嫌原来的命名“Freax”的名称不好听，把内核的称呼改成“Linux”，当时仅有10000行程序码，仍必须运行于Minix操作系统之上，并且必须使用硬盘开机；随后在10月份第二个版本（0.02版）发布，同时这位芬兰赫尔辛基的大学生在comp.os.minix上发布一则消息

>>Hello everybody out there using minix- I’m doing a (free) operation system (just a hobby, won’t be big and professional like gnu) for 386(486) AT clones.

>>1994年3月，Linux1.0版正式发布，Marc Ewing成立Red Hat软件公司，成为最著名的Linux经销商之一。

>>Unix & Linux历史源流
>>早期Linux的开机管理程序（boot loader）使用LILO（Linux Loader），早期的LILO存在着一些难以容忍的缺陷，例如无法识别1024柱面以后的硬盘空间，后来的GRUB（GRand Unified Bootloader）克服这些缺点，具有‘动态搜索内核文件’的功能，可以让用户在开机的时候，自行编辑开机设置系统文件，通过ext2或ext3文件系统中加载Linux Kernel（GRUB通过不同的文件系统驱动可以识别几乎所有Linux支持的文件系统，因此可以使用很多文件系统来格式化内核文件所在的扇区，并不局限于ext文件系统）。

>>Linux的标志和吉祥物是一只名字叫做Tux的企鹅，标志的由来是因为Linus在澳洲时曾被一只动物园里的企鹅咬了一口，便选择企鹅作为Linux的标志。更容易被接受的说法是：企鹅代表南极，而南极又是全世界所共有的一块陆地。这也就代表Linux是所有人的Linux。
***
# 2017年6月19日
>Linux基本命令的使用
1. cat：组合文件，将标准输入复制到标准输出

2.tee：将标准输入复制到文件和标准输出
3.xargs：使用来自标准输入的参数运行命令
## 命令工具
1. alias：创建/显示别名
2. type：定位命令：显示命令的路径名或别名
3. unalias：删除别名
4. whence：定位命令：显示命令的路径名或别名
5. which：定位命令：显示命令的路径名或别名
## 比较文件
1. cmp：比较两个文件
2. comm: 比较两个有序文件，显示区别
3. diff:比较两个文件，显示区别
4. sdiff:比较两个文件，显示区别
## 目录
1. cd:改变工作目录
2.chmod:改变文件或目录的文件权限
3.dirs:显示/清除目录栈中的内容
4.du:显示文件使用的磁盘空间量
5.file:分析文件的类型
6.ls:显示文件的各种类型的信息
7.mkdir:创建目录
8.mv:移动或重命名文件或目录
9.popd:改变工作目录，将名称从目录栈中弹出
10.pushd:改变工作目录，将名称压入到目录栈中
11.pwd:显示工作目录的路径名
12. rm:删除文件或目录
13. rmdir：删除空目录
14. tree：显示目录树的图表
## 显示数据
1. cat：组合文件，将标准输入复制到标准输出
2. echo:将参数写到标准输出
3.head:从数据的开头选择行
4.hexdump:显示二进制(非文本)文件
5.less:分页程序：每次一屏地显示数据
6.more:分布程序：每次一屏地显示数据
7.od:显示二进制(非文本)文件
8.print：将参数写到标准输出
9.tail：在数据的末尾选择行
# 2017年6月20日
>CGI程序
>>获取表单数据
```java
cgiFormResultType   cgiFormString(char *name, char *result, int max);
参数：  name, 指定要获取的表单项的名字
       result,将获得的数据存储到result中
       max， 指定最多读取的字符个数

比如： cgiFormString("name", result,  16);可以获得最多16个字符并且保存于result中
```
>>补充函数fprintf
```java
int fprintf(FILE *stream, const char *format, ...);
功能： 将格式化的语句输出到指定的流
fprintf(stdin, "helloworld\n")  等价于 printf("helloworld\n);
```
补充函数atoi
```java
int atoi(const char *nptr);
功能：将一个字符串转换成对应的数字，比如：“1234” ==》 1234
```
# 2017年6月21日
>设计mysql数据库
# 2017年6月22日
>整理文档
# 2017年6月23日
