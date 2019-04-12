# More Deep from String

Kali ini kita akan mencoba belajar lebih dalam tentang string, dengan menggunakan studi kasus tentunya.

Katakanlah kita ingin mencari index dari string yang beda sendiri, misalnya kita ingin mencari angka di rentetan huruf, untuk validasi nama yang di input oleh user, kita bisa coba menggunakan logika seperti ini

```javascript
// Carilah index dari string yang bernilai angka

// Di berikan sebuah string berupa w3basho, carilah index dan value dari string tersebut yang bernilai angka.

/*
Algoritma

- Kita harus melooping satu per satu dari input yang di berikan
- Lalu kita coba convert ke Number
- Jika berupa number, maka return indexnya
- Jika tidak, biarkan
*/

function validateName(string) {
  for (let i = 0; i < string.length; i++) {
    console.log(Number(string[i])); // kita coba console.log dulu
  }
}

const name = "w3basho";
console.log(validateName(name));
```

Dan inilah hasil dari console.log, maka bisa kita simpulkan bahwa yang berupa number ada di index ke 1;

```
NaN
3
NaN
NaN
NaN
NaN
NaN
```

Lalu jadikan seperti ini

```javascript
function validateName(string) {
  for (let i = 0; i < string.length; i++) {
    // console.log(Number(string[i])); // kita coba console.log dulu
    if (Number(string[i])) {
      return "ini index ke " + i + " dan berupa angka " + string[i];
    }
  }
}

const name = "w3basho";
console.log(validateName(name));
```

Maka hasilnya akan seperti ini

```
ini index ke 1 dan berupa angka 3
```

Kenapa ada **Number** disitu ? itu adalah function yang berguna untuk merubah string menjadi Integer, ada beberapa cara untuk merubah string menjadi integer, yakni **Number, parseInt, dan parseFloat**

```javascript
console.log(parseInt("42.1px")); // 42
console.log(Number("42.1px")); // NaN
console.log(parseFloat("42.1px")); // 42.1
```

Setelah membaca [ini](https://gomakethings.com/converting-strings-to-numbers-with-vanilla-javascript/) saya berkesimpulan bahwa, perbedaan mencolok dari ke 3 function di atas adalah

```
parseInt => hanya convert angka asli dan mengabaikan huruf juga angka dibelakang koma

Number => hanya menerima string berupa number, jika ada selain number seperti huruf maka akan mengembalikan NaN (Not a Number)

parseFloat => convert angka di belakang koma dan juga mengabaikan huruf
```
