# [4]函式/函數/function

>* 函數是組織好的，可重複使用的，用來實現單一，或相關聯功能的程式碼片段。
>* 函數能提高應用的模組性，和代碼的重複利用率。
>* Python提供了許多內建函數，比如print()。
>* 使用者也可以自己創建函數，這被叫做使用者自訂函數。

### 定義語法:
>* 函數代碼塊以 def 關鍵字開頭，後接函數識別字名稱和圓括號()。
>* 任何傳入參數和引數必須放在圓括號中間。圓括號之間可以用於定義參數。
>* 函數的第一行語句可以選擇性地使用文檔字串—用於存放函數說明。
>* 函數內容以冒號起始，並且縮排。
>* return [運算式] 結束函數，選擇性地返回一個值給調用方。不帶運算式的return相當於返回 None。
>* 函式包含標頭和主體。
>* 標頭(header)起源於def關鍵字，後接函式名稱和參數，最後以冒號結尾。 

```
def functionname(parameters):
   "函數_文檔字串"
   function_suite
   return [expression]
```

# 功能==>函數

請分別計算 1 到 10，20 到 37，以及 35 到 49 間整數的總和?

你會怎麼做

方法一:
```
sum = 0
for i in range(1, 10):
    sum += i
print("Sum from 1 to 10 is", sum)

sum = 0
for i in range(20, 37):
    sum += i
print("Sum from 20 to 37 is", sum)
sum = 0
for i in range(35, 49):
    sum += i
print("Sum from 35 to 49 is", sum)
```

方法二:
```
def sum(i1, i2):
    result = 0
    for i in range(i1, i2):
        result += i
    return result

def main():
    print("Sum from 1 to 10 is", sum(1, 10)) 
    print("Sum from 20 to 37 is", sum(20, 37))
    print("Sum from 35 to 49 is", sum(35, 49))

main() # Call the main function
```
形式參數 vs 實質參數(引數)

>* 形式參數==定義於函數標頭的變數
>* 實質參數(引數)==當函式被呼叫時，你必須給予的參數則被稱為
>* 函式會使用關鍵字return 回傳一個結果數值，此數值被稱為回傳值。

# 抽象(abstraction)==>函數     計算費氏序列:

計算前十個費氏序列
```
fibs = [0, 1] 
for i in range(8): 
    fibs.append(fibs[-2] + fibs[-1]) 
    
 >>> fibs 
```
計算前個費氏序列
```
fibs = [0, 1] 
num = int(input('How many Fibonacci numbers do you want? ')) 
for i in range(num-2): 
    fibs.append(fibs[-2] + fibs[-1]) 
print(fibs) 
```

抽象(abstraction)==>函數
```
num = input('How many numbers do you want? ') 
print(fibs(num)) 
```
```
def fibs(num): 
    result = [0, 1] 
    for i in range(num-2): 
        result.append(result[-2] + result[-1]) 
    return result 

>>> fibs(10) 
>>> fibs(15) 
```
### docstring:為函式註解

撰寫函式註解
```
def square(x): 
   'Calculates the square of the number x.' 
   return x * x 
```
讀取函式註解1:使用__doc__ 
```
>>> square.__doc__ 
```
讀取函式註解2:使用help()內建函式
```
>>> help(square)
```
### 函式與return value

所有的函式都return value。如果你沒有告訴它要返回什麼，他就會返回None(也就是有返回值) 

```
def test(): 
    print('This is printed') 
    return 
    print('This is not printed at all') 

>>> x = test()
>>> x 
>>> print(x) 
```

# 函式呼叫:

how arguments are passed to functions in Python??

傳值呼叫(pass by value) vs 傳參考呼叫(pass by reference) or "call-by-object," or "call-by-object-reference" OR call-by-assignment

https://jeffknupp.com/blog/2012/11/13/is-python-callbyvalue-or-callbyreference-neither/

https://stackoverflow.com/questions/986006/how-do-i-pass-a-variable-by-reference

