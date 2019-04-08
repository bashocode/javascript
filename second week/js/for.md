# FOR in JavaScript

For digunakan jika kita ingin melakukan sesuatu berulang ulang seperti

```javascript
console.log("Hello World!");
console.log("Hello World!");
console.log("Hello World!");
console.log("Hello World!");
console.log("Hello World!");
```

Daripada kita menulis kode semacam itu lebih baik kita gunakan for loop

```javascript
for (let i = 0; i < 5; i++) {
  console.log("Hello World!");
}
```

Mari kita lihat struktur dari for loop

```javascript
for (initialExpression; condition; incrementExpression) {
    statementOne;
    statementTwo;
    etc.........;
}
```

Pertama kita punya **for** di ikuti tanda kurung **()** dan tanda kurung kurawal **{}**

```
di dalam tanda kurung (), kita punya:
    intitalExpression => yakni awal mula kita mulai
    condition => kapan kita berhenti
    incrementExpression => pertambahan atau pengurangan
lalu di dalam kurung kurawal {}, kita bisa menulis banyak hal,
bahkan kita bisa menambahkan for lagi di dalamnya atau if else,
atau bahkan dua duanya
```

```javascript
for (let i = 0; i < 5; i++) {
  console.log("Hello World!");
}
```

Mari kita breakdown kode di atas,

```
pertama i adalah index, jadi daripada menulis index lebih baik menulis i bukan ?

i bermula dari 0; lalu apakah i kurang dari 5 ? true; maka
console.log("Hello World!") di jalankan
kemudian i++, yakni i di tambah 1

i menjadi 1; lalu apakah i kurang dari 5 ? true; maka
console.log("Hello World!") di jalankan
kemudian i++, yakni i di tambah 1

i menjadi 2; lalu apakah i kurang dari 5 ? true; maka
console.log("Hello World!") di jalankan
kemudian i++, yakni i di tambah 1

i menjadi 3; lalu apakah i kurang dari 5 ? true; maka
console.log("Hello World!") di jalankan
kemudian i++, yakni i di tambah 1

i menjadi 4; lalu apakah i kurang dari 5 ? true; maka
console.log("Hello World!") di jalankan
kemudian i++, yakni i di tambah 1

i menjadi 5; lalu apakah i kurang dari 5 ? false; maka
looping akan berhenti sampai disini
```

Sampai sini paham ?

Bagaimana cara membuat output seperti ini ?

```
*
*
*
*
*
```

Dan bagaimana pula kita membuat output seperti ini ?

```
***** // 5 bintang
```

Di samping kita bisa menggunakan **i++** kita juga bisa menggunakan **i--** dan ini biasanya untuk membalikkan sesuatu,

Katakanlah kita ingin membalikkan kata "aku" menjadi "uka"

maka kita bisa menulis seperti ini

```javascript
function myReverseWord(string) {
  let result = "";

  for (let i = string.length - 1; i >= 0; i--) {
    result += string[i];
  }

  return result;
}

console.log(myReverseWord("aku"));
console.log(myReverseWord("kamu"));
console.log(myReverseWord("dia"));
```

Mari breakdown sebentar

```
Pertama kita membuat i menjadi index terakhir dari kata, masih ingat jika index di mulai dari 0 dan length di mulai dari 1 ? itulah kenapa kita membuat length di kurangi satu,

lalu looping akan berhenti saat index ke 0

dan variable result di tambahkan huruf yang di balik satu per satu

mari lihat contoh dari kata "aku"

aku mempunyai length 3, dan index di mulai dari 0, maka
a adalah index 0
k adalah index 1
u adalah index 2

maka i menjadi length yakni 3 di kurangi 1

i adalah 2, lalu apakah i lebih dari sama dengan 0 ? true, maka
result di tambahkan huruf index ke 2, yakni u
lalu i dikurangi 1

i menjadi 1, lalu apakah i lebih dari sama dengan 0 ? true, maka
result di tambahkan huruf index ke 1, yakni k
lalu i dikurangi 1

i menjadi 0, lalu apakah i lebih dari sama dengan 0 ? true, maka
result di tambahkan huruf index ke 0, yakni a
lalu i dikurangi 1

i menjadi -1; apakah i lebih dari sama dengan 0 ? false, maka looping berhenti

kemudian mereturn result;
```
