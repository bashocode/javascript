# Cloning an Object

Kali ini kita akan mencoba untuk mempelajari **kagebunshin no jutsu** dan akan kita terapkan di object

```
kagebunshin no jutsu => jurus bayangan (clone)
```

Haha, sudah berhenti bercandanya, mari langsung saja

```javascript
const phone = {
  brand: "Xiaosung",
  price: 199
};
```

Untuk meng-clone object di atas, kita bisa menggunakan for in loop

```javascript
const anotherPhone = {};

for (let key in phone) {
  anotherPhone[key] = phone[key];
}

console.log(anotherPhone);
```

Breakdown

```
- Kita iterate key di dalam object phone,
- Lalu kita membuat anotherPhone mempunyai key yang sama dengan phone
- Dan kita memberi value pada anotherPhone persis seperti value pada phone
```

Namun, di modern javascript kita bisa melakukan hal ini dengan lebih mudah

```javascript
const phone = {
  brand: "Xiaosung",
  price: 199
};

const anotherPhone = Object.assign({}, phone);

console.log(anotherPhone);
```

Kita bisa menggunakan **Object.assign** yang menerima dua parameter, parameter pertama adalah object (bisa kosong atau sudah ada propertynya), dan yang kedua adalah object mana yang akan kita clone (bisa lebih dari satu object).

Contohnya kita bisa coba dengan object yang sudah ada propertynya sebagai parameter pertama

```javascript
const phone = {
  brand: "Xiaosung",
  price: 199
};

const anotherPhone = Object.assign({ os: "android" }, phone);

console.log(anotherPhone);
```

Tapi ada cara yang lebih keren lagi, kita bisa gunakan spread operator

```javascript
const phone = {
  brand: "Xiaosung",
  price: 199
};

const anotherPhone = { ...phone };

console.log(anotherPhone);
```

Spread operator adalah **...** (titik tiga), dia akan mengambil semua property dari phone, dan kita membungkusnya di dalam object literal **{}** (kurung kurawal).
