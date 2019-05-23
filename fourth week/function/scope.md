# Local and Global Scope

Scope adalah hal penting yang harus kita pahami, pertama kita akan membahas local scope.

```javascript
const word = 'hello';

console.log(word);
```

Jika kita menjalankan kode diatas, maka akan keluar _hello_ bukan ?

```javascript
{
  const word = 'hello';
}

console.log(word);
```

Namun jika kita memasukkan const word kedalam _code block_ maka akan terjadi error, itulah yang dinamakan scope.

Sekarang, coba ganti const menjadi let.

Lalu apa contoh dari code block ?

1. function

```javascript
function test() {
  const word = 'hello';
}

console.log(word);
```

1. if else

```javascript
if (true) {
  const word = 'hello';
}

console.log(word);
```

1. loop

```javascript
for (let i = 0; i < 5; i++) {
  const word = 'hello';
}

console.log(word);
```

Misalkan kita punya dua function

```javascript
function letter() {
  const word = 'hello';
}

function mail() {
  const word = 'world!';
}
```

Kode diatas tetap bisa dijalankan, meskipun ada dua _const word_ disana. Kenapa ? Karena mereka berbeda scope, ibaratnya ruangan A punya murid bernama 'Ali' dan ruangan B juga punya murid bernama 'Ali' dan mereka tetap berbeda bukan ?

---

Lalu, kita akan membahas tentang global

```javascript
const name = 'Brew';

function print() {
  console.log(name);
}
```

Kita tetap bisa mengakses name karena name ada di global scope, bahkan jika kita punya function lain, kita tetap bisa mengakses name tersebut.

```javascript
const name = 'Brew';

function print() {
  const name = 'Rashta';
  console.log(name);
}
```

Coba jalankan kode diatas, variable di dalam local scope lebih kuat dari global scope

Dan best practicenya kita jangan menggunakan global scope, karena bisa saja terjadi insiden mengganti valunya dan terjadilah error.
