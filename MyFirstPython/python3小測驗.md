
#

```
print("Word counter")
sentence = input("Please enter a sentence to count the number of words. Press ENTER to end the sentence:")
print("In this sentence, the number of words is:")
print(len(sentence.split(' ')))
```
https://github.com/PacktPublishing/Begin-Python-Programming-in-7-Days-Video-/blob/master/day-4.py

# FOR loop 

### 執行下列程式並說明其結果


# while loop 

### 執行下列程式並說明其結果
```
n1 = 0
n2 = 1
count = 0

while count < 20:
   print(n1)
   n3 = n1 + n2
   n1 = n2
   n2 = n3
   count += 1
```

https://github.com/PacktPublishing/Begin-Python-Programming-in-7-Days-Video-/blob/master/day-2.py
   
# Function

### 
```
def add(x, y):
   return x + y

def subtract(x, y):
   return x - y

def multiply(x, y):
   return x * y

def divide(x, y):
   return x / y

print("Python Calculator:")
print("1. Add")
print("2. Subtract")
print("3. Multiply")
print("4. Divide")

choice = input("What are we calculating today? (1, 2, 3, or 4):")
num1 = int(input("Enter first number: "))
num2 = int(input("Enter second number: "))

if choice == '1':
   print(num1,"+",num2,"=", add(num1,num2))
elif choice == '2':
   print(num1,"-",num2,"=", subtract(num1,num2))
elif choice == '3':
   print(num1,"*",num2,"=", multiply(num1,num2))
elif choice == '4':
   print(num1,"/",num2,"=", divide(num1,num2))
else:
   print("Invalid input")
```

https://github.com/PacktPublishing/Begin-Python-Programming-in-7-Days-Video-/blob/master/day-3.py


