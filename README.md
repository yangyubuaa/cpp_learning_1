### C++的编译和链接过程
---
##### 文件内容
main.cpp是程序执行入口
math1.cpp是程序执行调用的函数的实现文件
math1.h是math1的头文件，包含了math1中函数的定义

##### 编译过程
C++中每个文件可以分别进行编译和汇编过程，最终得到二进制文件，然后进行链接才可以执行，比如main.cpp可以单独执行编译过程，但是main.cpp中使用了math1.cpp的函数；math1.cpp也可以单独执行编译过程。编译完后我们通过链接生成可执行文件

##### 涉及命令
1. g++ -c xxx.cpp -o xxx.o	生成二进制文件
2. g++ xxx.o qqq.o sss.o -o a.out	生成可执行文件
