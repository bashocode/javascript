# Getter and Setter

Saat kita ingin memanggil sebuah function di dalam object kita harus meng*invoke*nya bukan ?

```javascript
const person = {
  firstName: 'Basho',
  lastName: 'Code',
  // 1
  fullName() {
    return `${person.firstName} ${person.lastName}`;
  }
};

console.log(person.fullName());
```

Penjelasannya

1. Kita bisa langsung menggunakan function seperti diatas, sama seperti saat kita

```javascript
const person = {
  fullName: function() {
    return 'name';
  }
};
```

Hanya saja lebih simple penggunaannya

---

Dengan menggunakan getter and setter kita tidak perlu meng*invoke*nya

```javascript
const person = {
  firstName: 'Basho',
  lastName: 'Code',

  // 1
  get fullName() {
    return `${person.firstName} ${person.lastName}`;
  },

  // 2
  set fullName(name) {
    // 3
    const yourName = name.split(' ');
    // 4
    this.firstName = yourName[0];
    this.lastName = yourName[1];
  }
};

// 5
person.fullName = 'John Doe';

console.log(person.fullName);
```

Penjelasannya

1. Kita menambahkan get sebelum nama functionnya, untuk mendapatkan valuenya
1. Set di gunakan jika kita mempassing nama lain kedalamnya, dan saat itulah get dan set bekerja
1. Kenapa split ? karena kita mempassing 'John Doe' dan ada spasi disana
1. Index ke 0 adalah John, dan ke 1 adalah Doe
1. Kita seperti memanggil function dengan mempassing valuenya (optional, boleh di comment dulu)

```javascript
person.fullName('John Doe');
```

Jadi get dan set akan bekerja jika kita memanggil functionnya tentunya tanpa _invoke_ atau kita juga ingin mengganti valuenya (jadi valuenya dinamis sesuai dengan inputan)
