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

## Selanjutnya
Jika semua sudah siap sudah, mari kita mulai ke langkah [selanjutnya](getting-started.md)

[vscode]: https://code.visualstudio.com/assets/home/home-screenshot-mac-lg.png
