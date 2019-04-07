# Comparison II

Setelah sebelumnya kita sudah belajar tentang Relational, sekarang kita akan mempelajari Equality

### Equality

Equality ada dua cabang, yang pertama adalah Strict Equality dan yang kedua adalah Lose Equality. Apa perbedannya ? Jawabannya terserah anda, mari kita lihat

##### Strict Equality

Strict Equality ada dua, yakni **===** dan **!==**

**===** // sama dengan
**!==** // tidak sama dengan

```javascript
console.log(1 === 1); // true
console.log("1" === 1); // false
```

Strict Equality hanya akan true jika yang di bandingkan sama **tipe data** dan sama **value**-nya

Tipe data sudah kita pelajari sebelumnya bukan.

```javascript
console.log(1 !== 1); // false
console.log("1" !== 1); // true
```

Saya kira contoh yang diatas sudah paham, mari lanjut

##### Lose Equality

Lose Equality berupa **==** dan **!==**

Berbeda dengan Strict, Lose hanya membandingkan valuenya dan mengabaikan tipe data.

```javascript
console.log(1 == 1); // true
console.log("1" == 1); // true
```

Kode di atas adalah contoh nyata, lalu bagaiman cara kerjanya ? kita ambil contoh yang kedua yang membandingkan string dan number

Komputer mengambil value di sisi kiri, dan dia menemukan bahwa tipe datanya string, maka sisi kanan akan otomatis di convert ke tipe data string.

Lalu bagaimana dengan ini ?

```javascript
console.log(true == 1); // true
```

Bagaimana bisa true di bandingkan dengan 1 hasilnya true ?
Seperti sebelumnya, komputer akan mengconvert angka 1 menjadi tipe data yang sama dengan yang sebelah kiri, kebetulan

angka 1 adalah true

maka true di bandingkan dengan true

hasilnya akan true bukan ?

---

Lalu bagaimana dengan ini ?

```javascript
console.log(true == 0); // false
```

Kenapa hasilnya false ? nah kalian akan menemukan jawabannya jika sudah tau tentang apa itu **truthy** dan **falsy**

Silakan coba coba menggunakan operator **!=**
