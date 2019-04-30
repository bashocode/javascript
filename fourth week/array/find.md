# How to Find Element in the Array

Untuk mencari suatu element di dalam array, kita harus memperhatikan tipe datanya, apakah tipe datanya berupa primitive atau reference.

### Primitive

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

Karena dia akan mencari dari index ke 3.

Jika indexOf akan mereturn yang pertama kali di temukan, maka lastIndexOf akan mereturn yang terakhir kali di temukan.

Lalu bagaimana dengan includes ?

Includes akan mereturn true jika dia menemukan value yang di cari, dan false jika tidak.

Namun kita juga bisa menggunakan indexOf kok, contohnya

```javascript
const includeSomething = alpha.indexOf('a') !== -1;

console.log(includeSomething); // true
```

Karena -1 adalah tidak di temukan dan disitu ada tanda !==.

### Reference

Kita tidak bisa menggunakan cara dari primitive data types untuk mencari element di reference data types.

Jadi kita akan menggunakan method berupa find dan findIndex.

```
find => mereturn value jika di temukan, dan undefined jika tidak ada

findIndex => mereturn index value jika di temukan dan -1 jika tidak (mirip indexOf)
```

Lalu bagaiman strukturnya.

```javascript
blabla.find(function(callback) {
  return callback;
});

blabla.findIndex(function(callback) {
  return callback;
});
```

Jadi, di dalam function find atau findIndex akan ada callback function.

Apa itu callback function ? callback function adalah function yang menjadi parameter sebuah function.

Gimana ? bingung ? Kalau begitu coba cari apa itu callback hell.

Back in to topic, so Kali ini kita akan mencoba implementasikan pada array yang mempunyai object di dalamnya aka array of object.

```javascript
const cars = [
  { id: 1, name: 'Ferrari' },
  { id: 2, name: 'Lamborghini' },
  { id: 3, name: 'Porsche' },
  { id: 4, name: 'Bugatti' }
];

const car = cars.find(function(car) {
  return car.name === 'Ferrari';
});

console.log(car);

const carIndex = cars.findIndex(function(car) {
  return car.name === 'Ferrari';
});

console.log(carIndex);
```

Dan, di ES6 ada yang namanya arrow function, bedanya ?

```javascript
// function
function(car) {
    return car;
}

// arrow function
car => {
    return car;
}

// jika di dalam {} hanya ada satu statement, kita bisa menghapus tanda {} dan juga return
car => car;

// jika tidak ada parameter, kita bisa menggunakan tanda kurung saja ()
() => {
    return;
};
```

Contoh penggunaannya, kita memberikan sebuah variable dan nantinya untuk memanggil si function, kita bisa menggunakan nama variable tersebut.

```javascript
const name = () => {
  return 'bashocode';
};

const display = name();
console.log(display);
```

Mari kita rubah code di atas menjadi arrow function

```javascript
const cars = [
  { id: 1, name: 'Ferrari' },
  { id: 2, name: 'Lamborghini' },
  { id: 3, name: 'Porsche' },
  { id: 4, name: 'Bugatti' }
];

const car = cars.find(car => {
  return car.name === 'Ferrari';
});

console.log(car);

const carIndex = cars.findIndex(car => car.name === 'Ferrari');

console.log(carIndex);
```
