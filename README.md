# MyTest
该项目用来存放我的测试程序。其中：

* `FloatTest`展示了一个由浮点数精度而导致计算出错的问题。详见程序内的注释。<br>
详见：http://www.cnblogs.com/antineutrino/p/4525224.html

* `Fibonacci`展示了一种计算超大数`Fibonacci`数列（不超过`2005`位`10`进制数）的方法。<br>
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


