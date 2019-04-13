# Variable Naming Rules

Kali ini kita akan belajar tentang aturan aturan dalam penamaan variable

1. Menggunakan bahasa inggris untuk penamaan variablenya

1. Di mulai dari huruf, underscore **\_**, atau dollar **\$**

1. Tidak bisa di awali dengan nomor

   Jangan menulis variable dengan sebutan 1name, 2name, dan lainnya yang di awali dengan angka. Tidak akan bisa!

1. Tapi setelah karakter pertama, boleh menggunakan nomor contohnya name1, name2

1. Jangan gunakan _reserved word_ seperti if, else, if else, undefined, null, dll.

   Tidak perlu menghafalkan reserved word, namun semakin kesini kita akan semakin faham apa itu reserved word, reserved word itu kata yang sudah ada di syntax javascript, jika kita menulis di VS Code maka nantinya akan ada garis bawah berwarna merah, dan tandanya kita tidak bisa menggunakannya.

1. Harus bisa di pahami

   Jangan menulis variable dengan sesuatu yang tidak bisa di pahami seperti a, b, c, atau bahkan z. Apa coba maksudnya ?

1. Tidak bisa menambah spasi atau strip (-)
1. Case-Sesitive alias huruf besar dan kecil berpengaruh
1. Sebaiknya menambahkan ; (titik koma) di belakang
1. Menggunakan Camel Notation

   Camel itu unta ya, dan camel notation itu di ibaratkan seperti punuk unta, jika kita ingin menulis variable dengan dua kata atau lebih, kita tidak bisa menggunakan spasi atau strip bukan ? maka camel notation hadir untuk menyelesaikan masalah ini, contohnya bisa di lihat di bawah:

```javascript
const if = "something"; // Tidak boleh
const a = "jangan"; // Tidak bisa di pahami
const 1name = "basho"; // Tidak bisa
const full-name = "parah"; // Jangan, ga bakal bisa

// contoh yang di perbolehkan

const _handleRegister = "something";
const $handleLogin = "else";

let firstName;
// berbeda dengan
let FirstName;

let myNameIsBashoCode = "inilah yang di namakan camel notation";
```

Selanjutnya kita akan membahas value di variable
