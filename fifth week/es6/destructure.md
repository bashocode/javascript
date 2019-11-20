# Destructuring Assignment

### Array Matching

Ini adalah fitur menarik yang dibawa oleh ES6, yakni mengambil value dari array ke sebuah variable baru

```javascript
const arr = [1, 2, 3];
let [a, , b] = arr;

console.log(a, b);

[a, b] = [b, a];

console.log(a, b);
```

index ke 1 arr yakni 2 di lewati dan value dari a dan b di balik, bisa di bayangkan kalau di coba menggunakan ES5 ?
