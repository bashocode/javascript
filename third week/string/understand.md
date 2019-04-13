# Understanding String

Cara menggabungkan dua variable yang berupa string

```javascript
const name1 = "ikhda";
const name2 = "muhammad";
const name3 = "wildani";

const myName = name1 + " " + name2 + " " + name3;
```

terlalu ribet ? gunakan backticks

```javascript
const firstName = "ikhda";
const lastName = "wildani";
const fullName = `${firstName} ${lastName}`;

console.log(fullName); // ikhda wildani
```

Mengubah tipe data lain ke string

```javascript
const numbers = 23;
const stringuNumber = String(numbers);

console.log(stringNumber); // "23"

String(true); // "true"

// atau menggunakan

const secondStringNum = numbers.toString();
```

Kapan kita menggunakannya ? Lagi lagi tergantung kondisi, misalkan kita ingin mencari angka genap

```javascript
// carilah angka genap

function findEvenNumber(number) {
  // ubah dulu si number ke string, karena number ga bisa di looping
  const stringNum = String(number);

  // looping si stringNum, untuk mengambil satu per satu value
  for (let i = 0; i < stringNum.length; i++) {
    // cari angka yang genap, tentu tidak bisa kalau masih berupa string
    if (Number(stringNum[i]) % 2 === 0) {
      // return angkanya
      return stringNum[i];
    }
  }
}

console.log(findEvenNumber(123));
```

Lalu ada hal menarik nih, tau **ascii** ? coba [kesini](http://www.asciitable.com/)

Lihat bagian table angka HTML dan charnya,

```javascript
String.fromCharCode(104, 101, 108, 108, 111); //"hello"
```

Cocok ?

```
104 => h
101 => e
108 => l
108 => l
111 => o
```

Mantap bukan ? hwhw
