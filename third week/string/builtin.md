# Built In Function of String

### Length

Length di gunakan untuk menghitung panjang karakter sebuah variable, berbeda dengan Index yang dimulai dari 0, length dimulai dari 1

```javascript
const bootcamp = "bashocode";

// untuk mengetahui panjang string
const stringLength = bootcamp.length; // 9

// untuk mengambil karakter terakhir
const lastString = bootcamp[bootcamp.length - 1]; // e
// bootcamp.length = 9
// bootcamp.length - 1 = 8

// untuk mengambil karakter pertama

const firstString = bootcamp[0];
// or
const anotherFirstString = bootcamp.charAt(0);
```

### Comparing

Untuk membandingkan sebuah string, biasanya menggunakan

```javascript
function compareString(params1, params2) {
  if (params1 === params2) return true;
  else return false;

  // or

  /*
  if (params1 === params2)
    return true;
  else
    return false;
  */
}

const bootcamp = "bashocode";
const anotherBootcamp = "basho";
const onlineBootcamp = "code";
const learnCode = "bashocode";

console.log(compareString(bootcamp, learnCode)); // true
console.log(compareString(anotherBootcamp, onlineBootcamp)); // false
```

**tips**

> Jika setelah if/else hanya ada satu baris statement, kita bisa menghilangkan kurung kurawal

Namun, ada cara yang lebih mudah yakni menggunakan localCompare

```javascript
var a = "hello";
var b = "world";

console.log(a.localeCompare(b)); // -1
```

-1 untuk false, dan 1 untuk true.

### Index Of

Index Of adalah cara untuk mencari index darisuatu karakter yang kita ingin cari.

cara manual

```javascript
function myIndexOf(string, char) {
  for (let i = 0; i < string.length; i++) {
    if (string[i] === char) {
      return i;
    }
  }
}

console.log(myIndexOf("bashocode", "a")); // 1
```

dengan built in function

```javascript
const bootcamp = "bashocode";

const indexOfBootcamp = bootcamp.indexOf("a");

console.log(indexOfBootcamp);
```

Bahkan kita bisa mencari kata dalam suatu kalimat

```javascript
const bootcamp = "basho code";

const indexOfBootcamp = bootcamp.indexOf("code");

console.log(indexOfBootcamp);
```
