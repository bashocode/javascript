# Arithmetic Operator in JavaScript

Seperti operasi hitung di matematika, di JavaScript juga mempunyai operasi hitungnya sendiri.

```javascript
const firstNumber = 4;
const secondNumber = 2;

console.log(firstNumber + secondNumber); // Pertambahan
console.log(firstNumber - secondNumber); // Pengurangan
console.log(firstNumber * secondNumber); // Perkalian
console.log(firstNumber / secondNumber); // Pembagian
console.log(firstNumber % secondNumber); // Modulus
console.log(firstNumber ** secondNumber); // Perpangkatan
```

Dari pertambahan sampai pembagian pasti sudah tau kan, jadi tidak perlu di jelaskan ya, kita fokus di modulus dan perpangkatan

#### Modulus

Modulus adalah sisa bagi, misalnya begini 4 dibagi 2 sama dengan 2 bukan, nah sisa dari pembagian tersebut berapa ? 0 ya... jadi hasil dari 4 modulus 2 adalah 0.

Contoh lainnya adalah 5 modulus 2, kita breakdown dulu ya:

```
5 / 2 = 2
lalu 2 * 2 hasilnya 4 bukan ?
5 - 4 berapa ? 1
Nah, 5 modulus 2 hasilnya 1.
Itulah modulus.
```

Masih bingung ? coba contoh lain

```
9 / 2 = 4
4 * 2 = 8
9 - 8 = 1
Jadi, 9 % 2 hasilnya 1;
```

#### Perpangkatan

```
4 ** 2 hasilnya 16, kenapa ?

karena dari 4 * 4,

kalau 4 ** 1 maka 4
kalau 4 ** 3 maka 4 * 4 * 4
kalau 4 ** 4 maka 4 * 4 * 4 * 4
```

Selain yang di atas, kita juga punya nih yang namanya **increment (++)** dan **decrement (--)**

#### Increment

Increment itu pertambahan satu, contohnya

```javascript
let number = 10;

console.log(number++); // 10
```

Hasilnya akan berbeda dengan

```javascript
let number = 10;

console.log(++number); // 11
```

Kenapa ? karena komputer membaca dari _atas ke bawah dan dari kiri ke kanan_ maka penempatan sesuatu sangat berpengaruh

```
number++ akan menjalankan number terlebih dahulu yakni 10 baru kemudian di tambahkan.

Sedangkan ++number akan menjalankan pertambahan terlebih dahulu baru kemudian menampilkan si number
```

Untuk membuktikannya mari jalankan kode berikut

```javascript
let number = 10;

console.log(number++); // 10
console.log(number); // 11
```

#### Decrement

Prinsip decrement juga sama seperti increment, namun decrement mengurangi bukan menambah

```javascript
let number = 10;

console.log(number--); // 10
```

```javascript
let number = 10;

console.log(--number); // 9
```
