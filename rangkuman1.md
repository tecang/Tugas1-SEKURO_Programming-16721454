# Rangkuman Video 6

## Author
#### Nama: Eureka Theressa Chang
#### NIM  : 16721454

<br>

## Daftar Isi:
1. Cara Membuat & Mengakses Repository
2. Branches
3. Merge


## Cara Membuat & Mengakses Repository
Setelah mendownload Git dan menjalankan terminal Git Bash, sebuah folder local harus dibuat untuk dijadikan repository. Untuk mengakses repository, directory folder harus di-input atau bisa juga di-*drag* ke terminal.

```
$ cd /Documents/tesa/test_repos 
````
>![](https://i.ibb.co/QDhMXZK/Screenshot-154.png)

Kemudian, dianggap bahwa sudah ada file yang terdapat di dalam folder tersebut. File dinamakan `test_repos`. File ini berbentuk html.
<br>
File ini baru saja dibuat sehingga Git mengenali bahwa ada perubahan pada content folder. Dapat dicek menggunakan `$ git status`. Untuk menambahkan file tersebut ke repository, dapat menggunakan cmnd `$ git add .` atau `git add new_file` dilanjutkan dengan `$ git commit -m <pesan>`. Sekarang, setelah dicek, status akan menunjukkan *branch Master nothing to commit, working tree clean*.

>![](https://i.ibb.co/X3Xx1Mp/Screenshot-155.png)

Setelah itu, jika ada perubahan yang terjadi pada `new_file.html`, maka akan terdeteksi oleh Git. Dapat dilakukan cmnd sebagai yang tertera digambar agar perubahan tersimpan.

>![](https://i.ibb.co/W3xNgYv/Screenshot-156.png)

Semua ini tercatat pada log yang dapat dilihat sebagai berikut.
>![](https://i.ibb.co/kK4gzdv/Screenshot-157.png)

<br>

## Branches
Branch dipakai untuk melakukan perubahan terhadap suatu folder ataupun file yang belum final, dan untuk menambahkan atau melihat log branch, dapat dilakukan sebagai berikut. Untuk pindah branch, dapat dilakukan sebagai berikut. Saya membuat cmnd `logging` untuk mempermudah pendataan log.
>![](https://i.ibb.co/8bV5ZPG/Screenshot-158.png)

Saat dipindahkan ke branch `tesa2`, maka folder akan menampilkan file-file yang ada di branch itu, baik yang ekslusif maupun inklusif semua branch. 
>![](https://i.ibb.co/31nGT0B/Screenshot-159.png)

Saat ditambahkan file baru, maka akan terbentuk branch baru yang dapat dilihat sebagai berikut.
>![](https://i.ibb.co/tY4dv0g/Screenshot-161.png)

Saat ditambahkan file baru ke `tesa3` hasilnya adalah sebagai berikut. Dapat dilihat ada 2 branch yang telah terbuat.
>![](https://i.ibb.co/Kh7HqvW/Screenshot-163.png)

<br>

## Merge
### 1. Fast-Forward Merge

Dilakukan ketika branch yang ingin di-*merge* memiliki *path* langsung ke `master`. Untuk melakukan merge, *head* harus berada pada master. Setelah di-*merge*, branch selain master dapat dihapus. Disini `tesa2` dihapus.
>![](https://i.ibb.co/7tqZCk5/Screenshot-164.png)

### 2. Three-way Merge

Dilakukan ketika branch yang ingin di-*merge* tidak memiliki *path* langsung ke `master`. Untuk melakukan merge, *head* harus berada pada master. Untuk meng-*authorize* merge, dapat dilakukan dengan cmnd `(esc):wq!`. Setelah di-*merge*, branch selain master dapat dihapus. Disini `tesa3` dihapus.
>![](https://i.ibb.co/682nJmf/Screenshot-165.png)

Dapat dilihat sekarang semuanya telah dimerge.