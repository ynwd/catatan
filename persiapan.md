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

[vscode]: https://code.visualstudio.com/assets/home/home-screenshot-mac-lg.png
