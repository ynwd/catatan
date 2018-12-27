# Cara menggunakan linux

Alasan menggunakan linux, dalam hal ini ubuntu, adalah gratis. Kamu secara hukum, boleh meng-install tanpa dikenakan biaya apapun. Ini tentu saja berbeda dengan Microsoft Windows yang kamu harus membeli lisensinya agar secara hukum legal menggunakannya. Ubuntu juga sudah menyediakan driver-driver perangkat keras standar (seperti USB dan Wifi) sehingga kamu tidak perlu mencarinya.

- [Instalasi Ubuntu](#instalasi-ubuntu)
- [Cara penggunaan terminal](#cara-penggunaan-terminal)

## Instalasi Ubuntu

Berikut ini adalah tautan terkait bagaimana cara meng-install ubuntu. Ikuti saja langkah demi langkah.

[![ubuntu]()](https://tutorials.ubuntu.com/tutorial/tutorial-install-ubuntu-desktop)


## Cara Menggunakan Terminal

Berikut ini adalah perintah-perintah dasar yang biasa dipergunakan untuk keperluan sehari-hari.

### sudo

`sudo` Kependekan dari `SuperUserDo`. Digunakan untuk perintah yang memerlukan *`root's permission`*.  
`root` adalah user yang punya hak akses paling dalam sistem operasi ubuntu. Aktivitas install software adalah contoh perintah yang memerlukan `sudo`.

Contoh kasus: `apt-get`. Coba ketik perintah ini:

```terminal
$ apt-get install vim
```

Keterangan:  
- `apt-get` : advanced packaging tool, adalah command untuk manajemen perangkat lunak di ubuntu.
- `install` : adalah argumen untuk meng-install perangkat.
- `vim`     : adalah nama perangkat yang akan di-install