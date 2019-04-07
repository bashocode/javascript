# Logical Operator II

Sebelumnya kita sudah belajar Logical Operator dengan Boolean, saatnya kita belajar non-Boolean

```javascript
console.log(false || "Ikhda"); // Ikhda
console.log(false || 1); // 1
console.log(0 || "Ikhda"); // Ikhda
console.log(0 || 1); // 1
```

Saatnya membahas **truthy** dan **falsy** agar semakin paham,

falsy terdiri dari

```javascript
false;
undefined;
null;
0;
(""); // string kosong
NaN;
```

dan truthy adalah sesuatu selain falsy

Logical Operator **||** akan mengembalikan nilai true jika salah satunya bernilai true bukan ? dan truthy sebenarnya juga berupa true, jadi truthy akan di kembalikan.

```javascript
console.log(false || "Ikhda" || 1); // Ikhda
```

Contoh di atas ada dua value yang bernilai true bukan ? kenapa yang muncul hanya true yang pertama yakni **"Ikhda"** ?

Iya, betul. Operator akan mengembalikkan nilai true pertama yang mereka dapat, jadi true berikutnya meskipun ada berjuta juta akan tetap di lupakan.
