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
## Konfigurasi Nginx

Buka file `/etc/nginx/sites-available/default`. Hapus semua konten. Lalu paste dan simpan konfigurasi berikut:
```nginx
server {
    root /var/www/html;
    index index.html;

    location / {
        try_files $uri $uri/ =404;
    }
}
```
Lokasi folder `root` ada di `/var/www/html`. Masuk ke dalamnya, buat file `index.html`

```terminal
$ cd /var/www/html
$ sudo vim index.html
```

Paste dan save kode html berikut:

```html
<html>
  <h2>Hello World</h2>
</html>
```

Buka `http://localhost` di browser. Hasilnya seperti ini:



