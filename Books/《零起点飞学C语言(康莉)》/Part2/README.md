## 第二章 C语言数据及数据运算

1.常量：在程序运算过程中不可更改的量。

---

2.变量：用标识符标识且在程序运行过程中允许被改变的量。

---

3.变量名实际上是一个符号地址。

---

4.extern：声明外部变量，以扩展外部变量的作用域。

如：在变量定义点之前的函数引用函数外部的变量。

---

5.整形：

- 整形常量：主要有int,long两种类型。

- 整形变量：int,short int,unsigned int,unsigned short,long,unsigned long


---

6.实型：

- 实型常量：实数或浮点数。

- 实型变量：单精度(float)，双精度(double)


---

7.字符型：

- 字符常量：用单引号括起来的一个字符。

- 字符串常量：用双引号括起来的字符序列。

- 字符变量：用来存放单个字符，占用一个字节的内存。


---

8.运算符：

赋值运算符：=

复合赋值运算符：+=,-=,*=,/=,%=


---

9.算术运算符：+,-,*,/,%


---

10.自增、自减运算，只针对变量。


---

11.关系运算符：<,<=,>,>=,==,!=


---

12.逻辑运处符：&&,||,!


---

13.条件运算符：条件?表达式1:表达式2


---

14.逗号表达式，取值为最后一个表达式的值。


---

15.scanf()函数：scanf(格式控制，输入项列表);


---

16.“*”符：用以表示该输入项读入后不赋予相应的变量，跳过该输入值。

scanf(“%d %*d %d”,&a,&b);

输入为：1,2,3时，把1赋予a,2被跳过,3赋予b.


---

17.getchar()函数：从键盘上输入一个字符，把输入的字符赋予一个字符变量。

---


18.printf()函数：格式化输出函数：printf(格式控制,输出项列表);


---

19.putchar()函数：字符输出函数，输出单个字符。
