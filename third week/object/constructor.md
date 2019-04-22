# Constructor Function

Di samping menggunakan factory function, kita juga bisa menggunakan constructor function untuk membuat object,

Namun, jika kita ingin membuat constructor function kita harus menggunakan pascal notation, berbeda dengan factory function yang menggunakan camel notation

```
pascal notation => OneTwoThreeFour
camel notation => oneTwoThreeFour
```

Perbedaannya di awal ya, kalau pascal huruf awalnya menggunakan huruf besar sedangkan camel huruf awalnya menggunakan huruf kecil

Lalu kita juga harus menggunakan this untuk membuat key/property

Baik mari kita langsung mencoba!

```javascript
function Phone(price, brand) {
  this.price = price,
  this.merk = function() {
    console.log(brand);
  };
}

const phone1 = new Phone(999, "Grape");
const phone2 = new Phone(888, "Siosung");
const phone3 = new Phone(777, "Ovvo");
```

Lihat, kita harus menggunakan **=** dan untuk memanggil functionnya, kita menggunakan **new**
