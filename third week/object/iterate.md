# Iterate an Object

Kali ini kita akan mencoba untuk me-loop-ing object, mari kita bermain main sebentar.

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

for (let key in phone) {
  console.log(phone[key]);
}
```

Kita bisa memakai for-in loop untuk iterate object, dan jika kita menggunakan for-of maka tidak akan bisa.

```
akan muncul error
phone is not iterable
```

Lalu, bagaimana jika kita ngotot ingin memakai for-of loop ? karena kita sudah jatuh cinta (misalnya)

Kita bisa menggunakan ini

```javascript
for (let key of Object.keys(phone)) {
  console.log(phone[key]);
}
```

Atau ini

```javascript
for (let key of Object.entries(phone)) {
  console.log(key);
}
```

Silakan di coba untuk tau hasilnya hahahaha
