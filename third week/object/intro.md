# Get More from Object

Sebelumnya kita sudah menyinggung tentang object dan kali ini kita akan mengenal lebih dekat dengan object. Di dalam object kita bisa memberikan tipe data apa saja yang kita mau,

*string
*number
*undefined
*null
*boolean
*array
*object
*bahkan function

Contoh penggunaan object sebenarnya bisa kita lihat di sekitar kita, misalnya sebuah ponsel, dia punya kamera, punya layar, punya sistem operasi, dll.

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

// dan kita bisa memanggilnya dengan dot notation

phone.merk(); // memanggil function dalam object
console.log(phone.screenType); // memanggil key dalam object
console.log(phone.camera[0]);
```
