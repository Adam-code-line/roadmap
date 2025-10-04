> 📺 强烈推荐观看 [你是天才，所以不用学数据结构](https://www.bilibili.com/video/BV1RTxpzTEZ8/) 🎉

# 数据结构与算法扫盲文档

## 1. 变量 (Variable)

变量是程序中用来存储数据的“容器”，就像贴了标签的盒子。

### 示例（Python）

```python
age = 18      # 整数
name = "Tom"  # 字符串
pi = 3.14     # 小数
```

> 理解：变量就是把数据保存起来，给它一个名字，方便后续使用。

---

## 2. 字符串 (String)

字符串是由**字符组成的序列**，常用于表示文本。

### 示例

```python
text = "Hello, world!"
print(text[0])      # 输出 H
print(len(text))    # 输出字符串长度 13
print(text.upper()) # 输出 HELLO, WORLD!
```

> 理解：字符串可以看作是“字符的数组”。

---

## 3. 数组 (Array)

数组是一组**连续存储的元素**，每个元素通过**下标**访问。

### 示例

```python
arr = [10, 20, 30, 40]
print(arr[0])    # 输出 10
arr[2] = 99      # 修改元素
print(arr)       # [10, 20, 99, 40]
```

> 理解：数组适合快速按位置读取数据，但插入删除可能很慢。

---

## 4. 链表 (Linked List)

链表由多个“节点”组成，每个节点包含**数据**和**指向下一个节点的指针**。
不像数组那样连续存储。

### 示例（单向链表）

```python
class Node:
    def __init__(self, value):
        self.value = value
        self.next = None

# 构建链表 1 -> 2 -> 3
head = Node(1)
head.next = Node(2)
head.next.next = Node(3)

print(head.value)          # 输出 1
print(head.next.value)     # 输出 2
print(head.next.next.value)# 输出 3
```

> 理解：链表更灵活，适合频繁插入删除。

---

## 5. 队列 (Queue)

队列是一种**先进先出 (FIFO)** 的数据结构，就像排队买票。

### 示例

```python
from collections import deque

q = deque()
q.append(1)  # 入队
q.append(2)
print(q.popleft())  # 出队 → 1
print(q.popleft())  # 出队 → 2
```

> 理解：先来的先走，非常公平。

---

## 6. 栈 (Stack)

栈是一种**后进先出 (LIFO)** 的数据结构，就像一摞盘子。

### 示例

```python
stack = []
stack.append(1)  # 入栈
stack.append(2)
print(stack.pop())  # 出栈 → 2
print(stack.pop())  # 出栈 → 1
```

> 理解：后放进去的先拿出来，常用于函数调用、括号匹配。

---

## 7. 二叉树 (Binary Tree)

二叉树是一种层次结构，每个节点最多有两个子节点：**左子节点**和**右子节点**。

### 示例

```python
class TreeNode:
    def __init__(self, val):
        self.val = val
        self.left = None
        self.right = None

# 构建二叉树
root = TreeNode(1)
root.left = TreeNode(2)
root.right = TreeNode(3)

print(root.left.val)   # 输出 2
print(root.right.val)  # 输出 3
```

> 理解：树结构用于表达层次关系，如家谱、文件夹目录。

---

## 8. 图 (Graph)

图由**顶点 (Vertex)** 和**边 (Edge)** 构成，可用于表示“关系网络”。

### 示例（邻接表表示）

```python
graph = {
    "A": ["B", "C"],
    "B": ["A", "D"],
    "C": ["A", "D"],
    "D": ["B", "C"]
}
print(graph["A"])  # ['B', 'C']
```

> 理解：图用于表示复杂关系，如社交网络。

---

## 9. 哈希表 (Hash Table)

哈希表通过**键 (Key) → 值 (Value)** 的映射快速存取数据。
它利用**哈希函数**将 Key 映射到存储位置。

### 示例（Python 字典）

```python
student = {"Alice": 90, "Bob": 85}
print(student["Alice"])  # 90
student["Tom"] = 92      # 添加新数据
print(student)
```

> 理解：哈希表能在接近 O(1) 的时间完成查找，非常高效。

---

# 总结

* **变量**：存储数据
* **字符串**：字符序列
* **数组**：连续存储，快速索引
* **链表**：节点灵活，插入删除快
* **队列**：先进先出
* **栈**：后进先出
* **二叉树**：层次关系
* **图**：复杂关系网络
* **哈希表**：快速查找

---