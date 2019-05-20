# Arguments

Kali ini kita akan belajar tentang argumen di javascript,

```javascript
function myName() {
  console.log(arguments);
}

myName('bashocode');
```

arguments adalah cara memanggil parameter yang tak bernama, namun jika kita jalankan kode diatas maka yang keluar adalah object

Lalu bagaimana caranya agar kita bisa mengakses value dari arguments ?

```javascript
function myName() {
  for (let value of arguments) {
    console.log(value);
  }
}

myName('bashocode', 'basho', 'code');
```

Kita bisa menggunakan for of loop, loh bukannya for of untuk array ? inikan object harusnya for in donk

Benar, tetapi ini pengecualian, kalau kita menggunakan for in loop yang keluar nanti malah keynya bukan valuenya.

Kalau tidak percaya, coba kode ini

```javascript
function myName() {
  for (let key in arguments) {
    console.log(key);
  }
}

myName('bashocode', 'basho', 'code');
```
