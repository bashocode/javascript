# Assignment Operator in JavaScript

Di tutorial sebelumnya, kita sudah belajar tentang increment dan decrement,

```javascript
let number = 10;

number++;
console.log(number); // 11
```

sebenarnya, sama dengan ini

```javascript
let number = 10;

number = number + 1;
console.log(number); // 11
```

Tapi jika kita ingin menambahkan lebih dari satu, maka operator increment tidak akan bekerja, itulah sebabnya kita menggunakan Assignment Operator

```javascript
let number = 10;

number = number + 5;
console.log(number); // 15
```

Namun, ada cara penulisan yang lebih simple

```javascript
let number = 10;

number += 5;
console.log(number); // 15
```

kita menggunakan **+=**, cara ini juga bisa di gunakan untuk operator lain

```javascript
let number = 10;

number += 1;
number -= 1;
number *= 2;
number /= 2;
```
