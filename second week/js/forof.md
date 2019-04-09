# For-of in JavaScript

Sebelumnya kita sudah mencoba looping array menggunakan for-in, namun ada cara baru yang worth untuk di gunakan, yakni for-of.

Ini adalah for-in

```javascript
const numbers = [1, 2, 3];

for (let index in numbers) {
  console.log(numbers[index]);
}
```

hasilnya

```
1
2
3
```

dan ini adalah for-of

```javascript
const numbers = [1, 2, 3];

for (let number of numbers) {
  console.log(number);
}
```

Bagaimana ? Lebih simple bukan.

Karena for-of akan mengambil nilai setiap index dari array, kalau for-in mengambil index dari array bukan nilai setiap indexnya.
