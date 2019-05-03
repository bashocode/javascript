# forEach loop

Untuk iterating array, kita sudah tau bahwa kita bisa menggunakan for of loop.

Tetapi ada cara lebih simple lagi, yakni dengan menggunakan forEach

```
array.forEach((value, index) => {
    value
    index
});

atau menggunakan function biasa

array.forEach(function(value, index) {
    value
    index
});
```

array adalah variable yang akan kita iterate
forEach adalah method yang menerima dua parameter
parameter pertama adalah value, yakni isi dari array dalam variable
parameter kedua adalah index dari value

```javascript
const abjads = ['a', 'b', 'c'];

abjads.forEach((abjad, index) => {
  console.log(index, abjad);
});
```

Jika kita hanya ingin memberikan satu parameter, kita bisa menghilangkan tanda (), dan apabila kita hanya menggunakan satu line code di dalam tanda {}, kita bisa menghapus tanda {}

```javascript
const abjads = ['a', 'b', 'c'];

abjads.forEach(abjad => console.log(abjad)})
```
