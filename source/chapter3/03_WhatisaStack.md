# 3.3 什么是栈？

栈（也叫下推栈）一种线性有序的数据元素集合，它的特点是，数据的增加删除操作都在同一端进行。进行操作的这一端，我们一般叫做“顶”，另一端叫做“底”。

栈的底部很有象征性，因为元素越接近底部，就意味着在栈里的时间越长。最近进来的，总是最早被移走，这种排列规律叫做先进后出，综合为LIFO。所以栈的排序是按时间长短来排列元素的。新来的在栈顶，老家伙们在栈底。

栈的例子经常看到。比如自助餐厅的盘，人们总是从上面拿盘子，拿走一个后面的人再拿下面的一个，（服务员端来一些新的，又堆在上面了）。又如一堆书，（图1）你只能看到最上面一本的封面，要看下面一本，就要把上面的先拿 走。图2是另一种栈，这保存了同个主要的python语言数据对象。

<center>![](Figures/bookstack2.png)</center>

<center>Figure 1: A Stack of Books</center>

<center>![](Figures/primitive.png)</center>

<center>Figure 2: A Stack  Primioftive Python Objects</center>

与栈有关的思想来自生活中的观察，假设你从一张干净的桌子开始，一本一本地放上书，这就是在建立栈。当你一本一本地拿走，想像一下，是不是先进后出？由于这种结构具有翻转顺序的作用，所以非常重要。图3显示了Python数据栈，加入和移走的顺序。

<center>![](Figures/simplereversal.png)</center>

<center>Figure 3: The Reversal Property of Stacks</center>

->![alt text](Figures/simplereversal.png)<-

栈这种翻转性，在你用电脑上网的时候也用到了。浏览器软件上都有“返回”按钮，当你从一个链接到另一个链接，这时网址（URL）就被存进了栈。正在浏览的页就存在栈顶，点“返回”的时候，返回到刚刚浏览的页面。最早浏览的页面，要一直到最后才能看到。

