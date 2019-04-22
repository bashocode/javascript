# Factory Functions

Kenapa function ? Bukankah yang akan kita bahas adalah object ?

Benar, kita akan membahas tentang object, tetapi kita juga akan menyinggung sedikit tentang functions, di tutorial sebelumnya kita sudah membuat variable yang berisi object bukan

```javascript
const phone = {
  screenType: "Amoled",
  screenSize: 5.5,
  camera: [
    {
      front: 24
    },
    {
      back: [20, 12, 48]
    }
  ],
  isAndroid: true,
  price: 999,
  merk: function() {
    console.log("Siosung");
  }
};
```

Di atas, hanya ada sebuah object, lalu bagaima jika kita ingin membuat object lain yang sama persis ? misal untuk ponsel lain ? apa kita akan copy-paste ? hmm, kalau cuma 2 atau 3 sih tidak masalah, kalau ribuan ? gak pegel tuh tangan ?

Maka dari itu kita akan menggunakan factory functions, factory dalam bahasa indonesia adalah pabrik, dan di sini bisa kita asumsikan bahwa kita sedang membuat pabrik object haha

Kita akan membuat sebuah function bernama createPhone lalu di dalamnya kita akan membuat sebuah object seperti ini,

```javascript
function createPhone() {
  const phone = {
    screenType: "Amoled",
    screenSize: 5.5,
    camera: [
      {
        front: 24
      },
      {
        back: [20, 12, 48]
      }
    ],
    isAndroid: true,
    price: 999,
    merk: function() {
      console.log("Siosung");
    }
  };
  return phone;
}
```

Namun, kita tidak perlu mendeklarasikan constant dan hanya perlu return saja jadi bisa di buat seperti ini

```javascript
function createPhone() {
  return {
    screenType: "Amoled",
    screenSize: 5.5,
    camera: [
      {
        front: 24
      },
      {
        back: [20, 12, 48]
      }
    ],
    isAndroid: true,
    price: 999,
    merk: function() {
      console.log("Siosung");
    }
  };
}
```

Setiap kali kita memanggil createPhone maka akan muncul yang namanya object baru, tapi di function kita, kita me hardcode valuenya, maka kita coba untuk memberikan parameter saja ya,

Agar tidak bingung, kita bisa menghapus beberapa key/property

```javascript
function createPhone(price, brand) {
  return {
    price: price,
    merk: function() {
      console.log(brand);
    }
  };
}

createPhone(999, "Grape");
createPhone(888, "Siosung");
createPhone(777, "Ovvo");
```

Jika parameter dan key sama, kita bisa menulis sekali saja seperti ini

```javascript
function createPhone(price, brand) {
  return {
    price,
    merk: function() {
      console.log(brand);
    }
  };
}

createPhone(999, "Grape");
createPhone(888, "Siosung");
createPhone(777, "Ovvo");
```
