# Linux 学习日志
## 2026-10-14
- 学习了markdown的基本内容
## 2026-10-15
### shell and bash
- bash作为最常用的shell,是乌班图的解释器，用于直接编译命令行
- 命令提示符，由用户名@主机名:当前工作目录$命令组成，其工作核心是表示shell已经准备好接收下一条命令了
### echo  复读机
### sleep 数字
- 系统休息几秒，几秒后才会弹出下一条命令提示符
### ctrl c
- 强行终止运行，无需跟在命令提示符后，可直接输入
### ctrl l or clear  清屏
### tab
-自动填充，要打echo四个字母，可以选择打出ech，再按一下tab就可以自动补全，如果无法补全，则意味着有多个选项，连续按两次tab，就可以显示所有备选项
### home and end and ctrl </> 
- home  快速移动到命令的开头处
- end  快速移动到命令的结尾处
- ctrl <  向左快速移动一个单词，按照单词平移，只有<的话就是移动一个字母
- ctrl >  反之
### ctrl insert  复制；shift insert  粘贴
### cd  进入某个文件夹
### ls  展示当前文件夹下的所有文件
### rm  删除
- rm -rf  删除文件夹及文件夹内的所有文件
### .. and .
- ..  代指上一级的文件夹
- .  代指这一级的文件夹
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
