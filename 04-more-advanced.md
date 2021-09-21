## 1. What is the difference between git reset and git revert. When would you use one over the other?
   -Perintah Git reset, akan mengembalikan file ke kondisi sebelumnya, kemudian menghapus catatan history commit beikutnya.
   <br> -Git Revert artinya mengembalikan. Perintah ini lebih aman daripada git reset, karena tidak akan menghapus history commit sampai yang terakhir. Revert akan akan mengambil kondisi file yang ada di masa lalu atau membatalkan perubahan yang ada, kemudian menggabungkannya dengan commit terakhir.
   <br> 
   <br> kapan menggunakannya ?
   <br> -Git Revert biasa dilakukan saat commit sudah di-push secara remote
   <br> -Git Reset biasa dilakukan di lokal saat commit belum di-push
## 2. What is the difference between git merge and git rebase. When would you use one over the other?
   -git merge adalah penggabungan mengambil konten dari cabang sumber dan menggabungkannya dengan cabang target. Dalam proses ini, hanya cabang target yang diubah. history cabang sumber tetap tidak berubah. git merge mengintegrasikan perubahan dalam pengembangan ke cabang fitur dan membuat komit baru.
   <br> -git rebase adalah cara lain untuk melakukan perubahan dari satu cabang ke cabang lainnya. Rebase mengkompres semua perubahan menjadi satu patch. Kemudian mengintegrasikan patch ke cabang target.
   <br>
   <br>
   kapan menggunakannya ?
   <br> Saat ada 2 orang yang melakukan commit terhadap satu hal akan terjadi konflik, hal ini dapat diselesaikan dengan 2 cara yaitu: Merge dan Rebase. Merge membentuk diamond shape dimana yang dimana mewarisi perubahan dari kedua commit tersebut, sedangkan Rebase mengintegrasikan perubahan dari garis paralel yang berbeda dari pengembangan (cabang) bersama dengan membuat komit gabungan.
## 3. What is the difference between git stash pop and git stash apply. When would you use one over the other?
   git stash pop membuang simpanan (paling atas, secara default) setelah menerapkannya, sedangkan git stash apply meninggalkannya di daftar simpanan untuk kemungkinan nanti digunakan kembali (atau Anda dapat git stash drop). Ini terjadi kecuali ada konflik setelah git stash pop, dalam hal ini tidak akan menghapus simpanan, membiarkannya berperilaku persis seperti git stash apply.
## 4. What kinds of things can you do in interactive mode when rebasing?
   Ada 2 mode dalam git rebase yaitu standard dan --interactive. Dimana pada interactive mode keuntungannya adalah mengubah individual commit pada process. tanpa harus memindahkan semua commit pada base yang baru. Dengan mode ini anda dapat membersihkan history dengan menghapus,mengedit dan mengubah sequence dari commit yang sudah ada.
 
