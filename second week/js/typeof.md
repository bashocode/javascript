# TypeOf in JavaScript

Kita bisa mencari tau apa tipe data dari sebuah value, misalnya

```javascript
console.log(typeof 42); // "number"
console.log(typeof "blue"); // "string"
console.log(typeof true); // "boolean"
console.log(typeof null); // "object"
console.log(typeof ["blue"]); // "object"

// kenapa null dan array adalah object ? Well, I don't know exactly. So, let's make it our task to find the answer

const temp;
console.log(typeof temp); // "undefined" => ingat bahwa default value adalah undefined
```

Lalu kapan kita bisa menggunakan typeof ? kita mungkin akan menemukan kasus dimana kita harus cek bahwa inputan dari user adalah number dan bukan string

```javascript
function validateNumber(number) {
  if (typeof number !== "number") {
    console.log("please insert valid number");
  }

  console.log("valid"); // jika berupa number maka akan mengirim pesan
}

validateNumber("himitsu");
```
