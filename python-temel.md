# Python Temel

1. 1- Bir listeyi düzleştiren (flatten) fonksiyon yazın. Elemanları birden çok katmanlı listelerden ([[3],2] gibi) oluşabileceği gibi, non-scalar verilerden de oluşabilir. Örnek olarak:

```python
inp = [[1,'a',['cat'],2],[[[3]],'dog'],4,5]
lis = []
def d(x):
    for i in range(len(x)):
        if type(x[i]) == list:
            d(x[i])
        else:
            lis.append(x[i])
    return lis
d(inp)
```

2- Verilen listenin içindeki elemanları tersine döndüren bir fonksiyon yazın. Eğer listenin içindeki elemanlar da liste içeriyorsa onların elemanlarını da tersine döndürün. Örnek olarak:

```python
inp = [[1, 2], [3, 4], [5, 6, 7]]

def rev(arr):
    rev = []
    for ar in arr:
        rev.append(ar[::-1])
    return print(rev[::-1])

rev(inp)
```
