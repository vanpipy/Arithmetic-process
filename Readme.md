# 闲谈
对于任何一门科学的正确概念，都不能从有关这门科学的片段知识中形成，尽管这些片段知识足够广泛。还需要对这么科学的整体有正确的观点，需要了解这么科学的本质 -- `数学的内容，方法及意义`

显然如同上面所描述的，对于计算同样适用。计算是什么，它的本质又是什么。如果计算是一个问题，那么它的前一个问题是什么，后一个问题又什么，或者左边，右边的问题，

这些都不是该篇讨论的范围，该篇讨论范围仅限于事物本身，并不深究其承前以及启后。

# 四则运算
形如`x + y = z`可以称作公式，而`x`单独具有如何的意义取决于公式应用的场景，如果x代表兔的腿数，y代表鸡的腿数，那么z则代表兔和鸡腿数的总和。换一种说法同样成立。`x - y = z`同加法类似。

而`x * y = z`则可称作x个y相加或者y个x相加的和z，这种简便的书写方式称作乘法[1]。与乘法相对应的是除法`x = z / y`如果参照乘法的说明，z减去y个x得到的差，显然是有问题的。所以说乘法和除法同加法和减法是不同的，使用于加法和减法的规则并不一定使用于乘法和除法。那么如何描述它们？

首先假设[1]是成立的，那么`x + x + ...(y个) = z`，表示为`x * y = z`。显然如果是单独y - 1个的话就是`x + x * (y - 1) = z`，换成减法的话就是`x = z - x * (y - 1)`, 显然如果`x = z / y`是成立的话，`z - x * (y - 1) = z / y`，表示为z减去y - 1个x就得到x，这种表示方法就成为除法。

所以在这里可以重新定义一下计算的解释:

- `x + y = z` 定义为加法，`x - y = z` 定义为减法，`x * y = z` 定义为乘法， `x / y = z` 定义为除法。
- 乘法和除法是加法和减法的更高一级的抽象表达。
- 依据加法和减法的定义，乘法和除法的定义是可以证明的，而加法和减法自身可以归纳证明。

## 目录

- 四则运算的定义
    - 加减乘除的定义
    - 证明

- 抽象到实现
    - 计算机中如何定义加减乘除
    - 二叉树的计算公式表达
    - 基于树结构的C语言实现
