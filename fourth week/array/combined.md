# Combined and Slicing Arrays

Kita bisa menggabungkan dua array dengan concat.

```javascript
const firstArray = [1, 2];
const secondArray = [3, 4];

const thirdArray = firstArray.concat(secondArray);

console.log(thirdArray); // [1, 2, 3, 4]
```

Lalu kita juga bisa membagi array dengan slice

```javascript
const fourthArray = thirdArray.slice(1, 3);

console.log(fourthArray); // [3];
```

Parameter pertama dari slice adalah starting index, dan yang kedua adalah finish
