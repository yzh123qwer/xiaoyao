# 学习内容
## 1、c语言的学习
## 2、《数据结构与算法分析》的学习
### （1、插入排序和希尔排序
### （2、堆排序
### （3、归并排序
### （4、快速排序
### （5、大型数据结构的排序，桶式排序、外部排序
# 学习心得
这周的学习内容都是对数据进行排序操作，目的很明确，算法在理解上相对于前面的内容都是较为简单的。但是在理解算法之后，对程序的细节设计依然是比较困难的。<br>
递归使用时，必须使递归的方向向着一个基准型靠近。但是在书上给出归并算法的程序，对于基准型的判断是极其隐晦的（它能将基准型归类到了错误类型，又或者说这两者可以通过同一种方式判断）。<br>
在数组排序设计过程中，尤其需要考虑一些特殊的位置，这些地方通常伴随着加1、减1操作，书上给出的程序依然是非常高明并且简练的；但实际通过自己编写练习过程中，这些往往是复杂的，困难的。<br>
第七章除去程序设计的内容，还有大量的篇幅是关于算法时间分析的。这些内容同样是困难的！但是通过学习，可以很明显的发现，想要得到一个更快的排序的算法，主要在于将很长的数组按照一定规则分成较短的数组（分治，这在希尔排序、归并排序、快速排序中都有体现），以及根据数据类型来选取最佳的方案（桶式排序就是最好的例子！）。
