# leetcode

## 一、DFS
1. 判断树是否是满足某种关系(true or false)，如是否是搜索树、是否对称,一般使用前中后序遍历可解决问题


[验证二叉搜索树](https://leetcode-cn.com/problems/validate-binary-search-tree/)

[相同的树](https://leetcode-cn.com/problems/same-tree/)

[对称二叉树](https://leetcode-cn.com/problems/symmetric-tree/)

2. 寻找树中的某种参数，如树的深度、某种组合等

[二叉树的最大深度](https://leetcode-cn.com/problems/maximum-depth-of-binary-tree/)

[平衡二叉树](https://leetcode-cn.com/problems/balanced-binary-tree/)

[二叉树的最小深度](https://leetcode-cn.com/problems/minimum-depth-of-binary-tree/)

[路径总和](https://leetcode-cn.com/problems/path-sum/)

[路径总和2](https://leetcode-cn.com/problems/path-sum-ii/)

[求根节点到叶节点数字之和](https://leetcode-cn.com/problems/sum-root-to-leaf-numbers/)

3. 利用二叉树、遍历的某种性质解决问题,如根据便利结果构造二叉树

> note:前序遍历的结果中，第一个元素是根节点的值，后面依次是左子树和右子树，每一个子树都符合这种结构；对于中序和后续遍历，唯一的不同是根节点位于中间和最后

> 前序遍历：[root node,(left subtree),(right subtree)]

> 中序遍历：[(left subtree),root node,(right subtree)]

> 后序遍历：[(left subtree),(right subtree),root node]

[从前序与中序遍历序列构造二叉树](https://leetcode-cn.com/problems/construct-binary-tree-from-preorder-and-inorder-traversal/)

[从中序与后序遍历序列构造二叉树](https://leetcode-cn.com/problems/construct-binary-tree-from-inorder-and-postorder-traversal/)

[将有序数组转换为二叉搜索树](https://leetcode-cn.com/problems/convert-sorted-array-to-binary-search-tree/)

[二叉树展开为链表](https://leetcode-cn.com/problems/flatten-binary-tree-to-linked-list/)

## 二、BFS

1. 二叉树的层序遍历，一般用队列实现

[二叉树的层序遍历](https://leetcode-cn.com/problems/binary-tree-level-order-traversal/)

[二叉树的层序遍历2](https://leetcode-cn.com/problems/binary-tree-level-order-traversal-ii/)

[填充每个节点的下一个右侧节点指针](https://leetcode-cn.com/problems/populating-next-right-pointers-in-each-node/)

[二叉树的锯齿形层序遍历](https://leetcode-cn.com/problems/binary-tree-zigzag-level-order-traversal/)

2. 不是二叉树，但可以转换成二叉树的问题解决


## 三、二分搜索(比较考验细节)

> 1. 重点在于选择是[left,right]还是[left,right)，这两种解法细节差别很大；
> 2. 选择mid=left+(right-left)/2还是mid=left+(right-left+1)/2选择也很重要

1. 二分查找基本操作及其变种

[x的平方根](https://leetcode-cn.com/problems/sqrtx/) 乘法可能会溢出，因此要使用除法（小心被除数等于0的情况）

2. 通过多次二分搜索解决

[旋转数组的最小数字](https://leetcode-cn.com/problems/xuan-zhuan-shu-zu-de-zui-xiao-shu-zi-lcof/) 小心重复元素

[搜索旋转排序数组](https://leetcode-cn.com/problems/search-in-rotated-sorted-array/)

[搜索旋转排序数据2](https://leetcode-cn.com/problems/search-in-rotated-sorted-array-ii/) 重点关注如何处理重复(unsolved)

[在排序数组中查找元素的第一个和最后一个位置](https://leetcode-cn.com/problems/find-first-and-last-position-of-element-in-sorted-array/)

## 四、滑动窗口
两者在应用场景上有些相似，很多可以同时使用两种方法解决

1. 经典滑动窗口题 

[无重复字符的最长子串](https://leetcode-cn.com/problems/longest-substring-without-repeating-characters/)

[至多包含两个不同字符的最长子串](https://leetcode-cn.com/problems/longest-substring-with-at-most-two-distinct-characters/)

[至多包含 K 个不同字符的最长子串](https://leetcode-cn.com/problems/longest-substring-with-at-most-k-distinct-characters/)

## 五、双指针

1. 从左右两侧向中间检索

[盛最多水的容器](https://leetcode-cn.com/problems/container-with-most-water/)

[接雨水](https://leetcode-cn.com/problems/trapping-rain-water/) 	上面两个很相似

[三数之和](https://leetcode-cn.com/problems/3sum/)			注意去重复

2. 快慢指针（快指针始终比满指针快n倍或n步等）

[删除链表的倒数第N个节点](https://leetcode-cn.com/problems/remove-nth-node-from-end-of-list/)

3. 都从左侧出发，但步伐不定

[移动零](https://leetcode-cn.com/problems/move-zeroes/)

[环形链表](https://leetcode-cn.com/problems/linked-list-cycle/)

## 六、贪心算法 

> 每次都最大或最多

[跳跃游戏](https://leetcode-cn.com/problems/jump-game/)

[跳跃游戏2](https://leetcode-cn.com/problems/jump-game-ii/)


## 七、动态规划

1. 经典的两个维度的dp问题,把这些弄明白就行了
> 注意滚动数组思想，可以大幅度优化空间复杂度
> dp问题分为两种，一种是求最优解类，典型的是背包问题。另一种是技术类，比如求方案总数。他们的一个共同的是当前问题的最优解往往取决于子问题或前一个问题的最优解

[最长回文子串](https://leetcode-cn.com/problems/longest-palindromic-substring/) 

[连续子数组的最大和](https://leetcode-cn.com/problems/lian-xu-zi-shu-zu-de-zui-da-he-lcof/)

[爬楼梯](https://leetcode-cn.com/problems/climbing-stairs/)	

[不同路径](https://leetcode-cn.com/problems/unique-paths/)

[不同路径2](https://leetcode-cn.com/problems/unique-paths-ii/)

[最小路径和](https://leetcode-cn.com/problems/minimum-path-sum/)

## 八、原地修改

一般是给定一个长度为n的数组，数组内元素的范围往往在0-n之间

[数组中重复的数字](https://leetcode-cn.com/problems/shu-zu-zhong-zhong-fu-de-shu-zi-lcof/)
