| rank | ▲ | ✰ | vote | url |
|:-:|:-:|:-:|:-:|:-:|
|  77 | 340 | 83 | 533 | [url](http://stackoverflow.com/questions/339007/nicest-way-to-pad-zeroes-to-string) |

***

## 给字符串填充0

有什么方法可以给字符串左边填充0,这样就可以有一个特定长度.

***

字符串:

```python
>>> n = '4'
>>> print n.zfill(3)
>>> '004'
```

对于数字:

```python
>>> n = 4
>>> print '%03d' % n
>>> 004
>>> print format(4, '03') # python >= 2.6
>>> 004
>>> print "{0:03d}".format(4)  # python >= 2.6
>>> 004
>>> print("{0:03d}".format(4))  # python 3
>>> 004
```

***

```python
>>> t = 'test'
>>> t.rjust(10, '0')
>>> '000000test'
```

