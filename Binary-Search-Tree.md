# Veri Yapıları ve Algoritmalar
## Binary Search Tree
### [7,5,1,8,3,6,0,9,4,2] dizisinin Binary-Search-Tree aşamalarını yazınız.
***
###### Binary Search Tree oluştururken Root'un sağ tarafından kendinden büyük elemanlar, sol tarafında ise küçük elemanlar bulunur.
- ``` root -> 2 ``` alalım. Sonrasında 2'nin yanındaki sayıları karşılaştırarak büyükse sağ tarafa küçükse sol tarafa atayarak sıralamaya devam edelim
- ``` 4 ``` , 2'den büyüktür, dolayısıyla 1. Düğüm satırı'nda 2'nin sağında olacaktır.

```

                  2          -> Root Satırı
                   \
                    \
                     4             -> 1. Düğüm Satırı

```
                       
- ```9```, 2 ve 4'den büyüktür, dolayısıyla 2. Düğüm Satırı'nda 4'ün sağ tarafında olacaktır. 

```

                  2          -> Root Satırı
                   \
                    \
                     4             -> 1. Düğüm Satırı
                      \
                       \
                        9          -> 2. Düğüm Satırı
```
- ```0```, 2'den küçüktür, dolayısıyla 1. Düğüm Satırı'nda 2'nin sol tarafında olacaktır. 
```

                  2          -> Root Satırı
                 / \
                /   \
               0     4             -> 1. Düğüm Satırı
                      \
                       \
                        9          -> 2. Düğüm Satırı
```
- ```6```, 2'den ve 4'den büyüktür ancak 9'dan küçüktür bu yüzden 3. Düğüm Satırı'nda 9'un sol tarafında olacaktır. 
```

                  2          -> Root Satırı
                 / \
                /   \
               0     4             -> 1. Düğüm Satırı
                      \
                       \
                        9          -> 2. Düğüm Satırı
                       /
                      /
                     6             -> 3. Düğüm Satırı 
```
- ```3```, 2'den büyüktür ancak 4'den küçüktür bu yüzden 2. Düğüm Satırı'nda 4'ün sol tarafında olacaktır. 
```

                  2          -> Root Satırı
                 / \
                /   \
               0     4             -> 1. Düğüm Satırı
                    / \
                   /   \
                  3     9          -> 2. Düğüm Satırı
                       /
                      /
                     6             -> 3. Düğüm Satırı 
```
- ```8```, 2'den ve 4'den büyüktür ancak 9'den küçük ve 6'dan büyüktür bu yüzden 4. Düğüm Satırı'nda 6'nın sağ tarafında olacaktır. 
```

                  2          -> Root Satırı
                 / \
                /   \
               0     4             -> 1. Düğüm Satırı
                    / \
                   /   \
                  3     9          -> 2. Düğüm Satırı
                       /
                      /
                     6             -> 3. Düğüm Satırı 
                      \
                       \
                        8          -> 4. Düğüm Satırı 
```
- ```1```, 2'den küçüktür 0'dan büyüktür ancak 3'den küçüktür bu yüzden 3. Düğüm Satırı'nda 3'ün sol tarafında olacaktır. 
```

                  2          -> Root Satırı
                 / \
                /   \
               0     4             -> 1. Düğüm Satırı
                \   / \
                 \ /   \
                  3     9          -> 2. Düğüm Satırı
                 / \    /
                /   \ /
               1     6             -> 3. Düğüm Satırı 
                      \
                       \
                        8          -> 4. Düğüm Satırı 
```
- ```5```, 2'den ve 4'den büyüktür ancak 9'dan ve 6'dan küçüktür bu yüzden 4. Düğüm Satırı'nda 6'nın sol tarafında olacaktır. 
```

                  2          -> Root Satırı
                 / \
                /   \
               0     4             -> 1. Düğüm Satırı
                \   / \
                 \ /   \
                  3     9          -> 2. Düğüm Satırı
                 / \   /
                /   \ /
               1     6             -> 3. Düğüm Satırı 
                    / \
                   /   \
                  5     8          -> 4. Düğüm Satırı 
```
- ```7```, 2'den ve 4'den büyüktür, 9'dan küçük 6'dan büyük ancak 8'den küçüktür bu yüzden 5. Düğüm Satırı'nda 8'in sol tarafında olacaktır. 
```

                  2          -> Root Satırı
                 / \
                /   \
               0     4             -> 1. Düğüm Satırı
                \   / \
                 \ /   \
                  3     9          -> 2. Düğüm Satırı
                 / \   /
                /   \ /
               1     6             -> 3. Düğüm Satırı 
                    / \
                   /   \
                  5     8          -> 4. Düğüm Satırı 
                       / 
                      / 
                     7             -> 5. Düğüm Satırı 
```
* * *
[Ozan Bayram GitHub Hesabım](https://github.com/ozanbayramm)  
[Patika.dev Hesabım](https://app.patika.dev/ozanbyrm)