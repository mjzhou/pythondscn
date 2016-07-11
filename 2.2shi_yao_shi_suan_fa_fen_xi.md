# 什么是算法分析
 计算机科学系的学生比较他们的程序是非常常见的。你可能注意到计算程序看起来非常相似，特别是简单的那个。 一个有趣的问题经常出现。当两个看起来不同的程序解决相同的问题时，是否一个程序比另外一个更好？

为了能够回答这个问题, we need to remember that there is an important difference
between a program and the underlying algorithm that the program is representing. As we stated
in Chapter 1, an algorithm is a generic, step-by-step list of instructions for solving a problem.
It is a method for solving any instance of the problem such that given a particular input, the
algorithm produces the desired result. A program, on the other hand, is an algorithm that has
been encoded into some programming language. There may be many programs for the same
algorithm, depending on the programmer and the programming language being used.

进一步探讨这种差异, 思考下面的函数。这个函数解决了一个常见的问题，计算从1到整数n的和。 The algorithm uses the idea of an
accumulator variable that is initialized to 0. The solution then iterates through the n integers,
adding each to the accumulator.

```python
def sumOfN(n):
   theSum = 0
   for i in range(1,n+1):
       theSum = theSum + i

   return theSum

print(sumOfN(10))
```
