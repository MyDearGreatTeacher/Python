

# FOR loop 

### 執行下列程式並說明其結果


http://www.runoob.com/python/python-exercise-example1.html
```
#!/usr/bin/python
# -*- coding: UTF-8 -*-
 
for i in range(1,6):
    for j in range(1,5):
        for k in range(1,7):
            if( i != k ) and (i != j) and (j != k):
                print i,j,k

```
### 下列程式輸入淨利潤為11111時請問輸出為何?
```
#!/usr/bin/python
# -*- coding: UTF-8 -*-
 
i = int(raw_input('淨利潤:'))
arr = [1000000,600000,400000,200000,100000,0]
rat = [0.01,0.015,0.03,0.05,0.075,0.1]
r = 0
for idx in range(0,6):
    if i>arr[idx]:
        r+=(i-arr[idx])*rat[idx]
        print (i-arr[idx])*rat[idx]
        i=arr[idx]
print r
```
