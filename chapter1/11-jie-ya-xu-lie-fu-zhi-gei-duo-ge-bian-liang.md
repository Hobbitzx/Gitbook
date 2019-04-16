## 1.1 解压序列赋值给多个变量
任何的序列或者是可迭代对象（如列表、元组、字符串、文件对象、迭代器和生成器等）都可以通过一个简单的赋值语句解压并赋值给多个变量。
**唯一前提**：变量数量=序列元素的数量
```python
>>> p = (4, 5)
>>> x, y = p
>>> x
4
>>> y
5
>>>
>>> data = [ 'ACME', 50, 91.1, (2012, 12, 21) ]
>>> name, shares, price, date = data
>>> name
'ACME'
>>> date
(2012, 12, 21)
>>> name, shares, price, (year, mon, day) = data
>>> name
'ACME'
>>> year
2012
>>> mon
12
>>> day
21
>>>
>>> s = 'Hello'
>>> a, b, c, d, e = s
>>> a
'H'
>>> b
'e'
>>> e
'o'
>>>
```