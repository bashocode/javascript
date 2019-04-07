# Console in JavaScript

Kita pasti sudah tau bukan tentang **console.log()** ? Nah, ternyata masih ada yang lain loh selain _log_, contohnya:

```javascript
const datas = [
  {
    name: "Ikhda",
    course: "Front End"
  },
  {
    name: "Muhammad",
    course: "Back End"
  },
  {
    name: "Wildani",
    course: "Mobile App"
  }
];

console.table(datas);
```

Maka hasilnya akan berupa table seperti ini:
![]()

Dan masih banyak contoh lain seperti

```javascript
console.assert();
console.clear();
console.count();
console.debug();
console.dir();
console.dirxml();
console.error();
console.group();
console.groupCollapsed();
console.groupEnd();
console.info();
console.log();
console.markTimeline();
console.profile();
console.profileEnd();
console.table();
console.time();
console.timeEnd();
console.timeStamp();
console.timeline();
console.timelineEnd();
console.trace();
console.warn();
```

Untuk saat ini kita cukup tau **console.log()** saja karena sebenarnya console.log sudah cukup untuk debugging kode kita, dan memang console lain jarang di gunakan.
