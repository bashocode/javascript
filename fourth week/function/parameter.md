# Parameter

Mari kita belajar lebih dalam tentang Parameter sebuah function

```javascript
function shopping(price, discount) {
  const disc = discount * 100;
  return price - disc;
}

console.log(shopping(999));
```

Apa yang terjadi jika kita jalankan kode diatas ? Yap, that's right

Jadi kita akan menggunakan cara ini

```javascript
function shopping(price, discount) {
  discount = discount || 0.2;

  const disc = discount * 100;
  return price - disc;
}

console.log(shopping(999));
```

Tau kan maksud kode diatas ? Jika paham truthy dan falsy pasti ngeh

Nah, di ES6 kita bisa menggunakan cara yang lebih simple yakni

```javascript
function shopping(price, discount = 0.2) {
  const disc = discount * 100;
  return price - disc;
}

console.log(shopping(999));
```
