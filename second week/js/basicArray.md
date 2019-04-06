# Intro to Array

Array berbeda dengan object, jika object menggunakan tanda **{}** maka array menggunakan **[]** lalu penggunaannya juga berbeda, array di gunakan jika datanya berupa list.

```javascript
let anime = ["naruto", "one piece", "dragon ball"];

// akses index menggunakan bracket notation
anime[0]; // isinya naruto
anime[1]; // isinya one piece
anime[2]; // isinya dragon ball
```

kita juga bisa menggantinya atau menambahkannya loh

```javascript
let anime = ["naruto", "one piece", "dragon ball"];

anime[0] = "something";

// silakan di coba sendiri

anime[3] = "else";
anime[4] = 23; // array juga bisa di isi tipe data lain selain string, contohnya number.

// penasaran hasilnya ?
```

Ingat ya, **index di mulai dari 0**. Itulah kenapa _naruto_ ada di anime index ke 0.

Lalu berbeda dengan index yang dimulai dari 0, **length** dimulai dari 1.

```javascript
let anime = ["naruto", "one piece", "dragon ball"];

anime.length; // hasilnya 3
```

Jadi hal menariknya jika kita ingin mengambil sebuah value paling terakhir, kita bisa gunakan **length**

```javascript
let anime = ["naruto", "one piece", "dragon ball"];

anime[anime.length - 1]; // hasilnya dragon ball
```

kenapa length - 1 ? pikirkan ya, jangan lanjut kalau belum nemu jawabannya!
