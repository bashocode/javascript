## Git Branch

Kali ini kita akan belajar tentang git branch yang berguna untuk memisahkan antara project yang fix dan yang belum, jadi cara penggunaannya dalam sebuah tim development adalah kita akan membuat branch kita sendiri lalu orang lain akan membuat branch mereka sendiri dan tetap dalam satu repository, kalian pasti pernah menggunakan **git push origin master** kan ? lalu apa itu master ?

_master_ bisa dibilang adalah induknya branch, jadi master ini akan menampung semua branch kalian yang sudah benar benar fix dan bisa di gabung loh, jadi sangat penting untuk menggunakan fitur ini.

Langsung saja kita belajar cara menggunakannya

1. Buka folder kalian yang sudah terhubung dengan repository di terminal.
   ![repo](https://github.com/bashocode/javascript/blob/master/first%20week/img/Screenshot%20from%202019-03-29%2010-26-10.png)

2. Ketik **git checkout -b [nama branch yang kamu mau, terserah]**
   ![branch](https://github.com/bashocode/javascript/blob/master/first%20week/img/Screenshot%20from%202019-03-29%2010-26-22.png)

3. Bisa di cek menggunakan **git status**
   ![status](https://github.com/bashocode/javascript/blob/master/first%20week/img/Screenshot%20from%202019-03-29%2010-26-33.png)

4. Coba ubah isi dari file kalian
   ![file](https://github.com/bashocode/javascript/blob/master/first%20week/img/Screenshot%20from%202019-03-29%2010-29-30.png)

5. Push seperti biasa namun jangan menggunakan **master** tetapi gunakan nama branch kamu
   ![push](https://github.com/bashocode/javascript/blob/master/first%20week/img/Screenshot%20from%202019-03-29%2010-27-56.png)

6. Bisa kalian liat di repo kalian ada tulisan compare and pull request silakan cari tau sendiri apa maksudnya (tugas)
   ![pull](https://github.com/bashocode/javascript/blob/master/first%20week/img/Screenshot%20from%202019-03-29%2010-28-18.png)

7. Klik tombol branch untuk cek ada berapa branch disitu
   ![tombol](https://github.com/bashocode/javascript/blob/master/first%20week/img/Screenshot%20from%202019-03-29%2010-28-34.png)

8. Setelahnya terserah kalian, di klik dan di lihat boleh, ga di apa apain juga boleh
   ![done](https://github.com/bashocode/javascript/blob/master/first%20week/img/Screenshot%20from%202019-03-29%2010-28-27.png)
