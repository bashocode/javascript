# Do - While in JavaScript

Sebelumnya kita sudah belajar While, dan kali ini kita akan mengulik tentang Do-While.

Mari langsung lihat perbedannya saja ya

```javascript
let i = 1;

while (i < 4) {
  if (i % 2 === 0) console.log(i, "genap");
  i++;
}
```

Maka outputnya akan seperti ini

```
2 'genap'
```

Lalu bagaimana jika i bukan di bawah 4 melainkan di atas 4 (yakni condition)

```javascript
let i = 6;

while (i < 4) {
  if (i % 2 === 0) console.log(i, "genap");
  i++;
}
```

```
Maka tidak akan ada yang keluar karena 6 tidak kurang dari 4 bukan ? maka statement dalam while tidak akan di jalankan
```

Sedangkan jika kita menggunakan Do-While

```javascript
let i = 6;

do {
  if (i % 2 === 0) console.log(i, "genap");
  i++;
} while (i < 4);
```

Maka apa yang akan kita dapat ?

```
6 'genap'
```

Kenapa ? padahal 6 di atas 4 kan ? iya betul, tetapi condition berada di bawah dari statement, jadi statement akan di jalankan terlebih dahulu baru kemudian mengecek condition.

Perbedaan yang cukup mencolok bukan ? Do While loop sebenarnya jarang di gunakan, tetapi tidak apa apa untuk sekedar tau, agar nantinya jika melihat code seperti ini tidak bingung
