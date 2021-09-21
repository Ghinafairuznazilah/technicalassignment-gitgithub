## 1. What does git clean do?
   git clean is a convenience method for deleting untracked files in a repo's working directory. Untracked files are those that are in the repo's directory but have not yet been added to the repo's index with git add .
   git clean adalah perintah undo, yang melengkapi perintah lain seperti git reset dan git checkout. Namun, tidak seperti perintah lain yang beroperasi pada file yang sudah ditambahkan ke indeks pelacakan Git, perintah git clean berjalan pada file yang tidak terlacak.
## 2. What do the -d and -f flags for git clean do?
   -d digunakan untuk menghapus untracked directory, sedangkan -f flags memulai penghapusan secara paksa sebenarnya dari file yang tidak terlacak dari direktori saat ini. Secara default git clean -f akan beroperasi pada semua direktori saat ini file yang tidak terlacak.
## 3. What git command creates a branch?
   by using command :
   git branch [branch-name]
## 4. What is the difference between a fast-forward and recursive merge?
   -Fast-forward penggabungan paling umum digunakan hanya pada satu garis lurus. Saat membuat cabang dan membuat beberapa commit siap untuk menggabungkan, tidak ada penggabungan baru di master. 
   -Rekursif Dalam penggabungan Rekursif, setelah bercabang dan membuat beberapa komit, ada beberapa komit yang baru di branch'master'. Jadi, ketika digabungkan git berulang di atas cabang dan membuat komit gabungan baru. Komit gabungan memiliki 2 parents
## 5. What git command changes to another branch?
   git checkout [branch-name]
## 6. How do you remove modified or deleted files from the working directory?
   by using command :
   git add -u
## 7. What git command deletes a branch?
   by using command :
   git branch -d 
   atau jika pada remote by using command :
   git push [remote] --delete [branch]
## 8. What does the git diff command do?
   git diff secara default menampilkan yang tidak di commit ke repository, dengan git diff kita dapat melihat baris yang dihapus dari file sebelumnya serta baris apa pun yang ditambahkan atau diubah dalam file. Seringkali, Git diff digunakan untuk membandingkan cabang dalam repositori Git. 
## 9. How do you remove files from the staging area?
   by using command :
   git reset HEAD -- path/to/file atau git rm [file-name]
## 10.How do merge conflicts happen?
   biasanya terjadi saat 2 orang melakukan perubahan pada line yang sama di suatu file, atau saat seseorang melakukan delete file sementara orang yang lain sedang melakukan modifikasi terhadapnya sehingga akan terjadi konflik penggabungan.
