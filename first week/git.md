# Belajar GIT

## Create Github Account

Tugas kalian adalah membuat akun [github](https://github.com/) !!

### Set config git

open terminal kalian dan ketikkan satu per satu

```
git config --global user.name "Basho Code"
git config --global user.email bashocode@gmail.com
```

pastikan email sesuai dengan akun github kalian ya

oh iya, apa itu **--global** ? ini di gunakan agar kita tidak perlu mengetik perintah seperti di atas berkali kali, jadi cukup sekali saja.

## Create new repository

1. Masuk ke profile git kalian, tampilannya seperti ini.

![profile](https://github.com/bashocode/javascript/blob/master/first%20week/img/Screenshot%20from%202019-03-12%2022-31-22.png)

2. Setelah itu klik repositories

![repo](https://github.com/bashocode/javascript/blob/master/first%20week/img/Screenshot%20from%202019-03-12%2022-31-23.png)

3. Dan klik tombol hijau bernama **new**, setelah itu tampilannya akan seperti ini

![new](https://github.com/bashocode/javascript/blob/master/first%20week/img/Screenshot%20from%202019-03-12%2022-31-37.png)

4. Kali ini kita akan membuat web page pertama kita, dan formatnya seperti ini **[username_kamu].github.io** karena username github saya **emzhofb** maka repositorynya **emzhofb.github.io** begitu juga dengan **bashocode.github.io** lalu pastikan public ya, jangan private dan juga jangan lupa centang _initialize this repository with README_

![username](https://github.com/bashocode/javascript/blob/master/first%20week/img/Screenshot%20from%202019-03-12%2022-31-48.png)

5. Nah, tugas kalian selanjutnya adalah membuat file html dan css boleh juga menyematkan gambar dan upload di github kalian. gimana cara uploadnya ?

## How to upload github

Sebenarnya ada banyak cara untuk upload ke github repositories kita, bisa pakai git remote, lalu via upload langsung tanpa terminal, tapi disini kita akan gunakan cara mudah terlebih dahulu, yakni git clone.

1. Masuk ke akun kalian, dan pilih repositories yang kalian buat sebelumnya ya.

![repo](https://github.com/bashocode/javascript/blob/master/first%20week/img/Screenshot%20from%202019-03-12%2022-47-26.png)

2. Lalu carilah tombol berwarna hijau bertuliskan **clone or download** lalu copy linknya ya

![clone](https://github.com/bashocode/javascript/blob/master/first%20week/img/Screenshot%20from%202019-03-12%2022-47-36.png)

3. Setelah itu masuk ke terminal kalian dan masuk ke directory/folder yang kalian inginkan

![folder](https://github.com/bashocode/javascript/blob/master/first%20week/img/Screenshot%20from%202019-03-12%2022-59-23.png)

4. Ketikkan perintah **git clone [link yang tadi kamu copy]** paste dengan _ctrl+shift+v_ di terminal

![git clone](https://github.com/bashocode/javascript/blob/master/first%20week/img/Screenshot%20from%202019-03-12%2022-59-29.png)

5. CD lagi ke directory yang kalian clone dari github dan setelah itu masuk ke code editor masing masing, disini saya menggunakan visual studio code jadi saya cukup ketikkan perintah _code ._ di terminal

![cd](https://github.com/bashocode/javascript/blob/master/first%20week/img/Screenshot%20from%202019-03-12%2023-00-26.png)

6. Masukkan file html dan css yang kalian buat sebelumnya kedalam folder repositorynya ya, disini saya membuat file baru untuk contoh

![file](https://github.com/bashocode/javascript/blob/master/first%20week/img/Screenshot%20from%202019-03-12%2023-00-38.png)

7. Setelah siap di upload ketikkan:
   - **git add .** => _git add titik_ fungsinya untuk menambahkan semua file di dalam directorynya atau gunakan **git add [nama_file]** untuk upload satu file saja
   - **git commit -m "pesan kamu"** => untuk membantu orang lain tau apa yang sebenarnya kamu upload, contohnya "upload file html" dan saya sarankan jangan asal ya, kelihatan ga professional nanti kalau github kamu di cek oleh calon boss haha _ups_
   - **git status** => sifatnya opsional, untuk cek statusnya saja
   - **git pull origin master** => nah ini sebenarnya untuk cek apakah di github kalian ada orang lain yang update atau tidak, jadi kalau misalkan ada yang update maka otomatis file kalian berubah sesuai yang di github, jadi hati hati ya menggunakan perintah ini, saya sarankan kalau repo kalian hanya kalian sendiri yang jadi contributor, maka cukup langkahi saja step ini
   - **git push origin master** => inilah saat yang kita tunggu tunggu, upload ke github haha

![push](https://github.com/bashocode/javascript/blob/master/first%20week/img/Screenshot%20from%202019-03-12%2023-02-04.png)

tugas kalian adalah, latihan menggunakan git remote, bukan git clone hahaha _ketawa jahat_. tapi buat repository baru ya.... apapun isinya terserah kalian dan namanya bebas, tidak perlu di tambah _github.io_ di belakangnya. thank you!! keep learning

## Git Remote

Sudah mencoba mengerjakan tugas sebelumnya namun stuck ? baca ini dulu hehe
