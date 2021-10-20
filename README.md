<table>
  <thead>
    <tr>
      <th>#</th>
      <th>Q</th>
      <th>Fig</th>
      <th>A</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>3.1</td>
      <td>找出 0~n-1 中任意一个重复的数字</td>
      <td>

```
 0   1  2  3  4  5 6
--------------------
        p
(2)  3 (1) 0  2  5 3
     p
(1) (3) 2  0  2  5 3
           p
(3)  1  2 (0) 2  5 3
        p
 0   1 (2) 3 (2) 5 3
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>3.2</td>
      <td>不修改输入找出 1~n 中任意一个重复的数字</td>
      <td>

```
      4 3 5 2 3 2 6 7
range [1,           7]
            8
range [1,      4][5,7]
            5       3
range [1,2][3, 4]
        2   3
range      [3][4]
            2  1
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>4</td>
      <td>“二维数组中的查找”</td>
      <td>

```
7

(0,3)           (0,1)
A[:][:]         A[:][:2]
[1 (2)| 8  9]   [1  2 ]
[2  4 | 9 12]   [2  4 ]
[4  7 |10 13]   [4 (7)]
[6  8 |11 15]   [6  8 ]
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>5.2</td>
      <td>从后往前合并排序数组</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>6</td>
      <td>从尾到头打印链表</td>
      <td></td>
      <td>栈</td>
    </tr>
    <tr>
      <td>7</td>
      <td>前序+中序重建二叉树</td>
      <td>

```
Pre-order:
[1] 2 4 7 | 3 5 6 8
  [2] 4 7
    [4] 7
          [3] 5 | 6 8
                [6] 8
In-order:
4 7 2 [1] 5 3 8 6
4 7 [2]
[4] 7
          5 [3] 8 6
                8 [6]
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>8</td>
      <td>找出二叉树中序遍历序列的下一个节点</td>
      <td></td>
      <td><a href="https://en.wikipedia.org/wiki/Threaded_binary_tree">中序线索二叉树</a></td>
    </tr>
    <tr>
      <td>9.1</td>
      <td>“用两个栈实现队列”</td>
      <td>

```
In       Out
[a b c], []
[],      [c b]    pop() -> a
[],      [c]      pop() -> b
[d e],   []       pop() -> c
[],      [e]      pop() -> d
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>9.2</td>
      <td>“用两个队列实现一个栈”</td>
      <td>

```
                            < <, < a b (c)<
                  < a (b)<, < <             pop() -> c
          < a <,  < <                       pop() -> b
        < a (d)<                            push(d)
< a <,  < <                                 pop() -> d
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>10.1</td>
      <td>斐波那契数列</td>
      <td></td>
      <td>公式</td>
    </tr>
    <tr>
      <td>10.2</td>
      <td>青蛙跳台阶，一次1级或2级</td>
      <td></td>
      <td>f(n) = f(n-1) + f(n-2), 斐波那契数列</td>
    </tr>
    <tr>
      <td>10.3</td>
      <td>青蛙跳台阶，一次 1~n 级</td>
      <td>

```
n=1, a[1]=1
n=2, a[2]=2
n=3, a[3]=4
...
```

</td>
      <td>数学归纳法， f(n) = 2**(n-1)</td>
    </tr>
    <tr>
      <td>10.4</td>
      <td>盖瓷砖</td>
      <td>

```
 0 1 2 3 4 5 6 7
|*| | | | | | | |
|*| | | | | | | |
 0 1 2 3 4 5 6 7
|*|*| | | | | | |
| | | | | | | | |
```

</td>
      <td>f(8) = f(7) + f(6), 斐波那契数列</td>
    </tr>
    <tr>
      <td>11</td>
      <td>“旋转数组的最小数字”</td>
      <td>

