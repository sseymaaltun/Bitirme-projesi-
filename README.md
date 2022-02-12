# Bitirme-projesi-
Python Temel Bitirme projesi 

*1- Bir listeyi düzleştiren (flatten) fonksiyon yazın. Elemanları birden çok katmanlı listelerden ([[3],2] gibi) oluşabileceği gibi, non-scalar verilerden de oluşabilir. Örnek olarak:*

*input: [[1,'a',['cat'],2],[[[3]],'dog'],4,5]*

*output: [1,'a','cat',2,3,'dog',4,5]*
```
list=[[1,'a',['cat'],2],[[[3]],'dog'],4,5] 
def flatten(list): 
    flat_list = [] 
    for i in list: 
        if type(i) == list: 
            flatten(i) 
        else: 
            flat_list.append(i) 
flatten(list) 
print(flat_list)
```
*2- Verilen listenin içindeki elemanları tersine döndüren bir fonksiyon yazın. Eğer listenin içindeki elemanlar da liste içeriyorsa onların elemanlarını da tersine döndürün. Örnek olarak:*

*input: [[1, 2], [3, 4], [5, 6, 7]]*

*output: [[[7, 6, 5], [4, 3], [2, 1]]*

```list=[[1, 2], [3, 4], [5, 6, 7]]
def reversed(y):
    new=[]
    for i in sort(list,reverse=True):
        new.append(sorted(i, reverse=True))
print(new)
```
