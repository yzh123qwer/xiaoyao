# 学习内容
## 1、c语言的学习
### （1、malloc函数的学习和使用；
malloc函数
如果分配成功，则返回指向被分配内存空间的指针（指针类型为void*），不然返回指针NULL
补充：void*表示未被定义类型的指针，c/c++规定void*可以强制转换为任何其他类型的指针；其他任何类型都可以直接赋值给它，无需进行强制转换，但是反过来不可以。
### （2、函数中形参的理解，尤其是当函数参数为指针时；
### （2、
# 学习心得
在学习c语言的过程中，无论是对于函数的理解还是对于算法的理解，都会随着对计算机本身了解深入而深入。如在malloc函数的学习过程中，在之前的学习内容中包含二叉树和链表的使用，在定义完ADT结构体之后，第一想法是创建一个节点的数组，完成数据录入之后，在通过一定的方式将这些节点通过结构体中的指针互相连起来，尽管这样也实现了二叉树或者链表的目的，但这显然是不合理的，因为在定义数组的过程中，本身已经将所有数据通过数组的方式相连，在构造一种连接方式显然就是多此一举的；而在学习完malloc函数之后，malloc函数能够申请得到一片存储空间（这个空间一定是能将数据存储下的，因为malloc函数的参数通常可以使用sizeof函数来获取某一类型的占用空间），这样就达到了最开始目的，使得一些数据能够通过二叉树或者链表的形式连接起来（仅有这种方式）。