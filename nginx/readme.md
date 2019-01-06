# Nginx Webserver

Nginx adalah aplikasi yang berguna sebagai server HTTP.

- [Cara Install Nginx](#cara-install-nginx)
- [Cara Menjalankan Nginx](#cara-menjalankan-nginx)
- [Konfigurasi Nginx](#konfigurasi-nginx)

## Cara Install Nginx

Dengan asumsi sudah [install ubuntu linux](linux/readme.md), berikut adalah cara installnya:

```terminal
$ sudo apt install nginx
```

## Cara Menjalankan Nginx

Untuk menjalankan nginx:
```terminal
$ sudo nginx
```

Buka browser dengan url http://localhost. Hasilnya:

![nginx](welcome.png)

Untuk menghentkan nginx:
```terminal
$ sudo nginx -s quit
```

