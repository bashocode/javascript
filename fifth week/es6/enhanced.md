# Enhanced Object Properties

Penyingkatan syntax di dalam object bisa dilakukan setelah adanya ES6 ini

### Property Sorthand

Jika di dalam ES5 kita biasa mendeklarasikan properti object seperti ini

```javascript
var x = 0, y = 0;
var obj = {
	x: x,
	y: y
};
```

Sedangkan di ES6 kita bisa mempersingkat kodingan kita, seperti ini

```javascript
let x = 0; y = 0;
let obj = { x, y };
```

Dengan catatan nama variable dan nama propertynya kita asumsikan sama, jadi kalau misalnya seperti ini

```javascript
let a = 0; b = 0;
let obj = { x, y };
```

**x** dan **y** darimana ? Kan cuma ada **a** dan **b**, begitu kira kira.

### Methods Properties

Jika di ES5 saat kita ingin membuat function di dalam object kita biasa menggunakan

```javascript
var obj = {
	foo: function (a, b) {
		console.log(a);
		return b;
	},
	bar: function (x, z) {
		console.log(x);
		return z;
	}
};
```

Maka di ES6 kita bisa lebih membuatnya menarik seperti ini

```javascript
var obj = {
	foo (a, b) {
		console.log(a);
		return b;
	},
	bar (x, z) {
		console.log(x);
		return z;
	}
};
```
