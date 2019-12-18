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
}

const car = new Car("BMW", "Sport", "120k");

console.log(car.merk); // BMW
console.log(car.model); // Sport
console.log(car.price); // 120k
```

Lebih singkat ga ? dikit sih, tapi syaratnya harus sama ya di dalam destructure dan dalam classnya, biasanya sering di gunakan saat kita memakai module module dari npm.

Ada juga yang lebih dalam lagi, misalkan object di dalam object, caranya gimana ? mari kita cari tahu

```javascript
class Car {
  constructor(merk, model, price) {
    this.merk = {
      nameOfMerk: merk
    };
    this.model = model;
    this.price = price;
  }
}

const {
  merk: { nameOfMerk: sayMerk },
  model,
  price
} = new Car("BMW", "Sport", "120k");

console.log(sayMerk); // BMW
console.log(model); // Sport
console.log(price); // 120k
```

Seperti contoh kode diatas, kenapa kita bisa destructure di dalam destructure ? oh ya, ini agak mengerikan kalau di pikirkan, mari di breakdown

Pokonya _merk_ yang di destructure namanya harus sama dengan yang constructor didalam class, dan didalam constructor ternyata adalah sebuah object, dan kita ingin mengambilnya, maka kita harus menyamakan key object _nameOfMerk_ dan di ambil valuenya, terserah mau di namai apa, disini saya menamainya _sayMerk_

Jadi pertama di ambil lah _merk_ => ternyata _merk_ ada di dalam constructor dan didalamnya adalah object. Kemudian, kita destructure lagi dan ambil key objectnya, dan masukkan valuenya kedalam penampung yang bernama _sayMerk_. Nah itulah kenapa kita akses _sayMerk_ keluarnya BMW. Simple kan ?

### Default Values

ada fitur lagi yang mantap banget di ES6, ga perlu lagi kita musingin untuk ngasi default value memakai _ternary_,

```javascript
const obj = { name: "Bashocode" };
const arr = ["javascript"];

const { name, field = "programming" } = obj;
const [a, b = "python"] = arr;

console.log(name);
console.log(field);
console.log(a);
console.log(b);
```

arti **field = 'programming'** adalah jika dia valuenya adalah undefined maka langsung di ganti dengan 'programming', kalau di ES5 kita biasa menggunakan ternary seperti ini

```javascript
var obj = { name: "Bashocode" };
var arr = ["javascript"];

var name = obj.name;
var field = obj.field === undefined ? "programming" : obj.field;
var a = arr[0];
var b = arr[1] === undefined ? "python" : arr[1];

console.log(name);
console.log(field);
console.log(a);
console.log(b);
```
