# Reverse

Apa itu ? Dunia paralel ? atau dunia kebalikan ? Yap betul....

Reverse di gunakan untuk membaca dari belakang ke depan, misalkan kita ingin membalikkan **bashocode** menjadi **edocohsab**

Kita bisa gunakan cara manual, yakni looping

```javascript
function myReverse(string) {
  let result = "";

  for (let i = string.length - 1; i >= 0; i--) {
    result += string[i];
  }

  return result;
}

console.log(myReverse("bashocode"));
```

Looping yang kita gunakan adalah kebalikan, dan i di awali dari length string di kurangi 1, ingat bahwa index dimulai dari 0 dan length dimulai dari 1 bukan ?

Kemudian kondisinya adalah jika lebih dari 0 atau sama dengan 0

Lalu yang terakhir expressionnya adalah decrement

Atau kita bisa menggunakan cara singkat

```javascript
function reverseString(str) {
  return str
    .split("")
    .reverse()
    .join("");
}

console.log(reverseString("bashocode"));
```

Split adalah cara untuk memisahkan string per karakter, logikanya sama kayak kita menggunakan for, jadi di ambil satu per satu,

```
b
a
s
h
o
c
o
d
e
```

Lalu Reverse adalah fungsinya membalikkan string yang sudah terpisah pisah

```
e
d
o
c
o
h
s
a
b
```

Baru kemudian Join, untuk menambahkan karakter menjadi satu

```
edocohsab
```

Well, mau pilih cara mana itu terserah, namun cara manual bisa melatih otak kita untuk paham alur kerja dari komputer, maka saya sarankan teruslah berlatih logic dengan mengerjakan sesuatu menggunakan cara manual di samping menggunakan built in method (gunakan bebarengan)
