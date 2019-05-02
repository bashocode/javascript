# The Spread Operator

Di ES6 ada cara yang lebih mudah untuk menggabungkan dua array atau lebih, yakni menggunakan spread (...)

```javascript
const firstArr = [1, 2, 3];
const secondArr = [7, 8, 9];

const thirdArr = [...firstArr, secondArr];
// [1, 2, 3, 7, 8, 9]

const fourthArr = [...firstArr, 4, 5, 6, ...secondArr];
// [1, 2, 3, 4, 5, 6, 7, 8, 9]
```

Bahkan kita bisa menambahkan apapun di dalamnya,

```
... => akan mengambil semua value dari variable yang dia panggil
[] => akan menjadi array baru yang mempunyai value dari spread operator dan value yang di input manual
```
