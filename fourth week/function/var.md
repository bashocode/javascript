# Why we should avoid var ?

Kita pasti sudah tahu bahwa di JavaScript ada 3 variable bukan ? yakni **var, let, dan const**

Lalu kenapa kita tidak pernah menggunakan var sama sekali ? Sebelumnya sudah belajar tentang scope bukan, dan var tidak mengenal apa itu scope.

Jalankan kedua kode di bawah ini dan bandingkan perbedaannya

```javascript
function nice() {
  if (true) {
    let name = 'bashocode';
  }

  console.log(name);
}
```

---

```javascript
function nice() {
  if (true) {
    var name = 'bashocode';
  }

  console.log(name);
}
```

Jika menggunakan let, maka dia akan error dan jika menggunakan var maka tetap akan keluar, nah disini-lah masalahnya

```
var => function scope
const/let => block scope
```

var bisa kita akses dimana saja selama di dalam sebuah function, dan itu menjadi masalah selama ini sampai akhirnya ES6 (EcmaScript 2015) datang dan membawa const dan juga let yang memperbaiki hal ini.
