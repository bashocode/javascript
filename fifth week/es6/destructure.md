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

### Object Matching

Bagaimana jika menggunakan object, ini lebih mantep lagi karena dengan destructure kita bisa mempersingkat kodingan kita, mau tau contohnya ?

```javascript
class Car {
  constructor(merk, model, price) {
    this.merk = merk;
    this.model = model;
    this.price = price;
  }

  merk() {
    return this.merk;
  }

  model() {
    return this.model;
  }

  price() {
    return this.price;
  }
}

const { merk, model, price } = new Car("BMW", "Sport", "120k");

console.log(merk); // BMW
console.log(model); // Sport
console.log(price); // 120k
```

Bandingkan dengan cara biasa

```javascript
class Car {
  constructor(merk, model, price) {
    this.merk = merk;
    this.model = model;
    this.price = price;
  }

  merk() {
    return this.merk;
  }

  model() {
    return this.model;
  }

  price() {
    return this.price;
  }
}

const car = new Car("BMW", "Sport", "120k");

console.log(car.merk); // BMW
console.log(car.model); // Sport
console.log(car.price); // 120k
```

Lebih singkat ga ? dikit sih, tapi syaratnya harus sama ya di dalam destructure dan dalam classnya, biasanya sering di gunakan saat kita memakai module module dari npm.
