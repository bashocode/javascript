# Arrow Function

ES6 memperkenalkan fat arrow **=>** untuk mendeklrasikan function.

Jika di ES5 kita biasa menggunakan

```javascript
var sayIt = function(name) {
  return 'Hello ' + name;
};
```

Dengan fat arrow kita bisa menulis seperti ini

```javascript
const sayIt = name => {
  return `Hello ${name}`;
};
```

Jika kita hanya punya satu parameter, kita bisa menghapus tanda kurungnya

```javascript
const sayIt = name => {
  return `Hello ${name}`;
};
```

Dan apabila kita tidak mempunyai parameter apapun, kita bisa tanda kurung saja

```javascript
const sayIt = () => {
  return 'Hello';
};
```

### Exclude Return

Dengan arrow function kita bisa menghilangkan return seperti ini

```javascript
const sayIt = name => `Hello ${name}`;
```

Kalau kita ingin me*return* object, kita bisa menggunakan

```javascript
const animal = ['cat', 'rabbit', 'dog'];
const pet = 'yes, they are pets';

const result = animal.map((ani, i) => ({ animal: ani, pet, rank: i + 1 }));

console.log(result);
// [ { animal: 'cat', pet: 'yes, they are pets', rank: 1 },
//   { animal: 'rabbit', pet: 'yes, they are pets', rank: 2 },
//   { animal: 'dog', pet: 'yes, they are pets', rank: 3 } ]
```

Menulis `pet` dan `pet: pet` itu sama saja.

### Arrow Function itu Anonymous

Jika kita ingin menambahkan nama, maka kita bisa memasukkan function kita di dalam sebuah variable

```javascript
const myFunction = name => `Hai ${name}`;

myFunction('bashocode');
```
