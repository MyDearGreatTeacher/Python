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

