# Rest Operator

Rest Operator menggunakan titik tiga seperti spread operator, namun rest operator ada di parameter sebuah function

```javascript
function sum(...num) {
  console.log(num);
}

console.log(sum(1, 2, 3, 4, 5));
```

Jika kita jalankan kode di atas maka akan keluar array, dan seperti yang sudah kita pelajari sebelumnya, jika kita ingin menjumlahkan angka di atas (dan berupa array) maka kita akan menggunakan reduce

```javascript
function sum(...num) {
  return num.reduce((a, b) => a + b);
}

console.log(sum(1, 2, 3, 4, 5));
```

Lihat, kita menggunakan ...num hanya pada parameter function, dan untuk memanggilnya kita tidak perlu menggunakannya lagi
