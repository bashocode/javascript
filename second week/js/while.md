# WHILE in JavaScript

Di tutorial sebelumnya, kita sudah belajar tentang FOR Loop dan kali ini kita akan belajar tentang While loop, dan ada beberapa perbedaan dengan for loop.

```javascript
for (initializeExpression; condition; incrementExpression) {
  statement;
}
```

Di for loop, **initializeExpression, condition, dan incrementExpression** berada dalam satu tanda kurung kurawal, berbeda dengan while loop yang strukturnya seperti ini

```javascript
initializeExpression;

while (condition) {
  statement;
  incrementExpression;
}
```

Di while loop, intializeExpression berada di luar, lalu condition di dalam tanda kurung **()** dan incrementExpression berada dalam kurung kurawal **{}**

Kita bisa menggunakan while untuk menulis "Hello World!" 5x seperti menggunakan for

```javascript
let i = 0;

while (i < 5) {
  console.log("Hello World!");
  i++;
}
```

Hati-hati agar tidak terjadi **infinite loop**, infinite loop terjadi ketika kita melupakan sesuatu, seperti tidak memberikan incrementExpression atau bahkan tidak memberikan condition yang benar.

Jika terjadi infinite loop, biasanya laptop akan freeze atau bahkan mati sendiri, dan hal terburuk harddisk kita bisa rusak (seperti kejadian teman saya).

```
lalu kapan kita menggunakan for dan kapan menggunakan while ?

kita gunakan for,

    jika kita tau kapan kita harus menghentikan looping tersebut,
    kita tau dengan pasti condition dimana looping berhenti,

lalu, kita gunakan while,

    jika kita tidak tau kapan harus berhenti, misalkan angka harus terus menerus bertambah sampai menemukan angka prima.
```