```
0 1  2  3  4
------------
3 4 [5] 1  2    3<5>2, L = mid + 1
       [1] 2    3>1<2, R = mid
       [1]

0 1  2  3  4 5 6
----------------
1 2  0 [1] 1 1 1    1==1==1, ?
  2  0 [1] 1 1 1    2>1==1, R = mid
  2 [0] 1           2>0<1, R = mid
 [2] 0              2==2>1, L = mid + 1
    [0]

0 1  2  3  4  5
---------------
1 1 [1] 2  0  1     1==1==1, ?
        2 [0] 1     2>0<1, R = mid
       [2] 0        2==2>1, L = mid + 1
          [0]
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>12</td>
      <td>“矩阵中的路径”</td>
      <td>

```
a [b] t  g
c [f][c] s
j  d [e] h
```

</td>
      <td>DFS</td>
    </tr>
    <tr>
      <td>13</td>
      <td>“机器人的运动范围”</td>
      <td></td>
      <td>DFS/BFS</td>
    </tr>
    <tr>
      <td rowspan="2">14</td>
      <td rowspan="2">“剪绳子”</td>
      <td>

```
l = 0, a[0] = 0
l = 1, a[1] = 1
l = 2, a[2] = 2
l = 3, a[3] = 3
l = 4, a[4] = max(a[3]*a[1], a[2]*a[2]) = 4
l = 5, a[5] = max(a[4]*a[1], a[3]*a[2]) = 6
l = 6, a[6] = max(a[5]*a[1], a[4]*a[2], a[3]*a[3]) = 9
```

</td>
      <td>2和3很特殊，见下</td>
    </tr>
    <tr>
      <td></td>
      <td>数论题。“当n>=5时，我们尽可能多地剪长度为3的绳子；当剩下的绳子长度为4时，把绳子剪成两段长度为2的绳子（或不剪）。”</td>
    </tr>
    <tr>
      <td>15.1</td>
      <td>“二进制中1的个数”</td>
      <td>

```
   n & (n-1)
1111 & 1110 = 1110      1
1110 & 1101 = 1100      2
1100 & 1001 = 1000      3
1000 & 0111 = 0         4
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>15.2</td>
      <td>“判断一个整数是不是2的整数次方”</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>15.3</td>
      <td>Diff 整数 m 和 n 的二进制位</td>
      <td></td>
      <td>异或中1的位数</td>
    </tr>
    <tr>
      <td>16</td>
      <td>实现<code>pow()</code></td>
      <td></td>
      <td>快速幂</td>
    </tr>
    <tr>
      <td rowspan="2">17</td>
      <td rowspan="2">输出所有的 n 位数</td>
      <td></td>
      <td>Arbitrary integer</td>
    </tr>
    <tr>
      <td>

```
[0-9][...
    0[0-9][...
        09[0-9]
```

</td>
      <td><code>itertools.product()</code></td>
    </tr>
    <tr>
      <td>18.1</td>
      <td>篡改链表</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>18.2</td>
      <td>链表消消乐</td>
      <td>

```
None *    N
    [1]->[2]->[3]->[3]->[4]->[4]->[4]->[5]
HT
[]  (append)
3              *    N
              [3]->[3]->[4]->[4]->[4]->[5]
H         T
[]->[1]->[2]  (no append)
3                   *    N
              [3]->[3]->[4]->[4]->[4]->[5]
H         T
[]->[1]->[2]       (no append)
4                        *    N
                        [4]->[4]->[4]->[5]
H         T
[]->[1]->[2]            (no append)
None                                    *    N
                                       [5]
H         T
[]->[1]->[2]                           (append)
H              T
[]->[1]->[2]->[5]
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>19</td>
      <td>实现正则引擎</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>20</td>
      <td>Parse string to number</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>21</td>
      <td>调整数组中数字的顺序使奇数位于前半部分，偶数位于后半部分</td>
      <td>

```
  p     q
1 2 3 4 5
    q p
1 5 3 4 2
```

</td>
      <td>2 way partition</td>
    </tr>
    <tr>
      <td>22.1</td>
      <td>“链表中倒数第k个节点”</td>
      <td>

```
3

[1]->[2]->[3]->[4]->[5]->[6]
           R
[1]->[2]->[3]->[4]->[5]->[6]
 L         R
[1]->[2]->[3]->[4]->[5]->[6]
                L         R
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>22.2</td>
      <td>“求链表的中间节点”</td>
      <td>

```
Odd:
[1]->[2]->[3]->[4]->[5]
p,q
      p    q
           p         q
Even:
[1]->[2]->[3]->[4]->[5]->[6]
p,q
      p    q
           p         q
                p              q
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>23</td>
      <td>“链表中环的入口节点”</td>
      <td>

```
      t    h