```
================================================================
【Python 練習實例47】練習撰寫函式swap(a,b)
寫一個函式將輸入的兩個變數值互換
================================================================
#!/usr/bin/python
# -*- coding: UTF-8 -*-
 
def swap(a,b):
    a,b = b,a
    return (a,b)
 
if __name__ == '__main__':
    x = 10
    y = 20
    print 'x = %d,y = %d' % (x,y)
    x,y = swap(x,y)
    print 'x = %d,y = %d' % (x,y)
```
```
def try_to_change_list_contents(the_list):
    print('got', the_list)
    the_list.append('four')
    print('changed to', the_list)

outer_list = ['one', 'two', 'three']

print('before, outer_list =', outer_list)
try_to_change_list_contents(outer_list)
print('after, outer_list =', outer_list)
```
```
def try_to_change_list_reference(the_list):
    print('got', the_list)
    the_list = ['and', 'we', 'can', 'not', 'lie']
    print('set to', the_list)

outer_list = ['we', 'like', 'proper', 'English']

print('before, outer_list =', outer_list)
try_to_change_list_reference(outer_list)
print('after, outer_list =', outer_list)
``` 
```
Techs = ['MIT', 'Caltech']
Ivys = ['Harvard', 'Yale', 'Brown']

Univs = [Techs, Ivys]
Univs1 = [['MIT', 'Caltech'], ['Harvard', 'Yale', 'Brown']]

print 'Univs =', Univs
print 'Univs1 =', Univs1
print Univs == Univs1


That Univs and Univs1 are bound to different objects can be verified using the
built-in Python function id, which returns a unique integer identifier for an
object. This function allows us to test for object equality

print Univs == Univs1 #test value equality
print id(Univs) == id(Univs1) #test object equality
print 'Id of Univs =', id(Univs)
print 'Id of Univs1 =', id(Univs1)
```
```
#!/usr/bin/python 
# -*- coding: UTF-8 -*- 

def crypt(source, key):
    from itertools import cycle
    result = ''
    temp = cycle(key)
    for ch in source:
        result = result + chr(ord(ch) ^ ord(next(temp)))
    return result

source = 'BreakALLCTF_IknowhowtoXORRRRing'
key = 'HappyHackingHigh'

print('未加密的明文:'+source)
encrypted = crypt(source, key)
print('加密過的密文:'+encrypted)
decrypted = crypt(encrypted, key)
print('解密過的答案:'+decrypted)
print('使用的金鑰:'+ key)
```

# 函式與參數

>* Default arguments預設參數
>* Positional arguments位置參數
>* Keyword arguments關鍵字參數

### 預設參數值的函式

>* Python允許定義含有預設參數值的函式。
>* 當呼叫函式時，若沒有傳送參數，此時將使用預設參數值。

```
#!/usr/bin/python 
# -*- coding: UTF-8 -*- 

def printArea(width = 11, height = 12):
    area = width * height
    print("width:", width, "\theight:", height, "\tarea:", area)

printArea() # Default arguments width = 1 and height = 2
printArea(4, 2.5) # Positional arguments width = 4 and height = 2.5
printArea(height = 5, width = 3) # Keyword arguments width 
printArea(width = 1.2) # Default height = 2
printArea(height = 6.2) # Default widht = 1
```

### collectiong parameters(任意數量的參數):* 與 **

如何撰寫擁有任意數量參數的函式:
```
def print_params(*params): 
    print(params) 
```
```
>>> print_params('Testing') 
>>> print_params(1, 2, 3) 
```
>* return的是tuple資料型態

如何撰寫擁有任意數量參數的函式:可以和一般參數齊用
```
def print_params_2(title, *params): 
    print(title) 
    print(params)
```
```
>>> print_params_2('Params:', 1, 2, 3)
>>> print_params_2('Nothing:') 
```
如何撰寫擁有任意數量參數的函式:無法支援關鍵字參數??如何支援關鍵字參數
```
>>> print_params_2('Hmm...', something=42) 
```
如何撰寫擁有任意數量參數的函式:支援關鍵字參數==>使用**
```
def print_params_3(**params): 
    print(params) 

>>> print_params_3(x=1, y=2, z=3) 
```
return的是dict(字典資料型態)

