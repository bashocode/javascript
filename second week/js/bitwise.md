# Bitwise Operator

Bitwise mempunyai dua operator yakni **|** dan **&**, dan sebenarnya jarang digunakan tetapi tidak ada salahnya untuk tau tentang hal ini.

Di komputer bilangan yang di pakai adalah binary sedangkan kita sebenarnya menggunakan decimal

```
Decimal to Binary

0 => 00000000
1 => 00000001
2 => 00000010
3 => 00000011
4 => 00000100
5 => 00000101
6 => 00000110
7 => 00000111
dst....
```

Nah disini kita akan mencoba menggunakan operator bitwise yang memang menggunakan binary, jadi decimal akan di convert ke dalam binary terlebih dahulu

```javascript
console.log(1 | 2); // 3
```

Kita sudah tau bukan bahwa operator OR akan mengembalikan nilai true jika salah satunya adalah true, sedangkan angka 1 adalah true dan angka 0 adalah false. Maka bisa di breakdown seperti ini

```
angka 1 | 2 hasilnya 3 maka

00000001
00000010
--------+
00000011 => 3
```

1 | 0 hasilnya akan 1, jadi hasilnya akan berupa 00000011 yang jika di decimalkan maka menjadi angka 3

Sedangkan operator AND akan mengembalikan true jika keduanya bernilai true

```javascript
console.log(1 & 2); // 0
```

```
angka 1 & 2 hasilnya 0 maka

00000001
00000010
--------+
00000000 => 0
```

1 & 0 hasilnya akan 0, jadi hasilnya akan berupa 00000000 yang jika di decimalkan maka menjadi angka 0
