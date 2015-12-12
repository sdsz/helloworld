#简介#

这个工程只是一个样例工程，用于向社团中的成员解释github的基本使用方法，所有计算机社的成员需要阅读这个工程并完成相关设置

#步骤#

我们要做的事情包括这几部：
 - 1.建立自己的github账户
 - 2.在计算机上安装git，并配置
 - 3.克隆这个工程
 - 4.在工程文件中添加自己的个人说明文件（或者说简介），并向github push

#说明#

在此之前，我们要先说明几点：
 - 1.在完成建立github账户后请先向系统维护组的成员告知自己的github账户
 - 2.建议先按照 https://github.com/racaljk/hosts 上的步骤配置hosts，方便网络的访问
 - 3.推荐使用linux操作系统

#建立github账户#

请在 https://github.com 上建立自己的账户

#安装Git#

首先在浏览器中打开：

> https://msys2.github.com

然后下载并安装
然后在安装后的msys2 shell中输入命令：

> pacman --needed -Sy bash pacman pacman-mirrors msys2-runtime

重启msys shell，输入

> pacman -Su

然后安装Git：

> pacman -S git

Git就安装完成了。

然后是默认配置VIM

首先用管理员模式打开shell，并输入：

> vim $HOME/.vimrc

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
