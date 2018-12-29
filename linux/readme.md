# Cara Menggunakan Linux

![ubuntu](https://assets.ubuntu.com/v1/79439f53-Dell_XPS_Laptop_Front-Developer.png?w=600)

Panduan ini berisi cara praktis menggunakan linux untuk keperluan standar *programming*. Distro yang akan kamu gunakan adalah [ubuntu](https://www.ubuntu.com/desktop/developers). 

- [Alasan Menggunakan Ubuntu](#alasan-menggunakan-linux)
- [Cara Install Ubuntu](#instalasi-ubuntu)
- [Cara Menggunakan Terminal](#cara-menggunakan-terminal)
  - [mkdir](#mkdir) (make directory)
  - [cd](#cd) (change directory)
  - [pwd](#pwd) (show active location)
  - [ls](#ls) (list)
  - [sudo](#sudo) (super user do)
  - [apt](#apt) (advanced package tool)
  - [vim](#vim) (vi improved)
  - [cat](#cat) (concatenate)
  - [cp](#cp) (copy)
  - [rm](#rm) (remove)
- [Cara Menggunakan Vim](#cara-menggunakan-vim)

# Alasan Menggunakan Ubuntu

![stats](https://assets.ubuntu.com/v1/a9948f53-desktop_graph.png)  
*Source: Eclipse Community survey, 2014, Stackoverflow annual survey 2016*

Alasan utama memilih [ubuntu](https://pages.ubuntu.com/rs/066-EOV-335/images/Desktop_Developers_WP_Canonical_Final.pdf), adalah `freedom`. Kamu diperbolehkan men-*download* dan meng-*install*-nya tanpa membayar apapun. Ubuntu juga sudah menyediakan driver hardware standar (seperti USB, LAN, Wifi) dan driver untuk menjalankan file audio dan video (seperti MP3 dan AVI).

# Instalasi Ubuntu

> **Prasyarat**:  
> • Laptop tersambung dengan listrik  
> • Minimal punya space 5GB di hardisk   
> • Sudah memiliki Flash Disk yang berisi installer ubuntu. (Lihat: [cara membuat installer](https://tutorials.ubuntu.com/tutorial/tutorial-create-a-usb-stick-on-ubuntu))  
> • Backup semua data sebelum instalasi untuk jaga-jaga jika nanti ada kesalahan tidak disengaja   

Pada gambar di bawah ini terdapat tautan yang berisi bagaimana cara meng-install ubuntu. Klik dan ikuti saja langkah demi langkah.

[![ubuntu](https://tutorials.ubuntu.com/es6-bundled/src/codelabs/tutorial-install-ubuntu-desktop/img/747a83dc503cd86c.png)](https://tutorials.ubuntu.com/tutorial/tutorial-install-ubuntu-desktop)


# Cara Menggunakan Terminal

Di dalam Ubuntu versi desktop, sebenarnya sudah terdapat user-interface grafis untuk melakukan operasi-operasi standar, seperti install software, membuat dan men-delete folder & file, dsb. Tapi karena kamu ingin jadi developer, maka command-line di terminal, harus kamu ketahui. Akan ada banyak tools yang user-interface-nya memakainya. 

![ubuntu](ubuntu.png)

> **Catatan**:   
> Setiap command-line diawali dengan tanda `$` (dollar).  
> Barisan teks yang tidak diawali dengan `$` adalah hasil atau respon command-line.

Berikut ini adalah perintah-perintah dasar yang biasa dipergunakan untuk keperluan sehari-hari.

# mkdir  
```terminal
$ mkdir hello
```
`mkdir` dengan argumen `hello` di atas digunakan untuk membuat folder bernama `hello`.

# cd  
```terminal
$ cd hello
```
`cd` dengan argumen `hello` di atas digunakan untuk masuk ke folder bernama `hello`.

# pwd
```terminal
$ pwd
```  
Digunakan untuk mengetahui lokasi folder yang digunakan saat ini.
Hasilnya:
```terminal
/home/yanu/hello
```

# ls
```terminal
$ ls /apt
```
Digunakan untuk mengetahui isi sebuah folder. Pada contoh di atas, `ls` dipakai untuk mengetahui isi folder `/apt`.  
Hasilnya:
```terminal
apt.conf.d  preferences.d  sources.list  sources.list.d  trusted.gpg  trusted.gpg.d
```
# sudo 
```terminal
$ sudo
```
Kependekan dari `SuperUserDo`. Digunakan untuk perintah yang memerlukan *`root's permission`*.  

`root` adalah user yang punya hak akses paling tinggi dalam sistem operasi ubuntu. Install software adalah contoh perintah yang memerlukan `sudo`.

# apt
```terminal
$ apt
```
Berguna untuk menangani penambahan dan penghapusan perangkat lunak (package).

### Contoh penggunaan sudo dan apt: 
Misalnya kamu ingin coba membuat file bernama `hello.json` via terminal menggunakan file editor bernama `vim`. Tapi biasanya `vim` belum terpasang.

```terminal
$ vim hello.json
```
Hasilnya:
```terminal
bash: vim: command not found
```

Maka kamu harus install dulu vim tersebut memakai `apt`:

```terminal
$ apt install vim  
```
Hasilnya:
```terminal
E: Could not open lock file /var/lib/dpkg/lock - open (13: Permission denied)
E: Unable to lock the administration directory (/var/lib/dpkg/), are you root?
```

Sekarang tambahkan `sudo` sebelum command line:
```terminal
$ sudo apt install vim
```
Hasilnya:
```terminal
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following additional packages will be installed:
  libpython3.6 vim-common vim-runtime xxd
Suggested packages:
  ctags vim-doc vim-scripts
The following NEW packages will be installed:
  libpython3.6 vim vim-common vim-runtime xxd
0 upgraded, 5 newly installed, 0 to remove and 19 not upgraded.
Need to get 8123 kB of archives.
After this operation, 37.3 MB of additional disk space will be used.
Do you want to continue? [Y/n]
```

Enter `Y` untuk melanjutkan proses.   
Setelah instalasi selesai, ketik perintah ini untuk memastikan instalasi berhasil:

```terminal
$ vim -version
```
Hasilnya:
```terminal
VIM - Vi IMproved 8.0 (2016 Sep 12, compiled Apr 10 2018 21:31:58)
Garbage after option argument: "-version"
More info with: "vim -h"
```
# vim
### Cara menggunakan vim  
```terminal
$ vimtutor
  ```
Dengan asumsi kamu sudah [install vim](#contoh-penggunaan-sudo-dan-apt), ketik perintah di atas untuk step-by-step tutorial-nya.  

Jika sudah paham, buat file `hello.json`

  ```terminal
$ vim hello.json
```

Copy-paste dan save code berikut:
```json
{ 
  "text": "hello"
}
```

Quit.
# cat
```terminal
$ cat hello.json
```
`cat` dengan argumen `hello.json` digunakan untuk menampilkan isi `hello.json`.  

Jika perintah di atas kamu jalankan, hasilnya seperti ini:
```terminal
{ 
  "text": "hello"
}
```
# cp
```terminal
$ cp hello.json world.json
```
Digunakan untuk copy file `hello.json` ke file baru bernama `world.json`.  
Kalau kamu ketik:
  ```terminal
  $ ls
  ``` 
Maka hasilnya seperti ini:
```terminal
hello.json  world.json
```
Terlihat, ada dua file.
# rm
```terminal
$ rm world.json
  ```
`rm` dengan argumen `world.json` di atas dipergunakan untuk menghapus (remove) file `world.json`
