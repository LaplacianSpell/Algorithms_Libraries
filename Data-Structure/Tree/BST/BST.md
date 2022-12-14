# Binary Search Tree

## OJ-01

### 题目描述

琦琦有很多颗彩虹糖，每一颗彩虹糖有一个美味度（是不超过 $10^9$ 的非负整数），不同的彩虹糖可能有相同的美味度。

琦琦有一个大大的袋子，用来存放彩虹糖，初始时袋子为空。

琦琦每次会选择以下操作之一进行：

1. 琦琦给出 xx，把一颗美味度为 xx 的全新的彩虹糖放到袋子中，并且需要你输出袋子中有多少颗糖比这颗彩虹糖更美味（即美味度大于 xx）。
2. 琦琦给出 kk，从袋子中拿出袋子中第 kk 美味的糖，并且需要你输出该次操作拿出的糖的美味度。

### 输入格式

从标准输入读入数据。

第一行输入一个整数 mm，表示操作的总数。

接下来 mm 行，每行若干个整数，表示一个操作。

每行第 1 个整数表示这次进行的是第几种操作，每种操作格式如下：

1 x，其中 $1 \leq x \leq 10^9$。
2 k，其中 $k \geq 1$ 且 k 不超过当前袋子中的糖的个数。如果当前袋子为空，则不会出现此类操作。

### 输出格式

输出到标准输出。

输出 mm 行，每行一个整数，表示每次操作的输出结果。

>评价：采用特殊的节点，在构造节点的时候维护子树和重复值的大小，那么插入和寻找都是一个 $O(logn)$ 的过程