##### 測試看看
```
def print_params_4(x, y, z=3, *pospar, **keypar): 
    print(x, y, z) 
    print(pospar) 
    print(keypar) 

>>> print_params_4(1, 2, 4, 5, 6, 7, foo=1, bar=2)

>>> print_params_4(1, 2) 
```
```
def store(data, *full_names): 
   for full_name in full_names: 
       names = full_name.split() 
       if len(names) == 2: names.insert(1, '') 
       labels = 'first', 'middle', 'last' 
       for label, name in zip(labels, names): 
           people = lookup(data, label, name) 
           if people: 
              people.append(full_name) 
           else: 
              data[label][name] = [full_name] 
```
#### 小小測驗:執行下列程式並說明其結果
```
>>> def add(x, y): return x + y 

>>> params = (1, 2) 

#tuple要使用*
>>> add(*params)
```
#### 小小測驗:執行下列程式並說明其結果
```
def hello_3(greeting='Hello', name='world'): 
    print('{}, {}!'.format(greeting, name)) 


>>> hello_3() 
>>> hello_3('Greetings') 
>>> hello_3('Greetings', 'universe') 
>>> hello_3(name='GGGGGGoood') 

#字典dict要使用**
>>> params = {'name': 'Sir Simon Rattle', 'greeting': 'To my Great Conductor'} 
>>> hello_3(**params) 
```

# 函式與回傳值

>* Python的函式是否有無回傳值，端視函式是否有無return敘述。
>* 若函式沒有回傳值，預設是回傳一None特殊值。因此，沒有回傳值的函式也稱為None函式。
>* None值可以指定給一變數，表示此變數沒有參考到任何的物件

無回傳值的函式
```
#!/usr/bin/python 
# -*- coding: UTF-8 -*- 

# Print grade for the score 
def printGrade(score):
    if score >= 90.0:
        print('A')
    elif score >= 80.0:
        print('B')
    elif score >= 70.0:
        print('C')
    elif score >= 60.0:
        print('D')
    else:
        print('F')

def main():
    score = eval(input("Enter a score: "))
    print("The grade is ", end = "")
    printGrade(score)

main() # Call the main function
```

有回傳值的函式
```
#!/usr/bin/python 
# -*- coding: UTF-8 -*- 

# Return the grade for the score 
def getGrade(score):
    if score >= 90.0:
        return 'A'
    elif score >= 80.0:
        return 'B'
    elif score >= 70.0:
        return 'C'
    elif score >= 60.0:
        return 'D'
    else:
        return 'F'

def main():
    score = eval(input("Enter a score: "))
    print("The grade is", getGrade(score))

main() # Call the main function
```

多個回傳值的函式
```
#!/usr/bin/python 
# -*- coding: UTF-8 -*- 

def sort(number1, number2):
    if number1 < number2:
        return number1, number2
    else:
        return number2, number1

num1, num2 = sort(31, 25)

print("num1 is", num1)
print("num2 is", num2)
```

### 作業:撰寫十進位轉換為十六進位的程式

```
# Convert a decimal to a hex as a string 
def decimalToHex(decimalValue):
    hex = ""
 
    while decimalValue != 0:
        hexValue = decimalValue % 16 
        hex = toHexChar(hexValue) + hex
        decimalValue = decimalValue // 16
    
    return hex
  
# Convert an integer to a single hex digit in a character 
def toHexChar(hexValue):
    if 0 <= hexValue <= 9:
        return chr(hexValue + ord('0'))
    else:  # 10 <= hexValue <= 15
        return chr(hexValue - 10 + ord('A'))

def main():
    # Prompt the user to enter a decimal integer
    decimalValue = eval(input("Enter a decimal number: "))

    print("The hex number for decimal", 
        decimalValue, "is", decimalToHex(decimalValue))
  
main() # Call the main function
```
### 作業:撰寫計算任意數目的黑洞數

