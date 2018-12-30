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

## Contoh penggunaan git

*create a new directory, and initialize it with git-specific functions*
```terminal
$ git init my-repo
```
*change into the `my-repo` directory*
```terminal
$ cd my-repo
```
*create the first file in the project*
```terminal
$ touch README.md
```
*git isn't aware of the file, stage it*
```terminal
$ git add README.md
```
*take a snapshot of the staging area*
```terminal
$ git commit -m "add README to initial commit"
```
*provide the path for the repository you created on github*
```terminal
$ git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
```
*push changes to github*
```terminal
$ git push --set-upstream origin master
```

## Selanjutnya
- Penjelasan lebih detail dan contoh penggunaan git yg lain bisa kamu temukan di sini: [git-handbook](https://guides.github.com/introduction/git-handbook/#github)
- Versi video bisa kamu ikuti di sini: [Git and GitHub with Briana Swift](https://www.youtube.com/watch?v=47E-jcuQz5c&index=1&list=PLg7s6cbtAD17Gw5u8644bgKhgRLiJXdX4).
