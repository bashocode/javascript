# Filtering an Array

Kita bisa memfilter array dengan menggunakan method filter, misal kita punya banyak angka di dalam array, dan kita hanya ingin mereturn angka yang positif.

```javascript
const numbers = [-2, -1, 0, 1, 2, 3];

const positive = numbers.filter(function(num) {
  return num >= 0;
});
```

Maka kita akan menghiraukan angka di bawah 0 bukan ? Jadi kita bisa mereturn angka yang lebih dari atau sama dengan 0.

Kita juga bisa menggunakan arrow function disini

```javascript
const numbers = [-2, -1, 0, 1, 2, 3];

const positive = numbers.filter(num => {
  return num >= 0;
});

// or

const anotherPositive = numbers.filter(num => num >= 0);
```

Karena hanya satu line code, maka kita bisa menghapus curly braces dan return.

Ada juga method lain yang namanya map, sebagai tugas. Coba untuk mencari tau tentang map.
