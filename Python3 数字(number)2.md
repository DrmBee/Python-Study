# Python3 数字(number)

Python数字数据类型用于存储数值。

数据类型是不允许改变的，这就意味着如果改变数字类型的值，将重新分配空间。

可以使用del语句删除一些数字对象的引用。

del语句的语法是：

`del var1[,var2[,var3[...,varN]]]`

也可以通过del语句删除单个或多个对象的引用，例如

`del var`

`del var_a,var_b`

Python 支持三种不同的数值类型：

- 整型（int）-通常被称为是整型或整数，是正或负整数，不带小数点。Python3整型是没有限制大小的，可以当作Long类型使用，所以Python3没有Python2的Long类型。布尔（bool）是整型的子类型。
- 浮点型（float）-浮点型由整数部分与小数部分组成，浮点型也可以使用科学计数法表示。
- 复数（complex）-复数由实数部分和虚数部分构成，可以用a+bj，或者complex(a,b)表示，复数的实部a和虚部b都是浮点型。

------

###### Python数字类型转换

数据类型的转换，只需要将数据类型作为函数名即可。

- int(x)将x转换为一个整数。
- float(x)将x转换到一个浮点数。
- complex(x)将x转换到一个复数，实数部分为x，虚数部分为0。
- complex(x,y)将x和y转换到一个复数，实数部分为x，虚数部分为y。x和y是数字表达式。

------

###### Python数字运算

注意：`//`得到的并不一定是整数类型的数，它与分母分子的数据类型有关系。

```
print(5//2)
print(5.0//2)
print(5//2.0)
print(-5//2)
print(5//-2)
print(-5//-2)
---------------------------
输出：
2
2.0
2.0
-3
-3
2
```

Python可以使用 `**`操作来进行幂运算。

变量在使用前必须先“定义”（即赋予变量一个值），否则会出现错误。

不同类型的数混合运算时会将整数转换为浮点数。

在交互模式中，最后被输出的表达式结果被赋值给变量_。

------

###### **数学函数**

| 函数           | 返回值 ( 描述 )                                              |
| :------------- | :----------------------------------------------------------- |
| abs(x)         | 返回数字的绝对值，如abs(-10) 返回 10                         |
| ceil(x)        | 返回数字的上入整数，如math.ceil(4.1) 返回 5                  |
| cmp(x,y)       | 如果 x < y 返回 -1, 如果 x == y 返回 0, 如果 x > y 返回 1。 Python 3 已废弃，使用 (x>y)-(x<y) 替换。 |
| exp(x)         | 返回e的x次幂(ex),如math.exp(1) 返回2.718281828459045         |
| fabs(x)        | 返回数字的绝对值，如math.fabs(-10) 返回10.0                  |
| floor(x)       | 返回数字的下舍整数，如math.floor(4.9)返回 4                  |
| log(x)         | 如math.log(math.e)返回1.0,math.log(100,10)返回2.0            |
| log10(x)       | 返回以10为基数的x的对数，如math.log10(100)返回 2.0           |
| max(x1,x2,...) | 返回给定参数的最大值，参数可以为序列。                       |
| min(x1,x2,...) | 返回给定参数的最小值，参数可以为序列。                       |
| modf(x)        | 返回x的整数部分与小数部分，两部分的数值符号与x相同，整数部分以浮点型表示。 |
| pow(x, y)      | x**y 运算后的值。                                            |
| round(x[,n])   | 返回浮点数 x 的四舍五入值，如给出 n 值，则代表舍入到小数点后的位数。其实准确的说是保留值将保留到离上一位更近的一端。 |
| sqrt(x)        | 返回数字x的平方根。                                          |

------

###### 随机数函数

| 函数                               | 描述                                                         |
| :--------------------------------- | :----------------------------------------------------------- |
| choice(seq)                        | 从序列的元素中随机挑选一个元素，比如random.choice(range(10))，从0到9中随机挑选一个整数。 |
| randrange ([start,\] stop [,step]) | 从指定范围内，按指定基数递增的集合中获取一个随机数，基数默认值为 1 |
| random()                           | 随机生成下一个实数，它在[0,1)范围内。                        |
| seed([x\])                         | 改变随机数生成器的种子seed。如果你不了解其原理，你不必特别去设定seed，Python会帮你选择seed。 |
| shuffle(lst)                       | 将序列的所有元素随机排序                                     |
| uniform(x, y)                      | 随机生成下一个实数，它在[x,y]范围内。                        |

------

###### 三角函数

| 函数                                                         | 描述                                              |
| :----------------------------------------------------------- | :------------------------------------------------ |
| [acos(x)](https://www.runoob.com/python3/python3-func-number-acos.html) | 返回x的反余弦弧度值。                             |
| [asin(x)](https://www.runoob.com/python3/python3-func-number-asin.html) | 返回x的反正弦弧度值。                             |
| [atan(x)](https://www.runoob.com/python3/python3-func-number-atan.html) | 返回x的反正切弧度值。                             |
| [atan2(y, x)](https://www.runoob.com/python3/python3-func-number-atan2.html) | 返回给定的 X 及 Y 坐标值的反正切值。              |
| [cos(x)](https://www.runoob.com/python3/python3-func-number-cos.html) | 返回x的弧度的余弦值。                             |
| [hypot(x, y)](https://www.runoob.com/python3/python3-func-number-hypot.html) | 返回欧几里德范数 sqrt(x*x + y*y)。                |
| [sin(x)](https://www.runoob.com/python3/python3-func-number-sin.html) | 返回的x弧度的正弦值。                             |
| [tan(x)](https://www.runoob.com/python3/python3-func-number-tan.html) | 返回x弧度的正切值。                               |
| [degrees(x)](https://www.runoob.com/python3/python3-func-number-degrees.html) | 将弧度转换为角度,如degrees(math.pi/2) ， 返回90.0 |
| [radians(x)](https://www.runoob.com/python3/python3-func-number-radians.html) | 将角度转换为弧度                                  |

------

###### 数学常量

| 常量 | 描述                   |
| ---- | ---------------------- |
| pi   | 数学常量pi(圆周率)     |
| e    | 数学常量e，e即自然常数 |





