# Switch Case in JavaScript

Sebelumnya kita sudah belajar tentang IF ELSE dan sekarang kita akan berkenalan dengan Switch Case dimana fungsinya hampir sama dengan IF ELSE namun dengan kode yang lebih banyak dibandingkan IF ELSE.

```javascript
switch (key) {
  case value:
    statement;
    break;

  default:
    statement;
    break;
}
```

Di atas adalah pattern dari penulisan Switch-Case, **(key)** adalah apa yang kita kondisikan, dan **value** adalah isi dari keynya, lalu **statement** bisa kita lakukan sesuatu di dalamnya dan bisa lebih dari satu statement.

```
Key => biasanya adalah variable yang kita ingin cek
value => isi dari variable tersebut
break => break di gunakan untuk keluar dari kondisi, jika kita tidak menggunakan break maka semua statement di dalam case akan di jalankan
default => adalah kondisi yang di jalankan jika tidak ada case yang bernilai true
```

Misalnya pengguna memberikan inputan bulan berupa angka, dan kita ingin merubah angka tersebut menjadi januari sampai desember, kita bisa gunakan seperti ini

```javascript
let bulan = 5;
let some;

switch (bulan) {
  case 1:
    bulan = "Januari";
    some = "adalah bulan pertama";
    break;
  case 2:
    bulan = "Februari";
    some = "adalah bulan kedua";
    break;
  case 3:
    bulan = "Maret";
    some = "adalah bulan saat aku mengenangnya";
    break;
  case 4:
    bulan = "April";
    some = "di bulan ini RA Kartini lahir";
    break;
  case 5:
    bulan = "Mei";
    some = "adalah bulan lahirku";
    break;
  case 6:
    bulan = "Juni";
    some = "bulan ini bulan lahir temanku";
    break;
  case 7:
    bulan = "Juli";
    some = "saudaranya si juni";
    break;
  case 8:
    bulan = "Agustus";
    some = "bulan di mana Indonesia merdeka";
    break;
  case 9:
    bulan = "September";
    some = "bulan yang ke sembilan";
    break;
  case 10:
    bulan = "Oktober";
    some = "bulan apa ya";
    break;
  case 11:
    bulan = "November";
    some = "hm kenapa dengan bulan ini ya";
    break;
  case 12:
    bulan = "Desember";
    some = "bulan terakhir menuju tahun baru";
    break;
  default:
    bulan = "Bulan itu cuma dari angka 1 sampe 12 woe";
    break;
}

console.log(bulan, some);
```

Bagaimana jika kita lupa untuk menambahkan break ? Ya ! Semua statement akan di jalankan dari case yang terpilih sampai case terakhir.

Dan kondisi diatas bisa kita rubah ke dalam IF-ELSE loh, mau tau ? Coba aja
