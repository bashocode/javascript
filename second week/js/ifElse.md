# IF - ELSE in JavaScript

Sudah pernah belajar tentang ternary ? Kali ini kita akan belajar sesuatu yang mirip dengan ternary, jika ternary hanya ada dua kondisi maka di **IF - ELSE** kita bisa membuat banyak sekali kondisi bahkan membuat kondisi di dalam kondisi hwhw

```javascript
if (condition) {
  statement;
} else if (anotherCondition) {
  statement;
} else if (yetAnotherCondition) {
  statement;
  if (conditionInsideCondition) {
    statement;
  } else {
    statement;
  }
} else {
  statement;
}
```

**if** => digunakan pertama kali
**else if** => digunakan setelahnya
**else** => digunakan jika tidak ada kondisi lagi alias sisanya

Contohnya adalah kita ingin membuat klasifikasi dari SD sampai SMA, dimana ada 12 kelas

kelas 1 sampai 6 adalah SD
kelas 7 sampai 9 adalah SMP, dan
kelas 10 sampai 12 adalah SMA

Maka akan seperti ini

```javascript
const classOfStudent = 12;
let category;

if (classOfStudent >= 1 && classOfStudent <= 6) {
  category = "SD";
} else if (classOfStudent >= 7 && classOfStudent <= 9) {
  category = "SMP";
} else if (classOfStudent >= 10 && classOfStudent <= 12) {
  category = "SMA";
}

console.log(category);
```

Lihat, kita juga bisa menggunakan semua operators dalam if else, dan if else hanya akan mereturn true atau false, dan juga if else akan berhenti jika sudah mendapatkan apa yang mereka mau.

Jika kita hanya menggunakan if saja, maka kondisi tersebut akan di cek terus

```javascript
const classOfStudent = 12;
let category;

if (classOfStudent >= 1 && classOfStudent <= 6) {
  category = "SD";
}
if (classOfStudent >= 7 && classOfStudent <= 9) {
  category = "SMP";
}
if (classOfStudent >= 10 && classOfStudent <= 12) {
  category = "SMA";
}

console.log(category);
```

Dan berhati hatilah saat menggunakan && atau ||, pikirkan baik baik! Salah menggunakannya akan membuat outputnya juga berbeda.

Lalu, ada satu hal lagi yang perlu di ingat, kita tidak akan bisa menggunakan yang seperti ini

```javascript
const classOfStudent = 12;
let category;

if (classOfStudent >= 1 && <= 6) {
  category = "SD";
} else if (classOfStudent >= 7 && <= 9) {
  category = "SMP";
} else if (classOfStudent >= 10 && <= 12) {
  category = "SMA";
}

console.log(category);
```

Setelah tanda && atau || kita harus menulis ulang apa yang di kondisikan
