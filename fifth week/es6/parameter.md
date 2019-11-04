# Parameter

Kali ini kita akan belajar tentang parameter sebuah function

### Parameter Handling

Di dalam ES6 kita bisa langsung mendefinisikan value di dalam parameter sebuah function, contohnya bagaimana ?

Saat kita memberikan 3 parameter dalam function yang kita punya, misalkan parameter itu bernama x, y, dan z. Namun kita hanya melempar satu value nih, seperti dibawah.

```javascript
function f(x, y, z) {
  if (y === undefined) y = 7;
  if (z === undefined) z = 42;
  return x + y + z;
}

console.log(f(1)); // 50;
```

Artinya, parameter y dan z adalah undefined, alias ga ada. Lalu disitu kita bisa taro sebuah handler misalkan jika dia undefined maka kita ganti menjadi angka menggunakan if, inilah ES5.

Di dalam ES6 kita bisa membuat hal ini lebih simple.

```javascript
function f(x, y = 7, z = 42) {
  return x + y + z;
}

console.log(f(1)); // 50;
```

Bisa dilihat bahwa sangat mungkin untuk langsung menginiasikan value di dalam parameter sebuah function, dan cara ini fungsinya sama seperti memakai if. Lalu, bagaimana jika kita melempar 2 nilai ? silakan di coba sendiri ya...

### Rest Parameter

```javascript
function sum(a, b, ...z) {
  return (a + b) * z.length;
}

console.log(sum(1, 2, 'halo', true, 3)); // 9
```

Kenapa coba ? itu karena (1 + 2) _ 3 jadi 3 _ 3 sama dengan 9 dan alasan kenapa ada length disitu karena rest parameter akan membuat parameternya di bungkus kedalam array, ga percaya ? coba console.log z nya
