# Persiapan
Berikut ini adalah hal-hal yang harus kamu siapkan agar bisa mengikuti panduan ini dengan baik.

Untuk memperkecil perbedaan lingkungan kerja dan menghemat waktu, disarankan untuk menggunakan sistem operasi [Ubuntu](https://tutorials.ubuntu.com/tutorial/tutorial-install-ubuntu-desktop). Semua intruksi instalasi command line panduan ini seharusnya berjalan dengan baik di atasnya.


- [Install Nodejs](#install-nodejs)
- [Install VSCode](#install-vscode)
- [Install Git](#install-git)
- [Install Now](#install-now)
- [Buat Account di Github dan Zeit](#buat-account-di-github-dan-zeit)

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


## Install VSCode

Ada begitu banyak editor. Beberapa software gratis yang disukai beberapa developer misalnya [Vim](https://www.vim.org) dan [SublimeText](https://www.sublimetext.com/). Tapi, karena tampilan yang bagus, ringan, banyak plugins, dan free, maka saya memilih [VSCode](https://code.visualstudio.com/).

![vscode][vscode]

Berikut cara install-nya:

```terminal
$ curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > microsoft.gpg
$ sudo install -o root -g root -m 644 microsoft.gpg /etc/apt/trusted.gpg.d/
$ sudo sh -c 'echo "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main" > /etc/apt/sources.list.d/vscode.list'
```

```terminal
$ sudo apt-get install apt-transport-https
$ sudo apt-get update
$ sudo apt-get install code # or code-insiders
```

Intruksi lebih detail bisa diakses disini: [https://code.visualstudio.com/docs/setup/setup-overview](https://code.visualstudio.com/docs/setup/setup-overview).


## Install Git
   
Tool ini berguna untuk berbagi kode.
```terminal
$ apt install git
```

Cek hasil instalasi dengan perintah berikut.
```terminal
$ git --version
git version 2.17.1
```

## Install Now

Tool ini berguna untuk meng-upload aplikasi yang telah kita buat ke server [zeit](https://zeit.co/) agar bisa diakses di mana pun.

```terminal
$ npm install -g now
```

Cek hasil instalasi dengan perintah berikut.

```terminal
$ now --version
12.1.14
```

## Buat Account di Github dan Zeit

- Account Github nanti akan kamu pakai untuk sharing code & acuan deployment ke server.
- Isi dan proses intruksi halaman ini: [https://github.com/join](https://github.com/join)
- Account Zeit nanti akan kamu pakai untuk upload dan deploy ke server yang bisa diakses dari mana pun (worldwide).
- Isi dan proses intruksi halaman ini: [https://zeit.co/signup](https://zeit.co/signup)

## Selanjutnya
Jika semua sudah siap sudah, mari kita mulai ke langkah [selanjutnya](getting-started.md)

[nodejs]: https://nodejs.org/static/images/logos/nodejs-new-pantone-black.png
[vscode]: https://code.visualstudio.com/assets/home/home-screenshot-mac-lg.png
