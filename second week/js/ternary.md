# Ternary Operator

Sebuah sekolah ingin memilah siswa yang lulus dan yang tidak, yang nilainya 80 keatas akan lulus dan yang di bawahnya akan gagal.

```javascript
const gradePoint = 80;
const isGraduated = gradePoint >= 80 ? "lulus" : "tidak lulus";

console.log(isGraduated); // Lulus
```

Comparison Operator akan menghasilkan true atau false, dan dengan ternary kita bisa mengubah true atau false menjadi yang kita inginkan,

```
valueOne > valueTwo ? "outputTrue" : "outputFalse"
```

Ingat! ada tanda **?** dan **:**

dan sebelah kanan dari **:** adalah _true_, dan kirinya adalah _false_
