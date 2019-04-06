# Intro to Function

Function bisa digunakan untuk kita yang ingin membuat sebuah tugas yang bisa di akses berulang ulang, tanpa perlu menulis kembali.

```javascript
// Performing a Task

function hello() {
  console.log("Hello World!");
}

hello(); // Hasilnya Hello World!
```

function di tulis di awal dan di ikuti nama functionnya lalu tanda kurung **()** kemudian **{}** dan di dalam kurung kurawal **{}** terdapat kode yang bisa kita akses.

```javascript
// Performing a Task

function hello(name) {
  console.log("Hello " + name);
}

hello("Ikhda"); // Hello Ikhda
hello("Muhammad"); // Hello Muhammad
hello("Wildani"); // Hello Wildani
```

**(name)** adalah parameter dan bisa di panggil di dalam function, parameter bisa lebih dari satu.
**("ikhda")** adalah argumen dan inilah yang di lempar ke function, bisa lebih dari satu.

tapi bagaimana jika jumlah parameter dan argumen berbeda ?

```javascript
function hello(name, age) {
  console.log("Hello " + name + " " + age);
}

hello("Ikhda"); // Hello Ikhda undefined
```

maka parameter age akan berupa undefined, karena tidak ada valuenya.

function di atas adalah performing, ada juga function berupa calculate yang me **return** sesuatu

```javascript
function calculateNumber(number1, number2) {
  return number1 * number2;
}

const result = calculateNumber(3, 4);
console.log(result);

// atau langsung
console.log(calculateNumber(3, 4));
```
