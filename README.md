# Merge-Sort-Project
Patika Dev Profile: https://app.patika.dev/ezgikarali4

## Project 2
[16,21,11,8,12,22] -> Merge Sort

1. Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
2. Big-O gösterimini yazınız.

### ANSWER 1. ###

[16,21,11,8,12,22] Bu diziyi sıralanmamız isteniyor.

    -Önce diziyi 2'ye bölücez: [16,21,11] [8,12,22]
    -Böldüğümüz sayıları tekrar 2'ye ayırıyoruz: [16,21] [11] [8] [12,22]
    -Tek eleman kalana kadar devam ettik: [16] [21] [11] [8] [12] [22]
    
      [16,21,11,8,12,22]
       /     /   \     \
    [16,21] [11] [8] [12,22]
     /   \    |    |   \   \ 
    [16] [21] [11] [8] [12] [22]
    -Bölme işlemimiz bitti. Şimdi ise sıralı hale getire getire ayırdığımız şekilde birleştiriyoruz.
    
    [16] [21] [11] [8] [12] [22]
      \    /   |    |    \  /
      [16,21] [11] [8] [12,22]
          \    /     \     /
        [11,16,21]  [8,12,22]
              \        /
          [8,11,12,16,21,22] 


### ANSWER 2. ###

Merge sort, önce diziyi eşit yarıya böler ve ardından bunları sıralı bir şekilde birleştirir.

Merge sort first divides the array into equal halves and then combines them in a sorted manner.

    n=6
    Best case    : O(n*logn)
    Average case : O(n*logn)
    Worst case   : O(n*logn) -> O(6*log6)
