os 模块，主要与操作系统打交道

`Operating system`

为什么需要这个模块？
其实主要是用代码来对计算机进行操作，有点类似于Dos系统，在没有鼠标和交互界面的情况下，使用os语言执行系统操作，如：新建文件（夹），删除文件（夹），查看文件属性等等。


```python
import os

1. os.getcwd()    #获取当前路径 get current working directory 类似于 cd
>>>'D:\\Python'

2. os.listdir()   #列出目录中的内容 list directory 返回的是一个 list， 类似于 ls
>>>[['control_position_test_data.txt', 'control_position_test_data_2019-10-04_1.txt', 'control_position_test_data_2019-10-04_2.txt', 'control_position_test_data_2019-10-04_3.txt']

任意文件也可以，例如：
 
2.2 os.listdir('c:/tmp')  #查看路径下的文件，返回的是一个 list
>>>['LamDAApplicationStartlog.txt', 'libwap_g.so.1.zip', 'wap_mon_g', 'wap_mon_g.zip']


3. os.mkdir()    #新建一个创建目录(文件夹)  注意：如果该路径下已经有一个同名的目录，则会报错
os.mkdir('c:/test') #新建一个目录


4. os.rmdir()    #删除目录
os.rmdir('c:/test') #把刚才建的目录给删除了

```

Ref: https://blog.51cto.com/pmghong/1353340
