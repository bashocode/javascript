# Backtick in JavaScript

Backtick **``** ada sebelum angka 1 di keyboard kita, dan ini adalah fitur baru dari ES6 atau ES2015

Sebelumnya kita sudah mencoba kode ini bukan

```javascript
function validateName(string) {
  for (let i = 0; i < string.length; i++) {
    if (Number(string[i])) {
      return 'ini index ke ' + i + ' dan berupa angka ' + string[i];
    }
  }
}

const name = 'w3basho';
console.log(validateName(name));
```

Daripada kita menulis

```javascript
return 'ini index ke ' + i + ' dan berupa angka ' + string[i];
```

Dengan backtick kita bisa menulis lebih mudah, tanpa menggunakan operator **+**

```javascript
function validateName(string) {
  for (let i = 0; i < string.length; i++) {
    if (Number(string[i])) {
      return `ini index ke ${i} dan berupa angka ${string[i]}`;
    }
  }
}

const name = 'w3basho';
console.log(validateName(name));
```

Namun, kita harus menambahkan dollar dan kurung kurawal ya

Dan kita juga bisa menggunakan backtick ini untuk memberikan break line

```javascript
const paragraph = `I am a new paragraph.
And, you can make a new 'break line' inside of me.`;

console.log(paragraph);
```
