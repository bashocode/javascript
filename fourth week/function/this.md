# This

Sebelumnya kita telah melihat this, dan kali ini kita akan mencoba memahami apa itu this.

### This in Method

Jika kita punya function di dalam sebuah object maka function ini dinamakan method

```javascript
const book = {
  title: 'JavaScript',
  read() {
    console.log(this);
  }
};

book.read();
```

Kode diatas akan memunculkan semua isi dari object tersebut.

Atau kita ingin menambah method lain ?

```javascript
const book = {
  title: 'JavaScript',
  read() {
    console.log(this);
  }
};

book.mark = function() {
  console.log(this);
};

book.read();
```

Hasilnya juga akan memunculkan semua isi di dalam object

### This in Function

Nah, jika di dalam function murni kita tidak menggunakan seperti dibawah ini

```javascript
function book() {
  console.log(this);
}

book();
```

Tetapi, bisa menggunakan new.

```javascript
function Book(title) {
  this.title = title;
  console.log(this);
}

const newBook = new Book('JavaScript is Nice');
```

Coba jalankan kode diatas.

```
this.title => akan membuat sebuah key baru berupa title dan mempunyai value dari parameter title
new Book() => akan menjalankan function untuk membuat buku baru dengan judul yang di passing
```
