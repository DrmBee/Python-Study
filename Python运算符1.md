# Python运算符

###### Python逻辑运算符

| 运算符 | 逻辑表达式 | 描述                                                         |
| ------ | ---------- | ------------------------------------------------------------ |
| and    | x and y    | 布尔"与"-如果x为False，x and y 返回 x 的值，否则返回 y 的计算值。 |
| or     | x or y     | 布尔“或”-如果x为True,它返回x的值，否则它返回y的计算值。      |
| not    | not x      | 布尔“非”-如果x为True,返回False。如果x为False，它返回True.    |

###### Python成员运算符

| 运算符 | 描述                                                 |
| ------ | ---------------------------------------------------- |
| in     | 如果在指定的序列中找到值返回True，否则返回False。    |
| not in | 如果在指定的序列中没有找到值返回True,否则返回False。 |

###### Python身份运算符

身份运算符用于比较两个对象的存储单元。

| 运算符 | 描述                                        | 实例                                                         |
| ------ | ------------------------------------------- | ------------------------------------------------------------ |
| is     | is是判断两个标识符是不是引用自一个对象      | x is y,类似id(x)==id(y),如果引用的是同一个对象则返回True,否则返回False. |
| is not | is not 是判断两个标识符是不是引用自不同对象 | x is not y,类似id(a) != id(b)。如果引用的不是同一个对象则返回结果True,否则返回False. |

其他Python运算符和C差不多。