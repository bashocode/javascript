# Variable di JavaScript

Kita sudah install _node js_ bukan ? Nah di kesempatan kali ini kita tidak akan menggunakan console di web browser tetapi menggunakan terminal, nah jika kita menggunakan VS Code maka kita tinggal cari tab _terminal_ dan klik _New Terminal_ maka otomatis kita akan punya terminal di dalam VS Code jadi tidak perlu repot repot buka terminal bawaan PC ya.

Di dalam JavaScript versi sebelum ES6 atau EcmaScript 2015, kita hanya bisa menggunakan _var_ namun belakangan ini, _var_ mulai di tinggalkan dan di gantikan oleh _let_ atau _const_.

```javascript
var
let
const
```

Kenapa var di tinggalkan ? alasannya adalah let/const bisa mengurangi semacam bug dalam javascript, hmm untuk contohnya bisa kita lihat

```javascript
var name = "basho";
var name = "code";

console.log(name);
```

Jika kita run code kita di terminal dengan asumsi bahwa file kita bernama index.js dan kita ketikkan di terminal _node index.js_ maka yang keluar di terminal adalah **code** kenapa ? karena name di deklarasikan ulang dengan value yang berbeda di dalam _var_ nah, _let/const_ meminimalisir hal ini, agar kedepannya tidak terjadi bug bug yang tidak perlu,

```javascript
let name = "basho";
let name = "code";

console.log(name);
```

Jika kita menjalankan kode ini, maka hal yang terjadi adalah error, kenapa ? karena name sudah pernah di deklarasikan, kenapa di deklarasi ulang ? gw ini udah ada loh, parah lu mau duain gw. Seperti itu lah kira kira.

Maka dari itu, kita akan menanamkan di mindset kita bahwa kita tidak akan menggunakan _var_ dimanapun dan kapanpun wkwkwkwkwkwk

### Let

_let_ di gunakan jika kita ingin merubah nilainya di masa depan, misalkan kita ingin menambah nama kita di variable name dari Basho menjadi Basho Code, maka kita bisa gunakan let.

```javascript
let name = "basho";

name += " code";
// atau
name = name + " code";

// sama saja, pilih salah satu

console.log(name);
```

kemudian kita akan membahas const

### Const

const itu constant, dan sesuai namanya value di variable const nilainya tetap dan tidak akan bisa di rubah

```javascript
const name = "basho";
const name = "code";

console.log(name);
```

jika kita menjalankan code di atas, maka hasilnya akan error. Dan mulai sekarang dan seterusnya jangan gunakan _var_ tapi gunakanlah _let/const_ sesuai dengan kondisi masing masing, apakah mau di rubah nilainya atau di jadikan tetap.
