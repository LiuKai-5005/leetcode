
`.md`是`markdown`的缩写，markdown是一种编辑博客的语言。

更多是为了排版好看，想想之前写论文用`LaTex`是一样的，虽然用`Word`一样可以写，但是排版还是很难看。

下面就是一些练习的例子，知识点。

Contents
-----------
# 1 Two Sum

# 换行
`<br>`

* practice for leetcode problems

# 排版
  * 使用 星号 是 加一个 <br>
  *斜体*<br>
  **粗体**<br>
  ~~删除~~<br>


# 引用
>引用别人的话，需要使用`>`符号， 这一段灰色打底

# 打标签
`30岁大龄码农的成长之路` `刷题找工作`
``类似于 '' ``
`emoji`符号也是支持的，例如 :+1: :-1: :shipit: :star: :moon: :apple: :peach: :watermelon: :lemon: :banana:


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
[CSDN例子](https://blog.csdn.net/u012067966/article/details/50736647)
[官方说明](https://help.github.com/cn/github/writing-on-github/basic-writing-and-formatting-syntax#links)


