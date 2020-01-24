目录
==========================
md是markdown的缩写，markdown是一种编辑博客的语言。

LeetCode
-----------
# 1 Two Sum


LeetCode

刷题找工作 <br>
* practice for leetcode problems

# 排版
  使用Tab按键<br>
  * 使用 星号
  *斜体*




# 引用
>引用别人的话，需要使用">"符号

# 打标签
`30岁大龄码农的成长之路` `刷题找工作`

# 插入代码 
>之后加上你的编程语言
```Python
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

```

# 插入图片:
![](http://www.baidu.com/img/bdlogo.gif)  

`https://github.com/ 你的用户名 / 你的项目名 / raw / 分支名 / 存放图片的文件夹 / 该文件夹下的图片`



# 超链接:
[参考链接](https://blog.csdn.net/u012067966/article/details/50736647)





