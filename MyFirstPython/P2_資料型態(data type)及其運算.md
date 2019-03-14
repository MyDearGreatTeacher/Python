# Python程式設計{基礎課程}

# 2_1.各種資料型態(data type)及其運算[1][2][3][4]...[X]
```
識別字與關鍵字

數字型(numeric)資料型態及其運算
Integral 類型:整數類型|布爾型
浮點類型:浮點數|複數
二進位八進位十進位十六進位數字

字串(string)資料型態及其運算

文數字編碼與解碼
如何操縱Unicode字串

Collection Data Types組合類型資料型態 
列表|串列(list)資料型態及其運算
元組(tuple)資料型態及其運算
辭典|字典(dic)資料型態及其運算
集合(set)資料型態及其運算
```
# 數字()資料型態及其運算
```
a = 1.5344
int(a)
float(a)
complex(a)
```


```
17/3
17//3
17 % 3 

5*3 +2
```
```
1457986 除以 113   
商數=1457986 // 113
餘數=1457986 % 113

```
### 数学函数
```
x=4.9
ceil(x)
floor(x)
```
# 字串(string)資料型態及其運算
```
Python不支援單字元類型，單字元在 Python 中也是作為一個字串使用。
Python訪問子字串，可以使用方括號來截取字串
```
```
#!/usr/bin/python
 
var1 = 'Hello World!'
var2 = "Python Runoob"
 
print "var1[0]: ", var1[0]
print "var2[1:5]: ", var2[1:5]
```
# 列表|串列(list)資料型態及其運算[底下程式請用python 2執行]
```
#!/usr/bin/python
 
list1 = ['physics', 'chemistry', 1997, 2000]
list2 = [1, 2, 3, 4, 5, 6, 7 ]
 
print "list1[0]: ", list1[0]
print "list2[1:5]: ", list2[1:5]
```

```
#!/usr/bin/python
# -*- coding: UTF-8 -*-
 
list = []          ## 建立空的list
list.append('Google')   ## 使用 append() 添加元素
list.append('KSU當選')
print list
```

# 辭典|字典(dic)資料型態及其運算

dict = {key1 : value1, key2 : value2 }
```
dict = {'a': 1, 'b': 2, 'b': '3'}
dict['b']
dict

dict['b']==>答案為何?
dict會印出甚麼?

HINT:鍵一般是唯一的，如果重複最後的一個鍵值對會替換前面的，值不需要唯一。
```

```
【程式閱讀題】下列程式執行後結果為何??


#!/usr/bin/env python
#coding=utf-8
 
dict = {'Name': 'Zara', 'Age': 7, 'Class': 'First'}
 
print "dict['Name']: ", dict['Name']
print "dict['Age']: ", dict['Age']
```

### 辭典|字典(dic)的運算:更新字典內容
```
#!/usr/bin/env python
#coding=utf-8

dict = {'Name': 'Zara', 'Age': 27, 'Class': 'First'}
 
dict['Age'] = 38 
dict['School'] = "KSU" 
 
print "dict['Age']: ", dict['Age']
print "dict['School']: ", dict['School']
```
### 字典內置函數&方法
```
http://www.runoob.com/python/python-dictionary.html
```

### 運算子:
>* Arithmetic Operators算術運算子
>* 餘數運算子 (remainder|modulo)
>* Membership Operator
>* Comparison Operators
>* Logical Operators邏輯運算子
>* 關係運算子

### 組合類型資料型態的高級特性:切片|迭代 |列表生成式 |生成器|迭代器

# 2.2.數字型(numeric)資料型態及其運算

#### 餘數運算子 (remainder|modulo)
```
題目:將以秒表示的總時間長，分別取得分鐘數及剩餘的秒數。
```
```
#!/usr/bin/env python
#coding=utf-8

seconds = eval(input("Enter an integer for seconds: "))

minutes = seconds // 60     # Find minutes in seconds
remainingSeconds = seconds % 60   # Seconds remaining
print(seconds, "seconds is", minutes, "minutes and", remainingSeconds, "seconds")
```

# 2.3:二進位,八進位,十進位與十六進位

>* Python有許多內建函數(built-in functions)
>* https://docs.python.org/3/library/functions.html
>* https://docs.python.org/2/library/functions.html
>* https://www.programiz.com/python-programming/methods/built-in

```
題目:將十六進位的0xabcd寫出其二進位,八進位,十進位的表示
```