[1]->[2]->[3]->[4]
           |    |
          [6]<-[5]

           t
[1]->[2]->[3]->[4]
           |    |
          [6]<-[5]  h

           h    t
[1]->[2]->[3]->[4]
           |    |
          [6]<-[5]

[1]->[2]->[3]->[4]
           |    |
          [6]<-[5]  t,h

 t
[1]->[2]->[3]->[4]
           |    |
          [6]<-[5]  h

      t
[1]->[2]->[3]->[4]
           |    |
        h [6]<-[5]

          t,h
[1]->[2]->[3]->[4]
           |    |
          [6]<-[5]
```

</td>
      <td><a href="https://en.wikipedia.org/wiki/Cycle_detection#Floyd's_tortoise_and_hare">Floyd's tortoise and hare</a></td>
    </tr>
    <tr>
      <td>24</td>
      <td>“反转链表”</td>
      <td>

```
P    *    N
[]  [a]->[b]->...->[h]->[i]->[j]->...
L1  L2
     P    *    N
[]<-[a]<-[b]  ...->[h]->[i]->[j]->...
L1  L2
                    P    *    N
[]<-[a]<-[b]<-...<-[h]<-[i]  [j]->...
L1  L2                   R1  R2

Special case:       P    *    N
[]<-[a]<-[b]<-...<-[h]<-[i]
                         R1  R2
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>25</td>
      <td>“合并两个排序的链表”</td>
      <td>

```
      *    N
     [3]->[5]->[7]
 *    N
[2]->[4]->[6]->[8]
H    T
[]->[1]
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>26</td>
      <td>“树的子结构”</td>
      <td></td>
      <td>find + check</td>
    </tr>
    <tr>
      <td>27</td>
      <td>“二叉树的镜像”</td>
      <td>

```
    8             8
 6     10      10    6
5 7   9 11    11 9  7 5

    8
 10    6
9 11  5 7

    8
 10    6
11 9  7 5
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>28</td>
      <td>二叉树是否对称</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>29</td>
      <td>顺时针打印矩阵</td>
      <td>

```
A[:][:],      →,  x0 += 1
     1  2  3  4
     ----------
[1]  5  6  7  8
[2]  9 10 11 12
[3] 13 14 15 16
    [0  1  2  3]

A[1:][:],     ↓,  y1 -= 1
    [0  1  2]
[1]  5  6  7 | 8
[2]  9 10 11 |12
[3] 13 14 15 |16

A[1:][:3],    ←,  x1 -= 1
    [0  1  2]
[1]  5  6  7
[2]  9 10 11
    --------
    13 14 15

A[1:3][:3],   ↑,  y0 += 1
       [1  2]
    5 | 6  7  [1]
    9 |10 11  [2]

A[1:3][1:3],  →,  x0 += 1
       6  7
      -----
[2]   10 11
      [1  2]

A[2:3][1:3],  ↓,  y1 -= 1
      [1]
[2]   10 | 11

A[2:3][1:2],  ←,  x1 -= 1
      [1]
[2]   10

A[2:2][1:2]
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>30</td>
      <td>实现栈的<code>min()</code></td>
      <td>

```
Data      Min
3         3
3 4       3 3
3 4 2     3 3 2
3 4 2 1   3 3 2 1
3 4 2     3 3 2
3 4       3 3
3 4 0     3 3 0
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>31</td>
      <td>“栈的压入、弹出序列”</td>
      <td>

```
1,2,3,4,5
4,5,3,2,1   4,3,5,1,2

[1,2,3][5]  ->  4
[1,2,3][]   ->  5
[1,2][]     ->  3
[1][]       ->  2
[][]        ->  1

[1,2,3][5]  ->  4
[1,2][5]    ->  3
[1,2][]     ->  5
[1,2][]     ->  1   X
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>32</td>
      <td>二叉树 层序遍历</td>
      <td></td>
      <td>BFS</td>
    </tr>
    <tr>
      <td>33</td>
      <td>BST 后序遍历序列</td>
      <td>

```
[5  7  6][9 11 10][8]
[5][7][6]
        [9][11][10]

7 4 6 [5]
  X
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>34</td>
      <td>二叉树路径和</td>
      <td>

