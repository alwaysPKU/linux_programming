本例创建一个小型函数库，它包含两个函数，然后在一个示例程序里调用其中一个函数。
这两个函数是fred和bill
1.为两个函数分别创建各自的源文件，fred.c和bill.c
2.分别编译这些函数，产生要包含在库文件中的目标文件。gcc -c 阻止编译器创建一个完整的程序
3.编写一个调用bill函数的程序。lib.h
4.调用程序program.c。要include "lib.h"
5.gcc -c program.c
  gcc -o program.o bill.o
6.执行./program
