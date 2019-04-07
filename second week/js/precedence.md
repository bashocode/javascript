# Precedence

Seperti matematika, di JavaScript juga ada operator yang lebih dulu di kerjakan seperti perkalian dan pembagian

```javascript
const number = 5 + 6 * 2;

console.log(number); // 17
```

Maka operasi hitungnya akan mendahulukan perkalian, jika kita ingin menghitung pertambahan terlebih dahulu maka bisa gunakan **()**

```javascript
const number = (5 + 6) * 2;

console.log(number); // 22
```