```
    [10]
  [5] [12]
[4][7]  22
19  22
```

</td>
      <td>先序遍历</td>
    </tr>
    <tr>
      <td>35</td>
      <td>度为2的链表的复制</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>36</td>
      <td>BST 转双向链表</td>
      <td></td>
      <td><a href="https://en.wikipedia.org/wiki/Threaded_binary_tree">中序线索二叉树</a></td>
    </tr>
    <tr>
      <td>37</td>
      <td>序列化二叉树</td>
      <td>

```
Deserialize:
1   2 4 $ $ $   3 5 $ $ 6 $ $
   (2           3              )
     (4     $)   (5     6     )
       ($ $)       ($ $) ($ $)
```

```python
def traverse():
    root = dq.popleft()
    if root == '$':
        return None
    root = Node(root)
    root.left = traverse()
    root.right = traverse()
    return root
```

</td>
      <td>先序遍历</td>
    </tr>
    <tr>
      <td>38.1</td>
      <td>“字符串的排列”</td>
      <td>

```
a,b,c,d

[a|b,c,d]
    a[b|c,d]
        ab[c|d]
            abc[d]
        ab[d|c]
            abd[c]
    a[c|b,d]
        ac[b|d]
            acb[d]
        ac[d|b]
            acd[b]
    a[d|c,b]
        ad[c|b]
            adc[b]
        ad[b|c]
            adb[c]
[b|a,c,d]
    ...
    b[d|c,a]
        ...
        bd[a|c]
            bda[c]
[c|b,a,d]
    ...
    c[d|a,b]
        ...
        cd[b|a]
            cdb[a]
[d|b,c,a]
    ...
    d[a|c,b]
        ...
        da[b|c]
            dab[c]
```

</td>
      <td><code>itertools.permutations()</code></td>
    </tr>
    <tr>
      <td>38.2</td>
      <td>“字符串的组合”</td>
      <td>

```
a,b,c,d

0 0 0 0
0 0 0 1
...
1 1 1 1

Lexicographically ordered:
l = 1,  a, b, c, d
l = 2,  a[b,c,d]    ab, ac, ad
          b[c,d]    bc, bd
            c[d]    cd
             d[]    X
l = 3,           ab[c,d]    abc, abd
            ac[d], bc[d]    acd, bcd
        ad[], bd[], cd[]    X
l = 4,  abcd
```

</td>
      <td><code>itertools.combinations()</code></td>
    </tr>
    <tr>
      <td>39</td>
      <td>“数组中出现次数超过一半的数字”</td>
      <td></td>
      <td><a href="https://en.wikipedia.org/wiki/Boyer-Moore_majority_vote_algorithm">Boyer–Moore majority vote algorithm</a></td>
    </tr>
    <tr>
      <td rowspan="2">40</td>
      <td rowspan="2">“最小的k个数”</td>
      <td>

```
Top 4
while p < K:
         K           p
[4 5  1  6  2  7  3][8]
 4 5  1  6  2  7 [3]
 2 1  5  6  4  7 [3]
      p  |
[2 1][3][6  4  7  5]
         6  4  7 [5]
         4  6  7 [5]
         |  p
        [4][5][7, 6]
```

</td>
      <td><a href="https://en.wikipedia.org/wiki/Partial_sorting">Partial sorting</a></td>
    </tr>
    <tr>
      <td></td>
      <td><code>heapq</code></td>
    </tr>
    <tr>
      <td rowspan="2">41</td>
      <td rowspan="2">数据流中位数</td>
      <td></td>
      <td>类AVL树</td>
    </tr>
    <tr>
      <td>

```
When balanced:
                small   large
                [1 2 4] [6 8 9]
Push to small:  [1 2 4 7] [6 8 9]
Pop to large:   [1 2 4] [6 7 8 9]

When unbalanced:
                small   large
                [1 2 4] [6 7 8 9]
Push to large:  [1 2 4] [3 6 7 8 9]
Pop to small:   [1 2 3 4] [6 7 8 9]
```

</td>
      <td>LeetCode 295</td>
    </tr>
    <tr>
      <td>42</td>
      <td>“连续子数组的最大和”</td>
      <td>

```
1  -2  3  10  -4    7    2   -5
1  -2 [3] 10  -4    7    2   -5     Restart
1 [-1] 2 [13] [9] [16] [18] [13]    累加
```

