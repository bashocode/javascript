# Value of Variable

Sebelumnya pernah liat yang seperti ini ?

```javascript
let firstName;

console.log(firstName);
```

Jika kita run kode kita, maka hasilnya adalah **undefined**

```javascript
let firstName; // undefined
let myName = "Basho Code"; // string
let myAge = 20; // number
let isMarried = false; // boolean
let child = null; // null
let myCourse = ["javascript", "git"]; // array
let myJavaScript = {
  front: "react",
  back: "node"
}; // object
```

Di JavaScript, ada dua tipe data, yakni primitive dan reference.

### Primitive

dalam primitive, kita bisa menemukan **undefined, null, string, number, boolean**

##### Undefined

Undefined adalah tipe data yang jika kita mendeklarasikan sebuah variable tanpa value, maka secara default variable tersebut bernilai undefined, tetapi:

```javascript
const myName = undefined;

console.log(myName);
```

jika kita memberikan value kepada suatu variable dengan undefined, maka variable tersebut juga bernilai undefined, kenapa bisa ? karena undefined disamping sebuah tipe data, dia juga adalah value.

##### Null

null adalah tipe data yang berguna untuk menghapus value dari variable. Misalkan kita membuat sebuah variable buah

```javascript
let fruit = "apple";
```

kita sudah memilih buah tersebut bukan ? nah jika kita tidak jadi memilih buah tersebut, kita bisa gunakan null

```javascript
let fruit = "apple";

fruit = null;
```

##### String

string di tandai dengan tanda petik, boleh petik satu atau dua. Namun, disini kami menggunakan petik dua agar petik satu dapat berguna untuk hal lain, contohnya

```javascript
let eat = "don't, you're diet";
```

tapi semua kembali ke masing masing ya, karena bisa saja menggunakan seperti ini

```javascript
let eat = 'don\'t, you\'re on diet';
```

##### Number

number adalah angka, wkwkwkwk, namun di JavaScript kita bisa menggunakan:

```javascript
let myAge = 20;
let speed = 120.5;
```

ingat tanpa tanda petik ya.

##### Boolean

boolean hanya mempunyai dua value, yakni true atau false

```javascript
let isMarried = false;
let isNormal = true;
```
