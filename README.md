# Algorithm_and_Data_Structure

一、计算机领域待解决问题

	1）旅行商问题
	2）
二、双指针

	1）左指针指向已经处理好的序列的尾部，右指针指向待处理序列的头部
三、牛顿迭代法

	1）y_(n+1)=y_n−f(y_n )/(f^′ (y_n ) )
	2）例如求根号x，即f(y) = y2 - x，迭代表达式就为：y=y − (y^2−x)/2y=(y+x/y)/2
四、数组

	1.数组和链表的区别
		1）数组适合读取操作，链表适合插入删除操作
		2）数组支持随机访问，链表只能顺序访问
	2.常规数组和有序数组的区别：
		1）常规数组适合插入操作，有序数组适合查找操作
五、链表数组：数组包含n个元素，每个元素都指向一个链表

六、排序

	1.选择排序
		1）原理：首先在未排序序列中找到最小（大）元素，存放到排序序列的起始位置，然后，再从剩余未排序元素中继续寻找最小（大）元素，然后放到已排序序列的末尾。以此类推，直到所有元素均排序完毕
	2.快速排序
		1）原理：将数组的第一个元素用作基准值，然后将小于等于基准值的分为一组，大于基准值的也分为一组，然后对两个子数组继续进行快速排序
七、递归

	1.定义：递归指的是调用自己的函数
	2.递归函数的两部分
		1）基线条件：函数不在调用自己的条件
		2）递归条件：函数调用自己的条件
八、栈

	1.每当调用函数时，计算机会将调用涉及的所有变量的值存储到内存中，计算机使用栈来表示这些内存块
	2.当存在嵌套函数时，当调用嵌套函数时，嵌套函数的变量值压栈，嵌套函数调用完，其在栈中的变量值将被弹出
九、散列表

	1）Python提供的散列表实现为字典，可以使用dict()函数或者{ }来创建散列表
	2）网址映射到IP地址的过程称为DNS解析，散列表是提供这种功能的方式之一
	3）缓存是一种常用的加速方式，所有的大型网站都是用缓存，而缓存的数据则存储在散列表中
	4）散列表的冲突：散列函数将不同的键映射到数组的相同位置时发生的问题。
	5）冲突的解决办法：如果两个键映射到同一个位置，就在这个位置存储一个链表，即链表数组
	6）散列表非常适合用于防止重复
	7）散列表是无序的，因此添加键值对的顺序无关紧要
十、搜索

	1.广度优先搜索
		1）作用：求得通过节点最少的路径（非加权图）-对应换乘少
	2.狄克斯特拉算法
		1）作用：正加权边最短路径算法（加权图） -对应时间短
		2）适用范围：只适用有向无环图而且不能有负权边
十一、贪心算法

	1.定义：在对问题求解时，总是做出在当前看来是最好的选择
	2.涉及所有组合的问题通常是NP完全问题
十二、动态规划

	1.原理：将问题分成小问题，并先着手解决这些小问题
	2.适用范围：
		1）每个子问题都是独立及离散的，即不依赖其他子问题时，动态规划才管用
		2）只能在给定约束条件时找到最优解
十三、K最近邻算法

	1.原理：在训练集中找到该实例最邻近的K个实例，这K个实例的多数属于某个类，就把该输入实例分类到这个类中（物以类聚，人以群分）
	2.如何确定两个实例的邻近关系：特征提取（将物品转换为一系列可比较的数字），然后根据距离公式计算距离
	3.分类和回归：分类就是编组，回归就是预测结果
	4.余弦相似度：不计算两个矢量的距离，而比较它们的角度
十四、位图

	1.该数据结构描述了一个有限定义域内的稠密集合，其中的每一个元素最多出现一次并且没有其他任何数据与该元素相关联
十五、树

	1.域名体系就是树结构（mail.xs.ustb.edu.cn)
	2.叶节点：没有子节点的节点
	3.二叉树：每个节点最多有两个子节点的树
	4.树的定义：可以用递归定义
	5.树的实现：
		1）嵌套列表法
		2）节点链接法：每个节点保存根节点的数据项，以及指向左右子树的链接
	6.树的应用：
		1）表达式解析
		2）自然语言处理
十六、反向索引

	1.对于一个散列表，根据值映射到键的数据结构被称为反向索引，常用于创建搜索引擎
十七、基础知识：

	1.O(1)就是用来表示所有数据增长但是步数不变的算法；O(logN)表示当数据量翻倍时，步数加一
	2.
