# Sorting an Array

Jika kita ingin mengurutkan array, kita bisa menggunakan sort dan reverse

Sort jika kita ingin mengurutkan dari bawah ke atas, dan reverse dari atas ke bawah

```javascript
const numbers = [3, 1, 2];

numbers.sort(); // [1, 2, 3]

numbers.reverse(); // [3, 2, 1]
```

Tapi cara ini tidak akan berhasil jika

```javascript
const courses = [{ id: 1, name: 'React.js' }, { id: 2, name: 'Node.js' }];

courses.sort();
```

Kita harus menggunakan cara ini

```javascript
const courses = [{ id: 1, name: 'React.js' }, { id: 2, name: 'Node.js' }];

courses.sort(function(a, b) {
  // a < b => -1
  if (a.name < b.name) return -1;
  // a > b => 1
  if (a.name > b.name) return 1;
  // a === b => 0
  if (a.name === b.name) return 0;
});
```

Kita menggunakan function yang menerima parameter a dan b, yakni value yang akan kita bandingkan, dan kita akan mereturn -1 jika huruf awal dari a lebih kecil dari huruf awal dari b

Tapi jika hurufnya berbeda, R dan r kan berbeda, kita tidak bisa menggunakan cara diatas. Jadi kita harus convert dulu ke huruf kecil semua atau huruf besar semua

```javascript
const courses = [{ id: 1, name: 'React.js' }, { id: 2, name: 'Node.js' }];

courses.sort(function(a, b) {
  const A = a.name.toUpperCase();
  const B = B.name.toUpperCase();

  if (A < B) return -1;
  // a > b => 1
  if (A > B) return 1;
  // a === b => 0
  if (A === B) return 0;
});
```
