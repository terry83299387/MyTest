# MyTest
该项目用来存放我的测试程序。其中：

* `FloatTest.java`展示了一个由浮点数精度而导致计算出错的问题。详见程序内的注释。<br>
详见：http://www.cnblogs.com/antineutrino/p/4525224.html

* `Fibonacci.java`展示了一种计算超大数`Fibonacci`数列（不超过`2005`位`10`进制数）的方法。<br>
<br>
问题定义：
<br>
已知
<br>
`f(1)=f(2)=f(3)=f(4)=1`
<br>
当`n>4`时<br>
`f(n)=f(n-1)+f(n-2)+f(n-3)+f(n-4)`
<br>
给定正整数`n`，求`f(n)`（结果大小不超过`2005`个`10`进制位）。
<br>
<br>
由于涉及到超大数运算，所以无法直接使用编程语言内置的整数类型来计算。一种方法是使用字符串来保存数值，然后自己写运算算法。<br>
本程序使用另一种方法。将超大数用一个长整形（`long`）数组来表示，并实现相应的加法运算。<br>
由于`Java`中没有无符号整数类型，并且每个部分在运算时需要至少保留一位用来作为进位，否则将无法得到正确的结果。<br>
程序中，对数组中的每个长整型元素，只使用其中的`56`位来保存数值，第`57`位作为进位位，最高位的`7`位则没有使用。

* `BinaryTreeMinSum.java`是一个寻找二叉树最小和的程序。问题来自segmentfault：http://segmentfault.com/q/1010000003853178。<br>
详见程序内的注释。

* `DoubleToString.c`用来将浮点数转化为字符串，最多支持10位整数和5位小数。问题来自：http://www.cnblogs.com/batsing/p/4876280.html。<br>
详见程序内注释。

* `WouldIWinTheGame.java`用来用程序判断是否能赢得游戏。问题来自：http://segmentfault.com/q/1010000003883784。<br>
关于游戏的详细说明见程序内注释。

* `wiggle_sort.c`用来按小于、大于交替地对一个数组排序，问题来自：http://segmentfault.com/q/1010000004364292。<br>

