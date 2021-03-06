# IMPORTANT NOTES

From now on `sdsz` will be an organization instead of a personal account. Check your notifications inside GitHub and accept the invitations. To get into the organization ask for Owners to invite you.


# 简介

这个工程只是一个样例工程，用于向社团中的成员解释github的基本使用方法，所有计算机社的成员需要阅读这个工程并完成相关设置

# 步骤

我们要做的事情包括这几部：
 - 1.建立自己的github账户
 - 2.在计算机上安装git，并配置
 - 3.克隆这个工程
 - 4.在工程文件中添加自己的个人说明文件（或者说简介），并向github push

# 说明

在此之前，我们要先说明几点：
 - 1.在完成建立github账户后请先向系统维护组的成员告知自己的github账户
 - 2.建议先按照 https://github.com/racaljk/hosts 上的步骤配置hosts，方便网络的访问 **Removed previously added hosts from [here](https://github.com/racaljk/hosts) as it's against the `MIT` license**
 - 3.推荐使用linux操作系统

# 建立github账户

请在 https://github.com 上建立自己的账户

# 安装Git

首先在浏览器中打开：

    https://msys2.github.com

然后下载并安装
然后在安装后的msys2 shell中输入命令：

    pacman --needed -Sy bash pacman pacman-mirrors msys2-runtime

重启msys shell，输入

    pacman -Su

然后安装Git：

    pacman -S git

Git就安装完成了。

然后是默认配置VIM

首先用管理员模式打开shell，并输入：

    vim $HOME/.vimrc

在打开的文档中按i(插入模式)

输入：

```
"语法高亮
syntax on
syntax enable

"自动缩进
set ai
set ts=4
set sts=4
set sw=4

"设置回格键
set backspace=indent,eol,start

"启用鼠标
set mouse=a
set selectmode=mouse,key

"显示行号
set nu
```

下面是vim的一些基本用法：
 - 按i表示启用插入模式（正常输入）
 - 在插入模式按<Esc>进入命令模式
 - 在命令模式下输入 :w 表示保存
 - 在命令模式下输入 :q 表示退出
 - 在命令模式下输入 :wq 表示保存并退出
 - 在命令模式下输入 :q! 表示强制退出（不保存）
 - 在命令模式下输入 :e 表示重新加载，如果要放弃当前更改请输入 :e!
 - 在命令模式下按 数字 + G 表示转到那一行
 - 在命令模式下按 u 表示撤销一步
 - 在命令模式下按 dd 表示删除当前行
 - 在命令模式下按 数字 + 命令（u/d/其他） 表示做这么多步这一命令
 - 在命令模式下按 p 表示粘贴
 - 在命令模式下按 o 表示在本行之后新建一个空行
更多vim命令可以在网上自行搜索
  
如果同学觉得上述操作太复杂，可以直接从github官网下载github desktop来解决这个问题

# 配置Git

在命令行中输入:

    git config --global user.name "你的github用户名"

    git config --global user.email "你的github注册邮箱"

# 克隆工程

在命令行中找到一个常用的工作目录，输入：

    git clone http://github.com/sdsz/helloworld.git

解释一下这行命令：
首先一个git，这是运行git的命令，clone表示我们要做的操作是克隆，后面跟的是代码仓库的地址，我们的工程的地址大概是这个样子的：
http://github.com/建立仓库的用户名/项目名称.git

成功后你就可以在当前目录里找到一个叫做"helloworld"的子目录，这就是这个项目的工作目录了

# 修改并push

在修改工作目录中的文件后（修改、新建、删除），在命令行中输入:

    git status

可以查看当前文件的状态，如果有更改了却没有添加到监视中的文件可以在命令行中输入:

    git add <文件名>

或

    git add .

来添加所有文件的监视，当工程有更改时，输入:

    git commit

然后会进入一个文档，在不以"#"开头的行中可以添加说明，即对更改的说明，然后保存并退出(:wq)，之后再输入:

    git status

此时就已经没有更改了，但在网络上并没有变化，这时我们需要在命令行中输入:

    git push

然后输入你的用户名和密码就可以了，如果遇到冲突，可以尝试:

    git pull

如果遇到有不太清楚的问题，可以在命令行中输入:

    git help <命令>

以查看命令的具体帮助，或可以咨询维护组的同学，如果还不能解决，也可以上网查找

# Test if everyone has got the access to git

After you have followed the steps above, please make change in `README.md` in this section in the format below:

`<NAME(Pinyin accepted)       <DATE       <USERNAME OR EMAIL ON GITHUB>`

______

Xu Pengcheng	2015-12-19	xubin990510@126.com  
Jin Yueqi	2015-12-19	Sprjdfn jinyueqi1616@hotmail.com  
Jiang Lin	2015-12-19	jianglin332


