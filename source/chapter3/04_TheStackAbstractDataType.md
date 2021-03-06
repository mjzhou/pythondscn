# 3.4 栈的抽象数据类型

下面的结构和操作定义了栈的抽象数据类型。如前所述，栈是结构化的，有序的的数据集，它的增删操作都在叫在”栈顶“的一端进行，存储顺序是LIFO。栈的操作方法如下：

* `Stack()`,构造方法，创建一个空栈，无参数，返回值是空栈。
* `Push(item)`向栈顶压入一个新数据项，需要一个数据项参数，无返回值。
* `pop()`抛出栈顶数据项，无参数，返回被抛出的数据项，栈本身发生变化。
* `Peek()`返回栈顶数据项，但不删除。不需要参数，栈不变。
* `isEmpty()`测试栈是否空栈。不需要参数，返回布尔值。
* `size()`返回栈内数据项的数目，不需要参数，返回值是整数。

例如，s是一个空栈，表1是一系列的操作，栈内数据和返回值。注意栈顶在右侧。

|Stack Operation         | Stack Contents           | Return Value  |
| ------------- |-------------| ----- |
| `s.isEmpty()`	|`[]`|	`True`|
| `s.push(4)`	|`[4]`|	 |
| `s.push('dog')`	|`[4,'dog']`||	 
| `s.peek()`	|`[4,'dog']`|	`'dog'`|
| `s.push(True)`	|`[4,'dog',True]`|	| 
| `s.size()`	|`[4,'dog',True]`|	`3`|
| `s.isEmpty()`	|`[4,'dog',True]`|	`False`|
| `s.push(8.4)`	|`[4,'dog',True,8.4]`|	 |
| `s.pop()`	|`[4,'dog',True]`|	`8.4`|
| `s.pop()`	|`[4,'dog']`|	`True`|
| `s.size()`	|`[4,'dog']`|	`2`|