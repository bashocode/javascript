# Add an Element to the Array

Array adalah salah satu tipe data reference di dalam JavaScript, dan array sangat penting untuk di ketahui, maka kita akan memperdalam array di modul ini.

```javascript
const numbers = [5, 6];
```

Masih ingat dengan const ? constant tidak bisa kita re-assign seperti ini

```javascript
numbers = [1, 2];
```

Karena hasilnya akan error, tetapi tidak ada masalah jika kita ingin merubah isi di dalam array literal **[]**, sama seperti object.

Jadi, mari kita coba menambahkan value di dalam array tersebut,

### Beginning

Jika kita ingin menambahkan sesuatu di dalam array dan di awal alias beginning, kita bisa menggunakan unshift.

```javascript
const numbers = [5, 6];

numbers.unshift(1, 2);

console.log(numbers); // [1, 2, 5, 6]
```

### End

Lalu jika kita ingin menambah dari belakang ? Kita bisa menggunakan push.

```javascript
const numbers = [5, 6];

numbers.unshift(1, 2);

numbers.push(7, 8);

console.log(numbers); // [1, 2, 5, 6, 7, 8]
```

### Middle

Depan sudah belakang juga sudah, bagaimana dengan tengah ? well kita bisa menggunakan splice, namun ada beberapa parameter yang mesti kita perhatikan.

```javascript
splice(startingIndex, deletedCount, value);
```

```
startingIndex => index dari sebuah array yang akan kita rubah (ingat index di awali dari 0)

deletedCount => adalah berapa yang ingin kita hapus

value => adalah value yang akan kita tambahkan
```

```javascript
const numbers = [5, 6];

numbers.unshift(1, 2);

numbers.push(7, 8);

numbers.splice(2, 0, 3, 4);

console.log(numbers); // [1, 2, 3, 4, 5, 6, 7, 8]
```

Di kasus kita kali ini, kita ingin mengganti angka 5 menjadi 3,

```
[1, 2, 5, 6, 7, 8]

 0  1  2  3  4  5
```

Jadi kita mulai dari index ke 2 bukan ? Lalu kita ingin menghapus apapun disini, jadi kita passing angka 0, agar jumlah value yang di hapus adalah 0,

Lalu di parameter selanjutnya kita mempassing apa saja yang ingin kita tambahkan ke dalam array.
