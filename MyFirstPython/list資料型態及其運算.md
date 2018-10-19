# 列表|串列(list)資料型態及其運算

>* python提供內建的list類別

### 建立list
```
list1 = list() 
list1 = [] 

list2 = list([2, 3, 4])
list2 = [2, 3, 4] 

list3 = list(["red", "green", "blue"]) 
list4 = list(range(3, 6))
list5 = list("abcd") 
```

### list的各種函數1
```
[動手做]下列範例會產生何種結果
list1 = [21, 33, 14, 12, 32,98]

len(list1)
max(list1)
min(list1)
sum(list1) 
```

### list的各種函數2:串列的加法|乘法與分割運算

[動手做]下列範例會產生何種結果
```
list1 = [21, 23, 25]
list2 = [11, 92]

list3 = list1 + list2
list3
list4 = 3 * list1
list4
list5 = list3[2:4]
list5
```
### list的各種函數3:串列的分割運算
```
items = "Welcome to the MyFirstCTF".split() 
print(items)

items = "314#123#738#445".split("#")
print(items)
```
### list的各種函數4:more
```
加一元素到串列的尾端:append()
回傳元素x 出現於串列的次數:count()
附加在l中所有元素於串列:extend()
回傳在串列中第一次出現元素x的索引:index()
將串列中的元素加以反轉:reverse()
由小至大排序串列中的元素:sort()
```
### list的超強大功能:序列拆解
```
a=[12,212,321,325]
x,y,z,k = a
z
```

### list的超強大功能list comprehension列表生成式 
```
A list comprehension consists of brackets containing an expression followed by a for clause, 
then zero or more for or if clauses. 
The result will be a new list resulting from evaluating the expression 
in the context of the for and if clauses which follow it. 

https://en.wikipedia.org/wiki/List_comprehension
```

```
list1 = [x for x in range(0,5)] # Returns a list of 0, 1, 2, 4
list1 
list2 = [0.5 * x for x in list1] 
list2
list3 = [x for x in list2 if x < 1.5]
list3
```

# 綜合練習
```
import random
import time

x = list(range(10000))		#產生成列表
y = set(range(10000))		#產生成集合
z = dict(zip(range(1000),range(10000)))		#產生成字典
r = random.randint(0, 9999)	#產生成亂數

start = time.time()
for i in range(9999999):
    r in x 				#測試清單列表中是否包含某個元素
print('list,time used:', time.time()-start)

start = time.time()
for i in range(9999999):
    r in y					#測試集合中是否包含某個元素
print('set,time used:', time.time()-start)

start = time.time()
for i in range(9999999):
    r in z					#測試字典中是否包含某個元素
print('dict,time used:', time.time()-start)
```
