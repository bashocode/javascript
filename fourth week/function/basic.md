# Funtion Declaration vs Expression

Dalam JavaScript ada dua tipe function, yakni declaration dan juga expression dan ini berbeda dengan performing atau calculating function. Silakan buka intro to function.

### Declaration

Funtion Declaration adalah function yang biasa kita gunakan,

```javascript
function play() {
  console.log('play');
}

play();
```

### Expression

Sedangkan Function Expression menggunakan variable, maksudnya function yang menjadi value dalam variable.

Dan ada dua type function expression disini, yakni anonymouse dan named.

```javascript
// anonymouse function expression
const play = function() {
  console.log('play');
};

play();

// named function expression
const read = function book() {
  console.log('reading');
};

read();
```

anonymouse tidak mempunyai nama function, berbeda dengan named, nah kita menggunakan titik koma juga **;** karena function diatas adalah value dari sebuah variable

Lalu kita juga bisa mengganti const dengan let

## Hoisting

Apa itu hoisting ? Sebelum menjawabnya mari kita coba eksperiment sebentar

```javascript
play();

function play() {
  console.log('play');
}
```

Apakah kita bisa menjalankan code diatas ?

Jawabannya bisa, kenapa ? Karena di dalam javascript semua function akan di baca terlebih dahulu alias function akan otomatis berada di atas file kita

Begini sederhananya, function akan di prioritaskan oleh compiler jadi meskipun function yang kita punya berada di paling bawah sebuah file sekalipun, compiler akan mencari function terlebih dahulu baru kemudian akan membaca code kita yang lain.

Lalu, bagaimana dengan ini ?

```javascript
play();

read();

// anonymouse function expression
const play = function() {
  console.log('play');
};

// named function expression
const read = function book() {
  console.log('reading');
};
```

Hasilnya akan error, kenapa ? karena sifatnya bukan function, mereka adalah variable yang kebetulan mempunyai value berupa function.
