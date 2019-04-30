# How to Find Element in the Array

Untuk mencari suatu element di dalam array, kita harus memperhatikan tipe datanya, apakah tipe datanya berupa primitive atau reference.

Untuk mencari type data primitive, kita bisa menggunakan indexOf, lastIndexOf, atau includes.

```javascript
const alpha = ['a', 'b', 'c', 'd', 'e', 'a', 'b'];

const indexOfA = alpha.indexOf('a');
const lastIndexOfA = alpha.lastIndexOf('a');
const includesA = alpha.includes('a');

console.log(indexOfA); // 0
console.log(lastIndexOfA); // 5
console.log(includesA); // true
```

indexOf akan mereturn index yang mempunyai value yang sama dengan parameter pertama dan yang pertama kali di temukan, jika tidak ada value yang sama maka akan mereturn **-1**

```javascript
alpha.indexOf(firstParams, secondParams);
```

---

```
firstParams => value yang di cari
secondParams (optional) => index mulai pencarian
```

---

```javascript
const alpha = ['a', 'b', 'c', 'd', 'e', 'a', 'b'];

const indexOfA = alpha.indexOf('a', 3);

console.log(indexOfA); // 5
```

## Karena dia akan mencari dari index ke 3.

## Jika indexOf akan mereturn yang pertama kali di temukan, maka lastIndexOf akan mereturn yang terakhir kali di temukan.

Lalu bagaimana dengan includes ?

Includes akan mereturn true jika dia menemukan value yang di cari, dan false jika tidak.

Namun kita juga bisa menggunakan indexOf kok, contohnya

```javascript
const includeSomething = alpha.indexOf('a') !== -1;

console.log(includeSomething); // true
```

Karena -1 adalah tidak di temukan dan disitu ada tanda !==.
