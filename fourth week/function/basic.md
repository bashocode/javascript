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
}

read();
```

anonymouse tidak mempunyai nama function, berbeda dengan named, nah kita menggunakan titik koma juga **;** karena function diatas adalah value dari sebuah variable

Lalu kita juga bisa mengganti const dengan let
