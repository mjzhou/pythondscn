# 什么是算法分析
It is very common for beginning computer science students to compare their programs with
one another. You may also have noticed that it is common for computer programs to look very
similar, especially the simple ones. 一个有趣的问题经常出现. 当两个看起来不同的程序解决相同的问题时，是否一个程序比另外一个更好?

为了能够回答这个问题, we need to remember that there is an important difference
between a program and the underlying algorithm that the program is representing. As we stated
in Chapter 1, an algorithm is a generic, step-by-step list of instructions for solving a problem.
It is a method for solving any instance of the problem such that given a particular input, the
algorithm produces the desired result. A program, on the other hand, is an algorithm that has
been encoded into some programming language. There may be many programs for the same
algorithm, depending on the programmer and the programming language being used.

To explore this difference further, consider the function shown below. This function solves a
familiar problem, computing the sum of the first n integers. The algorithm uses the idea of an
accumulator variable that is initialized to 0. The solution then iterates through the n integers,
adding each to the accumulator.
