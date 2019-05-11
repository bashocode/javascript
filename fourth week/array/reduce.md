# Reduce an Array

Katakanlah kita ingin menjumlahkan semua bilangan di dalam sebuah array, dan kita bisa menggunakan sebuah for of loop seperti ini

```javascript
const numbers = [1, 2, 3, 4, 5];

let sum = 0;

for (let num of numbers) {
  sum += num;
}

console.log(sum);
```

Namun ada cara yang lebih elegan lagi yang bisa kita lakukan, yakni menggunakan reduce.

```javascript
const numbers = [1, 2, 3, 4, 5];

const total = numbers.reduce((accumulator, value) => {
  return accumulator + value;
}, 0);
```

reduce menerima dua argumen,

argumen pertama yakni callback function yang mempunyai dua parameter
    -accumulator yang fungsinya sama seperti variable sum (sebagai penampung hasil),
    -dan value yang fungsinya mengambil setiap index di dalam sebuah array

argumen kedua, nilai 0 yakni initial valuenya, dan kenapa 0 ? karena sama dengan apa yang kita inisialisasikan di variable sum
