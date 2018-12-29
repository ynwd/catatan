# Cara Menggunakan Git

Git adalah contoh *distributed version control system (DVCS)* yang digunakan developer untuk saling kerja sama. Dengan git kamu bisa meninjau sejarah sebuah proyek untuk mendapatkan informasi seperti:

- Apa saja yang telah berubah?
- Siapa yang telah mengubah?
- Kapan perubahan itu terjadi?
- Mengapa perubahan itu dibutuhkan?

Dan dengan sistem yang terdistribusi ini, kamu tidak perlu koneksi konstan ke repositori sentral. Kamu juga bisa bekerja di mana saja dan kapan saja secara asinkron. 

> **Catatan:**  
> Repositori adalah sebuah proyek yang berisi sejumlah file dan folder.  
> Asinkron artinya bisa dikerjakan tanpa menunggu proses lain selesai.

Berikut ini adalah panduan singkat mengenai cara penggunaan git:

- [Cara Install git](#cara-install-git)
- [Perintah dasar git](#perintah-dasar-git)
- [Contoh penggunaan git](#contoh-penggunaan-git)

## Cara install git

```terminal
$ sudo apt install git -y
```

## Perintah dasar git

| Perintah   | Digunakan untuk   |
|------------|-------------------|
|`git init`  | inisialisasi proyek. membuat hidden subfolder bernama `.git` <br>berisi struktur data yg diperlukan *version control* |
|`git clone` | membuat salinan lokal proyek yang sudah dibuat secara remote. |
|`git add`   | menambahkan file ke tahap staging (persiapan sebelum langkah berikutnya). |
|`git commit`| menyimpan snapshot (perubahan terakhir yg sudah ter-staging) ke dalam history.|
|`git status`| menampilkan status perubahan: untracked, modified, atau staged.|
|`git branch`| menampilkan branches (cabang-cabang) yang sedang dikerjakan secara lokal.|
|`git merge` | menggabungkan dua branch yang berbeda jadi satu. |
|`git pull`  | memperbarui repositori lokal dengan versi remote paling baru. |
|`git push`  | memperbarui repositori remote dengan versi lokal paling baru. |

Daftar perintah lain bisa kamu akses di sini: [https://git-scm.com/docs](https://git-scm.com/docs)