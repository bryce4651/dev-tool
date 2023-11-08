# dev-tool

 ## tree
1. 取消注释
```
# Uncomment for OS X:
# It is not allowed to install to /usr/bin on OS X any longer (SIP):
#CC=cc
#CFLAGS+=-O2 -Wall -fomit-frame-pointer -no-cpp-precomp
#LDFLAGS+=
#MANDIR=${PREFIX}/share/man

# Uncomment for OS X:
# It is not allowed to install to /usr/bin on OS X any longer (SIP):
CC=cc
CFLAGS+=-O2 -Wall -fomit-frame-pointer -no-cpp-precomp
LDFLAGS+=
MANDIR=${PREFIX}/share/man
```
2. 给tree命令的现实结果增加颜色显示。
```
进入 tree.c 文件，找到以下这一行代码。
  setlocale(LC_CTYPE, "");
在 setlocale(LC_CTYPE, ""); 这行代码的前面加上
  force_color=TRUE;
保存并退出。
```
3. 编译安装
```
$ cd tree-1.7.0
$ make
$ cp tree ~/go/bin/
```


## aircrask-ng
/opt/homebrew/Cellar/aircrack-ng/1.7_1