https://zh.wikipedia.org/wiki/黑洞數
```
2位數的狀況:沒有黑洞，只有1個5成員的循環
3位數的狀況:有1個黑洞,495==>954-459=495
4位數的狀況:有1個黑洞,6174==>7641-1467=6174
5位數的狀況:沒有黑洞，有3個循環
6位數的狀況:有2個黑洞631764、549945，還有1個7個成員的循環
7位數的狀況:沒有黑洞，只有1個8成員的循環
8位數的狀況:有2個黑洞63317664、97508421，還有2個循環
9位數的狀況:有2個黑洞554999445、864197532，還有1個14個成員的循環
10位數的狀況:有3個黑洞6333176664、9753086421、9975084201，還有5個循環
```

### 作業:韓信是如何點兵的??

韓信為了不讓敵人知道自己的兵力有多少， 士兵報數時先從1至3報數，再1至5重新報數，再1至7重新報數，只需記下最佳一名士兵每次報數是錯，即可快速計算出自己有多少士兵。

# 變數的有效範圍

變數的有效範圍(Scope)：變數在程式可參考的範圍。

>* 區域變數(local variable):宣告在函式內部的變數
>* 全域變數(global variables):宣告在所有函式外部的變數

```
x = 111

def f1():
    x = 222
    print(x) 

f1()
print(x) 
```

```
globalVar = 1

def f1():
    localVar = 2
    print(globalVar)
    print(localVar)

f1()
print(globalVar)
print(localVar)  # Out of scope. This gives an error
```

```
sum = 10

for i in range(0, 15):
    sum += i

print(i)
print(sum)
```
```
x = 1

def increase():
    global x
    x =  x + 1
    print(x) 

increase()
print(x)
```

遞迴函式的呼叫次數==>全域變數的應用

# 匿名函數==>lambda 運算式

>* 匿名函數==沒有函數名稱、臨時使用的小函數
>* 使用lambda 運算式來宣告匿名函數
>* lambda 運算式只能包含一個運算式， 不允許複雜的語句，但運算式中可呼叫其他函數

#### 把lambda運算式當做函數
```
f1 = lambda x, y, z: x+2y+3z
print(f(2,3,1))
```

#### 使用預設值參數
```
f2 = lambda x, y=2, z=4: x+2y+3z
print(f2(2))

print(f2(2,z=3, y=4)) #使用關鍵參數呼叫
```

#### 在lambda 運算式中呼叫其他函式(重要技術)
```
def myfunc(m):
    return m*m

my_list = [1, 3, 5, 7, 9]

#使用python的map()
map(lambda x:myfunc(x), my_list)
```

### lambda 運算式與區域變數{常見錯誤}

```
r ＝ []
for x in range(10):
 r.append(lambda: x**3)

r[0]()
r[1]()
r[5]()
r[7]()
r[9]()
```

```
r ＝ []
for x in range(10):
 r.append(lambda m=x: m**3)

r[0]()
r[1]()
r[5]()
r[7]()
r[9]()
```

# 遞迴函式 ==> recursive vs iterative(loop)
```
[程式開發作業]費氏數列
[程式開發作業]1+2+3+....+n
[程式開發作業]n!
[程式開發作業]x的n次方
[程式開發作業]二項係數
[程式開發作業][Ackermann函式](https://en.wikipedia.org/wiki/Ackermann_function)
[程式開發作業]河內塔
[程式開發作業]八皇后問題
[程式開發作業]binary search二元搜尋法
```
### 費氏數列Fibonacci sequence:recursive vs iterative(loop)

```
費氏數列Fibonacci sequence又稱黃金分割數列
0、1、1、2、3、5、8、13、21、34、……。

在數學上，費波那契數列是以遞迴的方法來定義：
F(0) = 0    (n=0)
F(1) = 1    (n=1)
F(n) = F(n-1)+ F(n-2)(n=>2)
```

