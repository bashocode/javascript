# Scope

### Block Scope Variables

Variable yang ada di javascript ada scopenya sendiri sendiri, jika **var** adalah block scope function (nanti akan dibahas dibawah) maka **let** dan **const** adalah block scope variable.

Block scope di tandai dengan {}

```javascript
let a = 0;
const b = 0;

console.log(a);
console.log(b);
```

coba jalankan kode diatas, lalu lihat apa yang terjadi. Bagaimana dengan ini ?

```javascript
{
  let a = 0;
  const b = 0;
}

console.log(a);
console.log(b);
```

begitupun jika kita menggunakan block block scope seperti di dalam **for, if else, switch case**, kita tidak akan bisa mengakses **let/const** yang berada dalam block scope.

```javascript
const flag = true;

if (flag) {
  let c = 0;
}

console.log(c);
```

### Block Scope Functions

Sebelumnya sudah disinggung bahwa **var** bukanlah block scope variable namun block scope function, artinya var bisa di akses dimanapun selama dia tidak keluar dari function (jika ada function).

```javascript
const flag = true;

if (flag) {
  var c = 0;
}

console.log(c);
```

Namun jika di luar function, dia tidak bisa di akses

```javascript
function scope() {
  var d = 1;
}

scope();
console.log(d);
```
