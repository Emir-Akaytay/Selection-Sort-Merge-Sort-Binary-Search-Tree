# Selection Sort, Merge Sort, Binary Search Tree

 **Veri Yapıları ve Algoritmalar** Dersinin 3 projesi

---

## Proje 1

[22,27,16,2,18,6] -> Insertion Sort

Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

Big-O gösterimini yazınız.

Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız

[7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.

*Çözüm* :

---INSERTION SORT---

[22,27,16,2,18,6] [22,16,27,2,18,6] [16,22,27,2,18,6] [16,22,2,27,18,6] [16,2,22,27,18,6] [2,16,22,27,18,6] [2,16,22,18,27,6] [2,16,18,22,27,6] [2,16,18,22,6,27] [2,16,18,6,22,27] [2,16,6,18,22,27] [2,6,16,18,22,27]

18 **average case** kapsamına girer.

**Time complexity**’si :

Best Case : O(n)
Worst Case : O(n²)
Average Case : O(n²)

---SELECTION SORT---

[7,3,5,8,2,9,4,15,6] [2,7,3,5,8,9,4,15,6] [2,3,7,5,8,9,4,15,6] [2,3,4,5,7,8,9,15,6] [2,3,4,5,6,7,8,9,15]

---

## Proje 2

[16,21,11,8,12,22] -> Merge Sort

Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
Big-O gösterimini yazınız.

*Çözüm* :

[16,21,11,8,12,22]
[16,21,11]        [8,12,22]
[16,21] [11]      [8,12] [22]
[16] [21] [11]    [8] [12] [22]
[16,21] [11]       [8]  [12,22]
[11,16,21]   [8,12,22]
[8,11,12,16,21,22]

**Big O** Gösterimi : 0(nlogn)

---

## Proje 3

[7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin **Binary-Search-Tree** aşamalarını yazınız.

*Çözüm* :

```1
            [7]         Root 7'dir.
        [5]             5 < 7 olduğu için sola doğru yerleştirdik.
    [1]                 1 < 7 ardından 1 < 5 olduğu için 5'ten sonra sola doğru yerleştirdik.
```

```2
            [7] 
        [5]     [8]     8 > 7 olduğu için 7'nin sağına yerleştirdik.
    [1]
```

```3
            [7] 
        [5]     [8]    
    [1]
       [3]              3 < 7 ardından 3 < 5 ardından 3 > 1 olduğu için 1'den sonra sağa doğru yerleştirdik.
```

```4
            [7] 
        [5]     [8]    
    [1]   [6]          6 < 7 ardından 6 > 5 olduğundan dolayı 5'den sonra sağa doğru yerleştirdik.
       [3]
```

```5

            [7] 
        [5]     [8]    
    [1]   [6]
  [0] [3]               0 < 7 ardından 0 < 5 ardından 0 < 1 olduğundan dolayı 1'den sonra sola doğru yerleştirdik.
```

```6
            [7] 
        [5]     [8]    
    [1]   [6]      [9]  9 > 7 ardından 9 > 8 olduğu için 8'den sonra hemen sağa doğru yerleştirdik.
  [0] [3]
```

```7
            [7] 
        [5]     [8]    
    [1]   [6]      [9]
  [0] [3]
        [4]             4 < 7 ardından 4 < 5 ardından 4 > 1 ardından 4 > 3 olduğu için 3'ten sonra sağa yerleştirdik.
```

```8
            [7] 
        [5]     [8]    
    [1]   [6]      [9]
 [0]   [3]
     [2] [4]            2 < 7 ardından 2 < 5 ardından 2 > 1 ardından 2 < 3 olduğu için 3'ten sonra sola yerleştirdik.
```

---
