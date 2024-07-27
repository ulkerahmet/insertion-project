# Örnek-1

### Insertion Sort Aşamaları

Başlangıç dizisi: [22, 27, 16, 2, 18, 6]

1. İlk eleman zaten sıralıdır. İkinci elemana geçilir.
   - [22, 27, 16, 2, 18, 6]
   
2. 27, 22'den büyük olduğu için yerine yerleştirilir.
   - [22, 27, 16, 2, 18, 6]
   
3. 16, 27'den küçük olduğu için 27'nin soluna yerleştirilir. 16, 22'den de küçük olduğu için 22'nin soluna yerleştirilir.
   - [16, 22, 27, 2, 18, 6]

4. 2, 27'den küçük olduğu için 27'nin soluna yerleştirilir. 2, 22'den küçük olduğu için 22'nin soluna yerleştirilir. 2, 16'dan küçük olduğu için 16'nın soluna yerleştirilir.
   - [2, 16, 22, 27, 18, 6]

5. 18, 27'den küçük olduğu için 27'nin soluna yerleştirilir. 18, 22'den küçük olduğu için 22'nin soluna yerleştirilir. 18, 16'dan büyük olduğu için yerine yerleştirilir.
   - [2, 16, 18, 22, 27, 6]

6. 6, 27'den küçük olduğu için 27'nin soluna yerleştirilir. 6, 22'den küçük olduğu için 22'nin soluna yerleştirilir. 6, 18'den küçük olduğu için 18'in soluna yerleştirilir. 6, 16'dan küçük olduğu için 16'nın soluna yerleştirilir. 6, 2'den büyük olduğu için yerine yerleştirilir.
   - [2, 6, 16, 18, 22, 27]

### Big-O Gösterimi

Insertion Sort'un en kötü durum zaman karmaşıklığı \( O(n^2) \)'dir. Ortalama durum zaman karmaşıklığı \( O(n^2) \) ve en iyi durum zaman karmaşıklığı \( O(n) \)'dir.

### 18 Sayısının Zaman Karmaşıklığı Durumu

18 sayısı sıralandıktan sonra dizinin ortasında bulunur. Bu nedenle, 18 sayısı **Average case** (ortalama durum) kapsamına girer.

# Örnek-2
### Selection Sort Aşamaları

Başlangıç dizisi: [7, 3, 5, 8, 2, 9, 4, 15, 6]

1. **Adım:** Dizideki en küçük eleman bulunur ve ilk eleman ile yer değiştirilir.
   - Mevcut dizi: [7, 3, 5, 8, 2, 9, 4, 15, 6]
   - En küçük eleman: 2
   - 2 ile 7 yer değiştirilir:
   - [2, 3, 5, 8, 7, 9, 4, 15, 6]

2. **Adım:** Kalan dizinin (ilk eleman hariç) en küçük elemanı bulunur ve ikinci eleman ile yer değiştirilir.
   - Mevcut dizi: [2, 3, 5, 8, 7, 9, 4, 15, 6]
   - En küçük eleman: 3 (zaten ikinci sırada, yer değiştirmeye gerek yok)
   - [2, 3, 5, 8, 7, 9, 4, 15, 6]

3. **Adım:** Kalan dizinin (ilk iki eleman hariç) en küçük elemanı bulunur ve üçüncü eleman ile yer değiştirilir.
   - Mevcut dizi: [2, 3, 5, 8, 7, 9, 4, 15, 6]
   - En küçük eleman: 4
   - 4 ile 5 yer değiştirilir:
   - [2, 3, 4, 8, 7, 9, 5, 15, 6]

4. **Adım:** Kalan dizinin (ilk üç eleman hariç) en küçük elemanı bulunur ve dördüncü eleman ile yer değiştirilir.
   - Mevcut dizi: [2, 3, 4, 8, 7, 9, 5, 15, 6]
   - En küçük eleman: 5
   - 5 ile 8 yer değiştirilir:
   - [2, 3, 4, 5, 7, 9, 8, 15, 6]

Bu dört adımdan sonra dizi: [2, 3, 4, 5, 7, 9, 8, 15, 6] şeklinde olacaktır.