方法一:使用iterative
```
#!/usr/bin/python
# -*- coding: UTF-8 -*-
 
def fib(n):
    a,b = 1,1
    for i in range(n-1):
        a,b = b,a+b
    return a
 
print fib(10)
```

方法二:使用recursive
```
#!/usr/bin/python
# -*- coding: UTF-8 -*-

def fib(n):
    if n==1 or n==2:
        return 1
    return fib(n-1)+fib(n-2)

print fib(10)
```
```
================================================================
【Python 練習實例28】
有5個人坐在一起，
問第五個人多少歲？他說比第4個人大2歲。
問第4個人歲數，他說比第3個人大2歲。
問第三個人，又說比第2人大兩歲。
問第2個人，說比第一個人大兩歲。
最後問第一個人，他說是10歲。
請問第五個人多大？
================================================================
```
### x的n次方

方法一:使用iterative
```
def power1(x, n): 
    result = 1 
    for i in range(n): 
        result *= x 
    return result 
```
方法二:使用recursive
```
def power2(x, n): 
   if n == 0: 
      return 1 
   else: 
      return x * power(x, n - 1)
```

## 搜尋演算法

### Sequential Search循序搜尋法

>* http://interactivepython.org/runestone/static/pythonds/SortSearch/TheSequentialSearch.html

```
def sequentialSearch(alist, item):
	    pos = 0
	    found = False
	
	    while pos < len(alist) and not found:
	        if alist[pos] == item:
	            found = True
	        else:
	            pos = pos+1
	
	    return found
	
testlist = [1, 2, 32, 8, 17, 19, 42, 13, 0]
print(sequentialSearch(testlist, 3))
print(sequentialSearch(testlist, 13))
```

### binary search二元搜尋法

recursive
```
def search(sequence, number, lower, upper): 
    if lower == upper: 
        assert number == sequence[upper] 
        return upper 
    else: 
        middle = (lower + upper) // 2 
        if number > sequence[middle]: 
           return search(sequence, number, middle + 1, upper) 
        else: 
           return search(sequence, number, lower, middle) 

>>> seq = [34, 67, 8, 123, 4, 100, 95] 
>>> seq.sort() 
>>> seq 
>>> search(seq, 34) 
>>> search(seq, 100)
```
iterative(loop)
```
def binarySearch(alist, item):
	    first = 0
	    last = len(alist)-1
	    found = False
	
	    while first<=last and not found:
	        midpoint = (first + last)//2
	        if alist[midpoint] == item:
	            found = True
	        else:
	            if item < alist[midpoint]:
	                last = midpoint-1
	            else:
	                first = midpoint+1
	
	    return found
	
testlist = [0, 1, 2, 8, 13, 17, 19, 32, 42,]
print(binarySearch(testlist, 3))
print(binarySearch(testlist, 13))
```
# 遞迴函式的呼叫次數==>全域變數的應用
```
def fib(x):
"""Assumes x an int >= 0
	Returns Fibonacci of x"""
	
	global numFibCalls
	numFibCalls += 1
	
	if x == 0 or x == 1:
           return 1
	else:
          return fib(x-1) + fib(x-2)

def testFib(n):
	for i in range(n+1):
          global numFibCalls
          numFibCalls = 0
          print 'fib of', i, '=', fib(i)
          print 'fib called', numFibCalls, 'times.'
```
# Python內建函數==>Built-in Functions:

>* https://docs.python.org/2/library/functions.html
>* https://www.programiz.com/python-programming/methods/built-in

### dir():

dir(__builtins__)

```
import sys
print(system.builtin_module_names)
```

### help()
```
help('math')
help(id)
```
### hex(x):Convert an integer number to a lowercase hexadecimal string prefixed with “0x”
```
>>> hex(255)
>>> hex(-42)
```
## oct(x):Convert an integer number to an octal string prefixed with “0o”
```
>>> oct(8)
>>> oct(-56)
```

### bin(x):Convert an integer number to a binary string prefixed with “0b”
```
>>> bin(3)
>>> bin(-10)
```
## 數學類

