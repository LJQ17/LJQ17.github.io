# ArchLinux的介绍及简易安装过程

本篇文章讲述如何在电脑上安装Arch Linux

## 0.关于Arch Linux
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;最初开始安装并使用Linux是在2019年初，当时觉得应该体验一下Linux，于是上网搜索哪种Linux发行版比较流行，最终发现名叫“Manjaro”的Linux发行版挺受欢迎的，于是安装并费劲的搞成双系统，大概用上了三个月，在一次神奇的重启后发现非root用户“消失了”，幸好重要的资料全在Windows的分区中...在后来的分析中我感觉可能还是自己的操作问题，**首先是在下游系统(Manjaro基于Arch)中使用了上游的软件(使用了Arch的软件源)可能导致的兼容问题，其次是在每一次滚动更新前没有做足功课(去官网阅读最新的更新是否有异常)**，但是总体上来说Manjaro的使用还是不错的，装在笔记本上续航不错，损耗小(风扇都不爱转了)，尽管那时用的还是机械硬盘，速度上也不是不能看，还有界面简洁(xfce桌面环境)。

后来2020年初因为配了台式电脑所以就又想着把老旧笔记本装成Linux...不过这次我做足了功课(现在看来并不)，直接选中的Manjaro的上游也就是本文的主题Arch Linux，由于Arch Linux并不自带桌面环境所以后来自己装了**深度桌面环境(DDE)**，非常的好用。虽然最后因为办公问题又装回了Windows...

接下来说一下[Arch Linux的特点](https://wiki.archlinux.org/index.php/Arch_Linux_(%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87))吧：<br>
1.KISS原则（保持简单和愚蠢），注重代码正确、优雅和极简主义，期待用户能够愿意去理解系统的操作。Arch Linux系统安装、删除和更新软件的软件包管理器叫做pacman。(百度百科)<br>
2.滚动更新:在使用Manjaro、Arch每天最快乐的就是使用“pacman -Syyu”的一键更新，无论是系统还是软件都更你更喽！但是要注意在更新前一定会要去官网看下公告(二次提醒)，如果出现更新异常的话会在公告上说明并提供解决方法的。(基本上吧)<br>
3. 解决依赖问题：使用pacman也可以在更新系统、软件的同时也会安装前置软件。<br>
4.强大的社区：有了社区的支持让Arch Linux无论是安装还是日常使用的问题都有很好的解决方式，而且现在中文的页面也有很多，软件的使用也说明的很详细，一些其他发行版的问题也可以在这里找到解决方法。<br>

尽管Arch现在已经有人称其为“邪教”了，但是在安装后会有种“这个操作系统都是我一行行代码敲出来的”的感觉。在安装完Arch后，你也会对Linux的一些基础知识有些了解。

## 1.在安装前需要知道的一些知识
首先对于一个软件、程序来说没什么比他的官网更能有说服力：<br>
中文官网: https://www.archlinuxcn.org/<br>
官网: https://archlinux.org/<br>
中文论坛: https://bbs.archlinuxcn.org/<br>
中文WIKI: https://wiki.archlinux.org/index.php/Main_page_(%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87)<br>
中文WIKI安装指南: https://wiki.archlinux.org/index.php/Installation_guide_(%E7%AE%80%E4%BD%93%E4%B8%AD%E6%96%87)<br>
论坛上的安装指南: https://bbs.archlinuxcn.org/viewtopic.php?id=1037 (2019年12月01日的，但是目前看来也适用)

硬件上的准备：<br>
Arch的安装是需要联网的，所以至少确保网络畅通，笔记本的话建议插上网线进行安装。<br>
由于官方不支持了32位系统，请确保机器是64位的。<br>
综上 保证机器为15年左右的即可。<br>

