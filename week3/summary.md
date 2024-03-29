# 学习内容
## 1、c语言的学习
### （1、malloc函数的学习和使用
malloc函数
如果分配成功，则返回指向被分配内存空间的指针（指针类型为void*），不然返回指针NULL
补充：void*表示未被定义类型的指针，c/c++规定void*可以强制转换为任何其他类型的指针；其他任何类型都可以直接赋值给它，无需进行强制转换，但是反过来不可以。
### （2、函数中形参的理解，尤其是当函数参数为指针时
### （3、复习字符串变量
### （4、enum函数的学习和使用
## 2、复习已学部分的《数据结构与算法分析》
## 3、《数据结构与算法分析》的学习
### （1、理解树中的单旋转和双旋转
### （2、理解散列函数的运算过程
散列函数能将字符进行运算的本质原因是字符在内存中存储方式也是数字，而在c语言中又是以ASCALL码进行存储的。如果散列函数只通过一些算数运算（如加减乘除）来获得散列值，那么想要得到一个好的散列函数，最重要的是数学的学习。但即使使得散列能将一个较为广泛的输入关键字群体（可以假设输入的都是字母），映射到一个较为广泛（几乎能映射到0到TableSize-1）的值域，也可能得到一些坏的结果，如假设用户输入的字母都是英文单词，那么此时映射所得到的值域将会变得相对集中在一些值（可能由于单词中的高频率词根或者词缀，需要结合算法来分析）。因此还要通过输入群体，来定义一个专属的，更好的散列函数。
### （3、理解解决散列函数发生冲突的原因，和与其相对应的解决方法
### （4、了解优先队列的背景，和优先队列的目的

# 学习心得
在学习c语言的过程中，无论是对于函数的理解还是对于算法的理解，都会随着对计算机本身了解深入而深入。如在malloc函数的学习过程中，在之前的学习内容中包含二叉树和链表的使用，在定义完ADT结构体之后，第一想法是创建一个节点的数组，完成数据录入之后，在通过一定的方式将这些节点通过结构体中的指针互相连起来，尽管这样也实现了二叉树或者链表的目的，但这显然是不合理的，因为在定义数组的过程中，本身已经将所有数据通过数组的方式相连，在构造一种连接方式显然就是多此一举的；而在学习完malloc函数之后，malloc函数能够申请得到一片存储空间（这个空间一定是能将数据存储下的，因为malloc函数的参数通常可以使用sizeof函数来获取某一类型的占用空间），这样就达到了最开始目的，使得一些数据能够通过二叉树或者链表的形式连接起来（仅有这种方式）。<br>
在学习`《数据结构与算法分析》`的过程中，随着难度的逐渐加大，过程是曲折的。如学习一个新的概念，读完定义以后，只会对新概念有一些极其简单的想法，甚至认为新概念是难以理解的，在读完c语言描述的算法（这个过程也是缓慢的）之后，对概念又有了一些新的看法和想法，反过来看定义又会有一些新的理解。