### pow(x, y[, z])

>* pow(x, y)== x**y
>* pow(x, y, z) == (x**y)%z

```
# positive x, positive y (x**y)
print(pow(2, 4))

# negative x, positive y
print(pow(-2, 4))
print(pow(-2, 3))

# positive x, negative y (x**-y)
print(pow(2, -4))

# negative x, negative y
print(pow(-2, -4))
```
>* pow(x, y, z) == (x**y)%z
```
x = 7
y = 2
z = 5

print(pow(x, y, z))
```

### float()
```
>>> float('+1.43')
>>> float('   -123645\n')
>>> float('1e-002')
>>> float('+1E4')
>>> float('-Infinity')
```
### abs(num):絕對值或複數的大小
```
# integer
integer = -210
print('Absolute value of -210 is:', abs(integer))

#floating number
floating = -30.343
print('Absolute value of -30.343 is:', abs(floating))

# complex number
complex = (5 - 12j)
print('Magnitude of 5 - 12j is:', abs(complex))
```


Ascii code==> https://zh.wikipedia.org/wiki/ASCII
```
ord('a')
chr(97)
chr(ord('A')+1)
```

### len(s):Return the length (the number of items) of an object. 

>* The argument may be a sequence (such as a string, bytes, tuple, list, or range) or a collection (such as a dictionary, set, or frozen set).

### reversed(seq):seq的反轉

```
# string的反轉
seqString = 'Python'
print(list(reversed(seqString)))

# tuple的反轉
seqTuple = ('P', 'y', 't', 'h', 'o', 'n')
print(list(reversed(seqTuple)))

# list的反轉
seqList = [1, 2, 4, 3, 5]
print(list(reversed(seqList)))

# for range
seqRange = range(5, 9)
print(list(reversed(seqRange)))

```

# 模組化程式設計

>* 使用函式來模組化程式==> 模組(modules) 標準函式庫(Standard library)
>* 函式可用來減少多餘的程式碼，允許程式碼重複使用，還可以用來模組化程式碼，提升程式品質

步驟一:先將常用的功能寫成函式MyGCD.py
```
#!/usr/bin/python
# -*- coding: UTF-8 -*-
# Return the gcd of two integers 
def gcd(n1, n2):
    gcd = 1 # Initial gcd is 1
    k = 2   # Possible gcd

    while k <= n1 and k <= n2:
        if n1 % k == 0 and n2 % k == 0:
            gcd = k # Update gcd
        k += 1

    return gcd # Return gcd
```

步驟二:在主程式呼叫函式MyGCD.py
```
#!/usr/bin/python
# -*- coding: UTF-8 -*-

from MyGCD import gcd # 載入要用的模組

# 請使用者輸入兩個整數
n1 = eval(input("請輸入第一個整數: "))
n2 = eval(input("請輸入第二個整數 "))

# 輸出兩個整數的最大公因數
print("兩個整數的最大公因數", n1,
    "and", n2, "is", gcd(n1, n2))
```
##### 作業:完成模組化程式設計練習

>* 設計一個PYTHON程式(模組)命名為circle.py提供計算圓面積,周長,球體積與表面積的功能
>* 撰寫測試程式test.py使用上述功能

```
pi = 3.14159

def area(radius):
   return pi*(radius**2)

def circumference(radius):
   return 2*pi*radius

def sphereSurface(radius):
   return 4.0*area(radius)

def sphereVolume(radius):
   return (4.0/3.0)*pi*(radius**3)
```

```
import circle

print circle.pi
print circle.area(3)
print circle.circumference(3)
print circle.sphereSurface(3)
```


##### 補充
```
當我們導入一個模組時：import  xxx，
預設情況下python解析器會搜索目前的目錄、已安裝的內置模組和第三方模組，
搜索路徑存放在sys模組的path中
import sys
sys.path

添加自己程式(模組)到path讓python 解釋器找得到你自己寫的模組
sys.path.append('./home/ksu/haha')
```
