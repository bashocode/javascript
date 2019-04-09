# For-in in JavaScript

For-in berbeda dengan for loop, for-in tidak memiliki initializeExpression, condition, atau incrementExpression. Contohnya

```javascript
for (let blabla in blabla) {
  statement;
}
```

Lihat, di dalam tanda kurung **()** hanya ada let dan in, mari kita lihat contohnya dalam me looping object

```javascript
const person = {
  name: "Ikhda",
  age: 20,
  gender: "Man"
};

for (let key in person) {
  console.log(key);
}
```

Hasilnya

```
name
age
gender
```

key akan mengambil key dari object, dan bagaimana cara kita memunculkan value di dalam key ? Sebelumnya kita sudah belajar bahwa cara untuk memunculkan value dalam key di object ada dua cara, yakni dot notation dan bracket notation.

Jika sebelumnya kita menggunakan dot notation sebagai best practice yakni sebagai praktek sehari hari, namun hal itu tidak akan berhasil karena kita tidak tau persis nama dari key.

Dan untuk itulah ada bracket notation, yang mana memang di peruntukkan jika kita tidak tau nama dari key karena keynya berbeda beda.

```javascript
const person = {
  name: "Ikhda",
  age: 20,
  gender: "Man"
};

for (let key in person) {
  console.log(person[key]);
}
```

Hasilnya

```
Ikhda
20
Man
```

Lihat, bahwa kita memanggil **person** di ikuti **key** di dalam bracket.

Lalu, apa kita bisa menggunakan for-in untuk array ? Tentu bisa, namun ada **for-of** yang bisa di gunakan untuk array.

contoh penggunaan for-in untuk array

```javascript
const number = [1, 2, 3];

for (let index in number) {
  console.log(number[index]);
}
```

hasilnya

```
1
2
3
```

Tapi kita akan belajar for-of yang di gunakan untuk array
