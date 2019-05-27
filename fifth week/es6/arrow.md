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
const sayIt = (name) => {
  return `Hello ${name}`;
}
```

Jika kita hanya punya satu parameter, kita bisa menghapus tanda kurungnya

```javascript
const sayIt = name => {
  return `Hello ${name}`;
}
```

Dan apabila kita tidak mempunyai parameter apapun, kita bisa tanda kurung saja


```javascript
const sayIt = () => {
  return 'Hello';
}
```

### Exclude Return

Dengan arrow function kita bisa menghilangkan return seperti ini

```javascript
const sayIt = (name) => `Hello ${name}`;
```
