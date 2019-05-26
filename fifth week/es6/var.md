# Var, Let, and Const

Sebelumnya kita sudah sering mencampur tentang pembahasan JavaScript dan ES6, namun di modul kali ini kita akan mengulas kembali tentang Variable di JavaScript yakni var, let dan const.

Mari kita lihat perbedaannya

### Var

**var** adalah _function scoped_ , artinya adalah dia akan bisa di akses dimanapun selama masih di dalam sebuha function.

contohnya var di dalam _for_ loop tetap bisa di akses meskipun di luar for loop tersebut

```javascript
for (var i = 0; i < 5; i++) {
  var message = 'You can call me outside of the loop';
}

console.log(message);
```

Namun jika kita panggil di luar function, maka akan error

```javascript
function greetings() {
  var message = 'You can call me outside of the loop';
}

greetings();
console.log(message);
```

Inilah kenapa var di namakan function scoped, jadi di contoh pertama dia bisa di akses meskipun di luar for, karena for bukanlah function melainkan block. Berbeda dengan contoh kedua dimana dia akan error karena mencoba di akses di luar function.

### Let

**let** dan juga (**const**) adalah _block scoped_, yakni dia hanya bisa di akses di dalam sebuah block dan sub-block dimana dia di deklarasikan.

```javascript
let x = 'global scoped';

if (x === 'global') {
  let x = 'block-scoped';

  console.log(x); // block-scoped
}

console.log(x); // global scoped
```

Bandingkan dengan var

```javascript
var x = 'global';

if (x === 'global') {
  var x = 'block-scoped';

  console.log(x); // block-scoped
}

console.log(x); // block-scoped
```

Seperti yang kita lihat, jika kita me-reassign let dengan value baru di dalam block-scoped, dia tidak akan merubah value di global scoped. Tetapi jika menggunakan var maka dia akan mengubah global scope variable yang kita punya.

### Const

Sama seperti let, **const** adalah _block scoped_. Tapi, const berbeda dengan let, sesuai dengan namanya yakni constant, **const tidak bisa di re-assignment atau re-declared**.

1. re-assign

```javascript
const constant = 'I am constant';
constant = "I can't be reassigned";
```

1. re-declare

```javascript
const constant = 'I am constant';
const constant = "I can't be reassigned";
```

**important**
Tetapi bukan berati dia immutable.

##### Example

```javascript
const bootcamp = {
  name: 'Basho Code',
  founder: 'Ikhda Muhammad Wildani'
};

bootcamp.name = 'bashocode';
```

Pada kasus diatas kita tidak akan mendapati error, karena yang kita re-assign bukan variablenya melainkan property-nya.

##### Important

Jika kita menggunakan _var_ maka sama saja seperti kita mendeklarasikan di awal (paling atas)

```javascript
console.log(x);
var x = 'I am a variable'; // undefined

console.log(y);
let y = 'I am a let'; // ReferenceError: can't access lexical declaration `y' before initialization
```

_var_ bisa di akses **sebelum** dia di definisikan, tapi tidak bisa di akses valuenya.
_let/const_ **tidak bisa** di akses sebelum dia di definisikan.

##### When to use var, let or const ?

Tidak ada aturan pasti mengenai ini. Tetapi saya menyarankan untuk tidak lagi menggunakan var,kenapa ?

Coba buat sebuah file **index.html** dan **index.js** dalam satu folder

_index.html_

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <title>Document</title>
  </head>
  <body>
    <script src="/index.js"></script>
  </body>
</html>
```

_index.js_

```javascript
var js = 'javascript';

console.log(js);
```

1. Lalu buka file index.html di browser
1. Klik kanan dan pilih _inspect element_
1. Cari tab _console_
1. Dan coba ketik _window._ dan cari js (nama dari variable yang kita buat)

_var_ akan membuat window baru disana dan itu tidak seharusnya kita lakukan, bagaimana jika kita merubah sesuatu yang secara _default_ ada di dalam window ?

Maka dari itu banyak yang menyarankan untuk melupakan var, karena memang lebih rentan ada bug di dalam aplikasi kita jika menggunakannya.

Ada juga opini lain seperti

Opini pertama dari [Mathias Bynes:](https://mathiasbynens.be/notes/es6-const)

- gunakan `const` secara default.
- gunakan `let` hanya jika kita ingin merubah nilainya suatu saat.
- `var` jangan pernah digunakan di ES6.

Opini kedua datang dari [Kyle Simpson:](blog.getify.com/constantly-confusing-const/)

- gunakan `var` untuk top-level variables yang akan di share ke banyak scope.
- gunakan `let` untuk local variable di dalam scope.
- refactor `let` ke `const` hanya jika sudah ada valuenya dan yakin kita tidak akan menggantinya lain waktu.