</td>
      <td>动态规划</td>
    </tr>
    <tr>
      <td>43</td>
      <td>“1~n整数中1出现的次数”</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>44</td>
      <td>求0123456789101112131415...中任意位数字</td>
      <td>

```
      +10
 0 ... 9
|0|...|9|
0 + 9   = 9
0 + 9*1 = 9
              +180
  1  0 ...   9   9
|10|11|...|188|189|
10 + 89   = 99
10 + 89*2 = 188
                          +2700
   1   0   0 ...    9    9    9
|190|191|192|...|2887|2888|2889|
100 + 899   = 999
190 + 899*3 = 2887
                                          +36000
    1    0    0    0 ...     9     9     9     9
|2890|2891|2892|2893|...|38886|38887|38888|38889|
1000 + 8999   = 9999
2890 + 8999*4 = 38886

1001 = 190 + 811 = 190 + 270*3 + 1
                              |0|1|2|
                   100 + 270 = 3 7 0
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>45</td>
      <td>字符串拼接排成最小的数</td>
      <td>

```python
def cmpkey(x, y):
    if y + x > x + y:
        return 1
    elif y + x < x + y:
        return -1
    else:
        return 0 
key=functools.cmp_to_key(cmpkey)

key=functools.cmp_to_key(
        lambda x, y: int(y + x) - int(x + y)
    )
```

</td>
      <td>LeetCode 179</td>
    </tr>
    <tr>
      <td>46</td>
      <td>字符串分解</td>
      <td>

```
12258   ('0', '1', ..., '25')

rtl:
    8   1                       dp['8'] = 1
   58   '5'|dp['8'] => 1        dp['58'] = 1
  258   '2'|dp['58'] => 1,
        '25'|dp['8'] => 1       dp['258'] = 2
 2258   '2'|dp['258'] => 2,
        '22'|dp['58'] => 1      dp['2258'] = 3
12258   '1'|dp['2258'] => 3,
        '12'|dp['258'] => 2     dp['12258'] = 5

ltr:
1       1                       dp['1'] = 1
12      dp['1']|'2' => 1
        |'12'                   dp['12'] = 2
122     dp['12']|'2' => 2,
        dp['1']|'22' => 1       dp['122'] = 3
1225    dp['122']|'5' => 3,
        dp['12']|'25' => 2      dp['1225'] = 5
12258   dp['1225']|'8' => 5     dp['12258'] = 5
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>47</td>
      <td>拿礼物</td>
      <td>

```
 1 10  3  8
12  2  9  6
 5  7  4 11
 3  7 16  5

 1←11←14←22
 ↑
13←15←24←30
 ↑        ↑
18←25←29 41
 ↑  ↑
21 32←48←53

dp: [18][25][24][30]
             24  30
     18  25 (29)
dp: [18][25][29][30]
                 30
     18  25  29 (41)
dp: [18][25][29][41]
```

</td>
      <td>Follow-up: LeetCode 741. Cherry Pickup</td>
    </tr>
    <tr>
      <td>48</td>
      <td>“最长不含重复字符的子字符串”</td>
      <td>

```
 a r a b c a c f r
 0
{a}   1
{a,r}   2
   1
  {r,a}   2
  {r,a,b}   3
  {r,a,b,c}   4
       3
      {b,c,a}   3
           5
          {a,c}   2
          {a,c,f}   3
          {a,c,f,r}   4
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>49</td>
      <td>“丑数”</td>
      <td>

```
      2  3  4  5
