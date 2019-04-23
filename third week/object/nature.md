# Inside of Object

Object bersifat dinamis, yakni kita bisa mengubah isinya seperti menambah atau menghapusnya.

```javascript
const phone = {
  merk: "Yeskia"
};
```

Kita bisa menambah key di dalam constant phone

```javascript
const phone = {
  brand: "Yeskia"
};

// menambah property
phone.os = "Android";
// atau menambah method
phone.madeBy = function() {
  return "Somewhere";
};
```

Bukankah constant itu nilainya tetap ? tidak bisa di rubah ?

Benar, constant memang tidak bisa di rubah, tapi maksudnya disini adalah re-assign seperti ini

```javascript
const phone = {
  merk: "Yeskia"
};

phone = {};
```

Kode di atas jika dijalankan maka error, karena kita me assign ulang sebuah constant.

Namun, jika kita merubah isi di dalamnya tetap bisa, seperti contoh sebelumnya, bahkan kita juga bisa menghapusnya

```javascript
const phone = {
  brand: "Yeskia"
};

phone.os = "Android";
phone.madeBy = function() {
  return "Somewhere";
};

// dengan menggunakan delete

delete phone.os;
```
