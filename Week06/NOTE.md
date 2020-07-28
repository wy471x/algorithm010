## 递归代码模板

```java
// Java
public void recur(int level, int param) { 
  // terminator 
  if (level > MAX_LEVEL) { 
    // process result 
    return; 
  }
  // process current logic 
  process(level, param); 
  // drill down 
  recur( level: level + 1, newParam); 
  // restore current status 
 
}
```

## 分治代码模板

```python
# Python
def divide_conquer(problem, param1, param2, ...): 
  # recursion terminator 
  if problem is None: 
	print_result 
	return 

  # prepare data 
  data = prepare_data(problem) 
  subproblems = split_problem(problem, data) 

  # conquer subproblems 
  subresult1 = self.divide_conquer(subproblems[0], p1, ...) 
  subresult2 = self.divide_conquer(subproblems[1], p1, ...) 
  subresult3 = self.divide_conquer(subproblems[2], p1, ...) 
  …

  # process and generate the final result 
  result = process_result(subresult1, subresult2, subresult3, …)
	
  # revert the current level states
```

## 动态规划（Dynamic Programming）关键点

1. > 动态规划和递归或者分治没有根本上的区别（关键看有无最优子结构）

2. > 共性：找到重复子问题

3. > 差异性：最优子结构、中途可以淘汰次优解



## 第六周作业

## 本周作业

### 中等

- [最小路径和](https://leetcode-cn.com/problems/minimum-path-sum/)（亚马逊、高盛集团、谷歌在半年内面试中考过）
- [解码方法](https://leetcode-cn.com/problems/decode-ways)（亚马逊、Facebook、字节跳动在半年内面试中考过）
- [最大正方形](https://leetcode-cn.com/problems/maximal-square/)（华为、谷歌、字节跳动在半年内面试中考过）
- [任务调度器](https://leetcode-cn.com/problems/task-scheduler/)（Facebook 在半年内面试中常考）
- [回文子串](https://leetcode-cn.com/problems/palindromic-substrings/)（Facebook、苹果、字节跳动在半年内面试中考过）

### 困难

- [最长有效括号](https://leetcode-cn.com/problems/longest-valid-parentheses/)（字节跳动、亚马逊、微软在半年内面试中考过）
- [编辑距离](https://leetcode-cn.com/problems/edit-distance/)（字节跳动、亚马逊、谷歌在半年内面试中考过）
- [矩形区域不超过 K 的最大数值和](https://leetcode-cn.com/problems/max-sum-of-rectangle-no-larger-than-k/)（谷歌在半年内面试中考过）
- [青蛙过河](https://leetcode-cn.com/problems/frog-jump/)（亚马逊、苹果、字节跳动在半年内面试中考过）
- [分割数组的最大值](https://leetcode-cn.com/problems/split-array-largest-sum)（谷歌、亚马逊、Facebook 在半年内面试中考过）
- [学生出勤记录 II ](https://leetcode-cn.com/problems/student-attendance-record-ii/)（谷歌在半年内面试中考过）
- [最小覆盖子串](https://leetcode-cn.com/problems/minimum-window-substring/)（Facebook 在半年内面试中常考）
- [戳气球](https://leetcode-cn.com/problems/burst-balloons/)（亚马逊在半年内面试中考过）

## 下周预习

### 预习题目：

- [实现 Trie (前缀树) ](https://leetcode-cn.com/problems/implement-trie-prefix-tree/#/description)
- [单词搜索 II ](https://leetcode-cn.com/problems/word-search-ii/)
- [岛屿数量](https://leetcode-cn.com/problems/number-of-islands/)
- [有效的数独](https://leetcode-cn.com/problems/valid-sudoku/description/)
- [ N 皇后](https://leetcode-cn.com/problems/n-queens/)
- [单词接龙](https://leetcode-cn.com/problems/word-ladder/)
- [二进制矩阵中的最短路径](https://leetcode-cn.com/problems/shortest-path-in-binary-matrix/)