x2   [4  6        ✓
x3   [6
x5  [10
      2  3  4  5  6
x2         [8        ✓
x3   [6  9
x5  [10
      2  3  4  5  6 -8-
x2           [10
x3      [9              ✓
x5  [10
      2  3  4  5  6  8  9
x2           [10           ✓
x3        [12
x5  [10
      2  3  4  5  6  8  9 10
x2              [12           ✓
x3        [12
x5     [15
      2  3  4  5  6  8  9 10 12
x2                 [16
x3           [15                 ✓
x5     [15
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>50.1</td>
      <td>“字符串中第一个只出现一次的字符”</td>
      <td>

```
0 1 2 3 4 5 6 7 8
a b a c c d e f f
a: [0, 2]
b: [1, 1]
c: [3, 2]
d: [5, 1]
e: [6, 1]
f: [7, 2]
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>50.2</td>
      <td>从字符串中删除字符</td>
      <td></td>
      <td><code>if c in set(s)</code></td>
    </tr>
    <tr>
      <td>50.3</td>
      <td>字符串去重</td>
      <td>

```
"google"
"gogle"
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>50.4</td>
      <td>Anagram</td>
      <td>

```
set('silent') == set('listen')
set('evil') == set('live')
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>50.5</td>
      <td>“字符流中第一个只出现一次的字符”</td>
      <td>

```
g o o g l e
g:0
  g:0, o:1
    g:0, o:-1
      g:-1, o:-1
```

</td>
      <td><code>collections.OrderedDict</code></td>
    </tr>
    <tr>
      <td>51</td>
      <td>“数组中的逆序对”</td>
      <td>

```
   7 5  6 4
[7][5]  [6][4]
+1*1    +1*1
[5,7]   [4,6]
[5,7]   [6]     [4]         +1*2 (5,4), (7,4)
[7]     [6]     [4,5]
[7]     []      [4,5,6]     +1*1 (7,6)
[4,5,6,7]
```

</td>
      <td>归并排序</td>
    </tr>
    <tr>
      <td>52</td>
      <td>“两个链表的第一个公共节点”</td>
      <td>

```
     p1
[1]->[2]->[3]
            \
            [6]->[7]
            /
     [4]->[5]
     p2
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>53.1</td>
      <td>实现 <code>bisect_left</code>, <code>bisect_right</code></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>53.2</td>
      <td><code>[0, ..., n-1]</code> 中缺失的一个数字</td>
      <td>

```
[0, ..., m-1, m+1, ..., n-1]
          =    >          
 0       m-1, m         n-2
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>53.3</td>
      <td>找出数组中任意一个数值等于其下标的元素</td>
      <td>

```
[-3,-1,1,3,5]
       < = >
  0  1 2 3 4
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>54</td>
      <td>“二叉搜索树的第k大节点”</td>
      <td>

```
k = 3
         5
  [2]  /   \
     3       7
    / \     / \
   2   4   6   8
[1]    [3]
```

</td>
      <td>中序遍历</td>
    </tr>
    <tr>
      <td>55.1</td>
      <td>“二叉树的深度”</td>
      <td>

```
      (4)
         1
  (3)  /   \  (2)
     2       3
    / \       \
   4   5       6  (1)
(1)   / (2)
     7
  (1)
```

</td>
      <td>求最短路径有陷阱</td>
    </tr>
    <tr>
      <td>55.2</td>
      <td>“平衡二叉树”</td>
      <td>

```
    (4,T)
         1
(3,T)  /   \  (2,T)
     2       3
    / \       \
   4   5       6  (1,T)
(1,T) / (2,T)
     7
(1,T)
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>56.1</td>
      <td>一个整数数组里只有两个数字只出现一次，其它数字都出现了两次</td>
      <td>

```
[2,4,3,6,3,2,5,5]
2^4^3^6^3^2^5^5 = 0010
__1_            __0_
[2,3,6,3,2]     [4,5,5]
2^3^6^3^2 = 6   4^5^5 = 4
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>56.2</td>
      <td>一个数组中只有一个数字只出现一次，其它数字都出现了三次</td>
      <td></td>
      <td>二进制的每一位加起来，能被3整除的位，那个数的对应位是0，否则是1</td>
    </tr>
    <tr>
      <td>57.1</td>
      <td>“和为s的两个数字”</td>
      <td>

```
s = 15
[1,2,4,7,11,15]
 1          15  = 16
 1       11     = 12
   2     11     = 13
     4   11     = 15
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>57.2</td>
      <td>所有和为s的连续正整数序列</td>
      <td>

```
n = 2:  7.5 7.5
        7   8
n = 3:  5 5 5
        4 5 6
n = 4:  3.25 3.25 3.25 3.25

n = 5:  3 3 3 3 3
        1 2 3 4 5
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>58.1</td>
      <td>“翻转单词顺序”</td>
      <td>

```
"I am a student."   s
".tneduts a ma I"   reversed s
"student. a am I"
"student. a ma I"
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>58.2</td>
      <td>“左旋转字符串”</td>
      <td>

```
  2
"abcdefg"   s
"gfedcba"   reversed s
"cdefgba"
"cdefgab"
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>59.1</td>
      <td>“滑动窗口的最大值”</td>
      <td>

```
max queue: [large, >= medium, >= small]
[2 3 4] 2 6 2 5 1
     4@2
2 [3 4 2] 6 2 5 1
     4@2, 2@3
2 3 [4 2 6] 2 5 1
         6@4
2 3 4 [2 6 2] 5 1
         6@4, 2@5
2 3 4 2 [6 2 5] 1
         6@4, 5@6
2 3 4 2 6 [2 5 1]
             5@6, 1@7
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>59.2</td>
      <td>实现队列的 <code>max()</code></td>
      <td></td>
      <td>同理</td>
    </tr>
    <tr>
      <td>60</td>
      <td>n个骰子点数之和的概率分布</td>
      <td>

```
n <= s <= 6n
        1 2 3 4 5 6  ... 6n
n = 1: [1,1,1,1,1,1, ..., 0]    frequency
n = 2: a2[i] = a1[i-1] + a1[i-2] + a1[i-3]
             + a1[i-4] + a1[i-5] + a1[i-6]
...
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>61</td>
      <td>判断随机抽的5张扑克牌是不是一个顺子</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>62</td>
      <td>约瑟夫环</td>
      <td>

```
m = 3
n = 1, f(1) = 0
n > 1, f(n) = (f(n-1) + 3) % n

n = 2, f(2) = (f(1) + 3) % 2 = 1
      0
          1

n = 3, f(3) = (f(2) + 3) % 3 = 1
      0
          1
        2

n = 4, f(4) = (f(3) + 3) % 4 = 0
      0
          1
    3   2

n = 5, f(5) = (f(4) + 3) % 5 = 3
      0
  4       1
    3   2
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>63</td>
      <td>买卖某股票一次可能获得的最大利润</td>
      <td>

```
[9,11,8,5,7,12,16,14]
 0  2 0 0 2  7 11  9
 9    8 5               (min)
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>64</td>
      <td>利用构造函数/虚函数/函数指针/模板类型求 1+2+...+n</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>65.1</td>
      <td>实现加法器</td>
      <td>

```
数位加
^   0, 0 => 0
    1, 1 => 0
    1, 0 => 1
进位
&   0, 0 => 0
    1, 0 => 0
    1, 1 => 1

a           00111
b           11111
^           11000
&   00111   01110
^           10110
&   01000   10000
^           00110
&   10000  100000
^          100110
&  000000  000000
a + b = 100110
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>65.2</td>
      <td>交换两个变量的值</td>
      <td>

```
a = a + b   sum of a, b
b = a - b   get a using b
a = a - b   get b using a

a = a ^ b   diff of a, b
b = a ^ b   get a using b
a = a ^ b   get b using a
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>66</td>
      <td>“构建乘积数组”</td>
      <td>

```
B0      C0  [1][A1,A2,...,An-2,An-1]  Dn-1
B1      C1  [A0]  [A2,...,An-2,An-1]  Dn-2
B2      C2  [A0,A1]   [...An-2,An-1]  Dn-3
    ...
Bn-2  Cn-2  [A0,A1,...,An-3]  [An-1]  D1
Bn-1  Cn-1  [A0,A1,...,An-3,An-2][1]  D0
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>67</td>
      <td>实现 <code>atoi()</code></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <td>68.1</td>
      <td>二叉搜索树中两个节点的最底公共祖先</td>
      <td>

```
          8
        /   \       3 < 4 < 6
      4       9         4            [4]
    /   \             /   \         /
  2       6                [6]
 / \     / \         \     /     /
1   3   5   7        [3]       [1]
```

</td>
      <td></td>
    </tr>
    <tr>
      <td>68.2</td>
      <td>树中两个节点的最底公共祖先</td>
      <td>

```
            A
    (2)   /   \
        B       C
(1)   /   \
    D       E (1)
   / \     /|\
 [F]  G  [H]I J
(1)     (1)
```

</td>
      <td></td>
    </tr>
  </tbody>
</table>
