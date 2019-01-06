# Persiapan

Untuk memperkecil perbedaan lingkungan kerja dan menghemat waktu, disarankan untuk menggunakan sistem operasi [Ubuntu](https://tutorials.ubuntu.com/tutorial/tutorial-install-ubuntu-desktop). Semua intruksi instalasi command line panduan ini seharusnya berjalan dengan baik di atasnya.

## Install Nodejs

![nodejs][nodejs]

```terminal
$ curl -sL https://deb.nodesource.com/setup_10.x -o nodesource_setup.sh
$ sudo bash nodesource_setup.sh 
$ sudo apt-get install -y nodejs
```
Cek hasil instalasi dengan perintah berikut.
```terminal
$ node --version
v10.14.2
```

```terminal
$ npm --version
6.4.1
```
Untuk sistem operasi lain, silahkan cek intruksinya di sini:
[https://nodejs.org/en/download/package-manager/](https://nodejs.org/en/download/package-manager/)

[nodejs]: https://nodejs.org/static/images/logos/nodejs-new-pantone-black.png
