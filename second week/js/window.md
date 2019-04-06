# Window in JavaScript

Window di JavaScript ada beberapa macam, disini kita akan belajar tentang:

```javascript
window.console.log("ore ga console");
window.alert("ore ga alert");
window.prompt("ore ga prompt");
window.confirm("ore ga confirm");
```

atau bisa di gunakan tanpa window

```javascript
console.log("ore ga console");
alert("ore ga alert");
prompt("ore ga prompt");
confirm("ore ga confirm");
```

Lalu bagaimana dan apa kegunaannya ?

Untuk mengetahuinya kita perlu membuat sebuah file html bukan ?
Baiklah mari kita buat sebuah folder terlebih dahulu, dan kita akan memisahkan file html dan file js kita.
Buatlah folder bernama latihan atau apapun terserah, lalu di dalam folder tersebut buatlah file bernama _index.html_ dan _index.js_

di file index.html, harusnya tidak berbeda dengan ini.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <title>Document</title>
  </head>
  <body>
    <h1>Hello World!</h1>

    <!-- Script in Here -->
    <script src="index.js"></script>
  </body>
</html>
```

lalu di file index.js

```javascript
console.log("ore ga console");
alert("ore ga alert");
prompt("ore ga prompt");
confirm("ore ga confirm");
```

Kemudian buka file index.html di browser, dan coba klik kanan di mana saja lalu pilihlah _inspect_ kemudian cari tab _console_

_console_ akan mengeluarkan apa yang kita _console.log_ dan alert, prompt, dan confirm akan muncul otomatis di layar saat kita membuka file html kita, bagaimana ? keren bukan.

Tutorial berikutnya akan membahas tentang variable di JavaScript
