# Removing Elements in Array

Sekarang, kita akan mencoba untuk meremove element di dalam array.

Caranya adalah menggunakan length

```javascript
const arr = [0, 1, 2, 3];

arr.length = 0;

console.log(arr); // []
```

Atau menggunakan splice

```javascript
const arr = [0, 1, 2, 3];

arr.splice(0, arr.length);

console.log(arr);
```

Lagi lagi butuh length bukan ?

Nah, ada satu tips lagi untuk kita, jangan menggunakan reassign

```javascript
let arr = [0, 1, 2, 3];
let another = arr;

arr = [];

console.log(arr); // []
console.log(another); // [0, 1, 2, 3]
```

Karena dia hanya akan menghapus array original, dan array copied akan tetap mempunyai value yang sama. Cara re assign tidak di rekomendasikan.
