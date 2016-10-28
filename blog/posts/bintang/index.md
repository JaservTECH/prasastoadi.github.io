<!-- 
.. title: Bintang
.. slug: bintang
.. date: 2016-10-28 21:43:14 UTC+07:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text
-->

Cara membuat bintang.

```python
#***********
# ********* 
#  *******  
#   *****   
#    ***    
#     *     
#    ***    
#   *****   
#  *******  
# ********* 
#***********

loop = 10+1
mid = loop//2
for line in range(loop):
    for star in range(loop):
        if (star >= mid-abs(mid-line)) and (star <= mid+abs(mid-line)):
            print('*', end='')
        else:
            print(' ', end='')
    print('')
```


```python
#     *     
#    ***    
#   *****   
#  *******  
# ********* 
#***********
# ********* 
#  *******  
#   *****   
#    ***    
#     *  

loop = 10+1
mid = loop//2
for line in range(loop):
    for star in range(loop):
        if star >= mid-abs(mid-abs(mid-line)) and star <= mid+abs(mid-abs(mid-line)):
            print('*', end='')
        else:
            print(' ', end='')
    print('')
```

