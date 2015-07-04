# go_misc_vim
golang 源码包里面的/misc/vim 配置文件


安装的话
先解压到你的一个你找得到的目录里面
首先你的~/.vimrc 要先打开支持语法高亮
vim ~/.vimrc
syntax on
set fencs=utf-8,gbk


1. mkdir ~/.vim
2. cp -R misc/vim/* ~/.vim/
3：新建~/.vim/ftdetect/go.vim,加入下面的内容：au BufRead,BufNewFile *.go set filetype=go
或者在命令行中运行如下：
     echo "au BufRead,BufNewFile *.go set filetype=go" > ~/.vim/ftdetect/go.vim
