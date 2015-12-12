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
