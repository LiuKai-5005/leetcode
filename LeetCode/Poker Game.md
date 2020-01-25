题目: 一副从1到n的牌，每次从牌堆顶取一张放桌子上，再取一张放牌堆底，直到手中没牌，最后桌子上的牌是从1到n有序，设计程序，输入n，输出牌堆的顺序数组
<br>
`小米面试题`
`Xiaomi`
`queue`

这道题我一开始想的应该是用双向队列，类似于传递热马铃薯问题（hot potato game），实际上是用一个双向队列，循环放牌，另一个数组接住pop出来的牌。
类推：valid parenthesis 为什么需要用stack而不是队列，其实，类似于“消消乐”这种需要抵消或者及时查看栈顶的操作的时候，我们需要stack，即list。

当然，这需要使用 from collections import deque

具体用法和list类似，无非多了两个左侧的append 和 pop 即 
queue.appendleft('xx') --> 注意区别，和list.insert('xx')不同，此操作只有O(1)的复杂度，不涉及数组的平移，类似linked list
queue.popleft()

```python

from collections import deque

def poker(n: int) -> list:

    ans = []
    flag = True
    queue = deque(range(1,n + 1))
    
    while len(queue) > 0:
        if flag:
            ans.append(queue.popleft())   #pop left and append into ans
        else:
            queue.append(queue.popleft()) #pop left and append into queue
        flag = not flag                 #reverse the flag
    return ans
