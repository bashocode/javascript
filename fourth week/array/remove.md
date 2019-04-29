# Removing an Element in Array

Setelah kita belajar cara menambahkan element di tutorial sebelumnya, tidak lengkap rasanya jika tidak mempelajari tentang kebalikannya.

Kita akan belajar cara menghapus element di dalam Array

### Beginning

Kita bisa menggunakan shift, kebalikan dari unshift

```javascript
const numbers = [1, 2, 3, 4, 5, 6, 7, 8];

numbers.shift();

console.log(numbers); // [ 2, 3, 4, 5, 6, 7, 8 ]
```

### End

Kebalikan dari push adalah pop, dulu saat saya belajar di bootcamp jokes ini bisa bikin ketawa loh hahaha (kami sering menyebut push and pop)

Nah, dari jokes yang tiap hari di perdengarkan akhirnya hapal **lol**

```javascript
const numbers = [1, 2, 3, 4, 5, 6, 7, 8];

numbers.pop();

console.log(numbers); // [ 1, 2, 3, 4, 5, 6, 7 ]
```

### Middle

Bisa menebak kira kira kita pakai apa ? Sebelumnya kita pernah passing 0 agar tidak ada yang di hapus bukan ?

Nah, disini kita akan menggunakan splice dan mempassing berapa yang akan kita hapus hehe

```javascript
const numbers = [1, 2, 3, 4, 5, 6, 7, 8];

numbers.splice(4);

console.log(numbers); // [ 1, 2, 3, 4 ]
```

Jika kita hanya mempassing startingIndexnya saja dan tidak mempassing berapa value yang di hapus maka dia akan menghapus semua valuenya

```javascript
const numbers = [1, 2, 3, 4, 5, 6, 7, 8];

numbers.splice(4, 2);

console.log(numbers); // [ 1, 2, 3, 4, 7, 8 ]
```

Dan jika kita mempassing jumlah yang di hapus maka dia akan menghapus dari startingIndex dan jumlahnya
