# Intro to Object

Object adalah salah satu dari **reference data types** disamping array and function

Bayangkan ada seorang manusia, dia mempunyai nama, umur, tinggi, berat, warna kulit, dll. Manusia adalah object yang mempunyai properti, sama seperti object dalam JavaScript, dia juga punya property. Mari lihat contoh:

```javascript
let person = {
  name: "Ikhda Muhammad Wildani",
  age: 20,
  height: 168,
  weight: 45
};
```

object di tandai dengan **{}** dan di belakang tanda **:** di namakan _key_ sedangkan setelahnya berupa data types, lalu paling belakang ada **,** tanda koma di gunakan jika kita ingin menambahkan properti lainnya, lihat yang paling bawah tidak ada tanda koma bukan?

Lalu bagaimana cara mengakses properti dalam object ?

```javascript
person;
console.log(person); // akses semua properti

// akses salah satu properti menggunakan dot notation
person.name;
console.log(person.name);

// akses menggunakan bracket
person["name"];
console.log(person["name"]);
```

best practicenya adalah menggunakan dot notation, demikian juga cara untuk mengubah valuenya, yakni menggunakan dot notation

```javascript
person.name = "Basho Code";
console.log(person.name);
```
