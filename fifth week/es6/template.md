# Template Literals

Kali ini kita akan mengulang kembali materi tentang template literals yang sering kita gunakan, karena template literals adanya di ES6 maka kita akan belajar lagi di modul ini.

### String Interpolation

Kita menggunakan template literals di multi-line ataupun single-line strings.

```javascript
const customer = { name: 'John Doe' };
const cart = {
	amount: 7,
	product: 'chicken',
	price: 5
};
const message = `Hello ${customer.name},
do you want to buy ${cart.amount} ${cart.product} for
${cart.amount * cart.price} ?`;

console.log(message);
```

Kita bisa menggunakan code diatas ketimbang harus menggunakan code lama seperti ini

```javascript
var customer = { name: 'John Doe' };
var cart = {
	amount: 7,
	product: 'chicken',
	price: 5
};
var message = 'Hello ' + customer.name ',\n do you want to buy ' + cart.amount + ' ' + cart.product + ' for ' + (cart.amount * cart.price) + ' ?';

console.log(message);
```

### Custom Interpolation

Kita juga bisa menggunakan template literals untuk yang lain seperti link website beserta parameter misalkan

```javascript
const username = 'bashocode';
const repository = 'javascript';
const github = `https://github.com/${username}/${repository}`;

console.log(github);
```

Dan lebih fleksible ketimbang ES5

```javascript
var username = 'bashocode';
var repository = 'javascript';
var github = 'https://github.com/' + username + '/' + repository;

console.log(github);
```
