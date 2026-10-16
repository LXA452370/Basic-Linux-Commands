# Linux 学习日志
## 2026-10-14
- 学习了markdown的基本内容
## 2026-10-15
### shell and bash
- bash作为最常用的shell,是乌班图的解释器，用于直接编译命令行
- 命令提示符，由用户名@主机名:当前工作目录$命令组成，其工作核心是表示shell已经准备好接收下一条命令了
### echo
- 复读机
### sleep 数字n
- 系统休息n秒，几秒后才会弹出下一条命令提示符
### ctrl c
- 强行终止运行，无需跟在命令提示符后，可直接输入
### ctrl l or clear
- 清屏
### tab
-自动填充，要打echo四个字母，可以选择打出ech，再按一下tab就可以自动补全，如果无法补全，则意味着有多个选项，连续按两次tab，就可以显示所有备选项
### home and end and ctrl </> 
- home  快速移动到命令的开头处
- end  快速移动到命令的结尾处
- ctrl <  向左快速移动一个单词，按照单词平移，只有<的话就是移动一个字母
- ctrl >  反之
### ctrl insert and shift insert
### cd
- 进入某个文件夹
### ls
- 展示当前文件夹下的所有文件
### .. and .
- ..  代指上一级的文件夹
- .  代指这一级的文件夹
## 2026-10-16
### ll and ls -aLF
- ll
    - 第一行为total * 表示当前列出的内容占据的磁盘块大小，单位是1MiB/磁盘块
    - 形如：drwxr-xr-x 3 lxa060120 lxa060120  4096 Mar 19  2026 .local/
    - 文件的类型和权限 硬链接数量 所有者 所属组 文件大小（字节） 最后修改日期 文件名
- ls -aLF
    - -a 该目录下所有的隐藏内容，即用.开头的内容
    - -L 以详细列表形式打印
    - -F 在文件名后展示类别指示符
- 注明：乌班图系统下ll和ls -aLF不相同
### pwd
- 打印当前的目录
### cat
- 猫眼
- cat a.txt 可以直接在shell上显示纯文本文件的内容，但要避免过大的文件
- cat a.txt b.log c.txt 可以连续显示多个文件的内容
### mkdir
- mkdir aaa bbb ccc 在当前目录下创建一个或多个文件夹
- mkdir home/ABC/abc 按照目录创建文件夹
- mkdir -p aaa/bbb/ccc 父文件夹不存在时，创建多级文件夹
### rm
- rm aaa.txt bbb.log ccc.c删除一个或多个文件
- rm -rf  aaa bbb ccc 删除一个或多个文件夹及文件夹内的所有文件，慎用！
### touch
- touch dir_a dir_b dir_c 创建一个或多个空文件，什么都没，也没后缀
### find
- find 目录 检索条件
- 按照递归检索的方式层层寻找目标文件，输出路径，目录和检索条件越详细，找得越快
- 如：find text 查找该目录下所有文件的路径并输出
- 检索条件如下
    - -name 按照名称查找
    - -iname 按照名称查找且不区分大小写
    - -type f 只查找普通文件
    - -type d 只查找目录
    - -maxdepth n 往下最多查找n层
    - 注："*.txt"指的是查找以txt为后缀的文件，*是通配符
 
- 
### vim
- 指令vim打开编辑器，显示编辑器的相关信息，如版本号
    - vim分为三种模式：命令模式command mode；插入模式insert mode
    - command mode 可通过a i o A I O几个按键变为insert mode，通常只使用i
- vim 文件名
    - 可打开相关的文件，如果没有这个文件就会直接创建，如：vim hello.c；vim Hello.txt
    - 打开后，左下角会显示当前的文件名，如："Hello.txt" [new]，new意味着新文件
- :wq保存并退出
- :q!不保存，强制退出
- :q未修改，直接退出
