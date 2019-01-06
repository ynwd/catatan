# Cara Menggunakan Git

Git adalah contoh *distributed version control system (DVCS)* yang digunakan developer untuk saling kerja sama. Dengan git kamu bisa meninjau sejarah sebuah proyek untuk mendapatkan informasi seperti:

- Apa saja yang telah berubah?
- Siapa yang telah mengubah?
- Kapan perubahan itu terjadi?
- Mengapa perubahan itu dibutuhkan?

Dan dengan sistem yang terdistribusi ini, kamu tidak harus terkoneksi ke repositori sentral. Kamu juga bisa bekerja di mana saja dan kapan saja secara asinkron. 

> **Catatan:**  
> Repositori adalah sebuah proyek yang berisi sejumlah file dan folder.  
> Asinkron artinya bisa dikerjakan tanpa menunggu proses lain selesai.

Berikut ini adalah panduan singkat mengenai cara penggunaan git:

- [Cara Install git](#cara-install-git)
- [Perintah dasar git](#perintah-dasar-git)
- [Contoh penggunaan git](#contoh-penggunaan-git)
## Cara install git
Dengan asumsi kamu sudah [install ubuntu](../linux/readme.md), berikut ini adalah cara install git:
```terminal
$ sudo apt install git -y
```

## Perintah dasar git
   
Berikut ini adalah perintah-perintah dasar yang akan sering kamu gunakan.

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

Daftar perintah lain bisa kamu akses di sini: [https://git-scm.com/docs](https://git-scm.com/docs).   

## Buat Account di Github
- Account Github nanti akan kamu pakai untuk sharing code & acuan deployment ke server.
- Isi dan proses intruksi halaman ini: [https://github.com/join](https://github.com/join)


## Contoh penggunaan git

Buat direktori dan inisialisasi proyek git.
```terminal
$ git init my-repo
```
Masuk ke dalam direktori.
```terminal
$ cd my-repo
```
Buat file di dalam repositori.
```terminal
$ touch README.md
```
Tambahkan file tsb ke area staging.
```terminal
$ git add README.md
```
Commit area staging.
```terminal
$ git commit -m "add README to initial commit"
```
Tambahkan url repositori yang telah kamu buat. Jika belum membuatnya, ikuti panduannya di sini: [Create a Repository](https://guides.github.com/activities/hello-world/#repository)
```terminal
$ git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
```
Push perubahan ke github.
```terminal
$ git push --set-upstream origin master
```

## Selanjutnya
- Penjelasan lebih detail dan contoh penggunaan git yg lain bisa kamu temukan di sini: [git-handbook](https://guides.github.com/introduction/git-handbook/#github)
- Versi video bisa kamu ikuti di sini: [Git and GitHub with Briana Swift](https://www.youtube.com/watch?v=47E-jcuQz5c&index=1&list=PLg7s6cbtAD17Gw5u8644bgKhgRLiJXdX4).
