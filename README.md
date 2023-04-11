# Tutorial menggunakan git untuk pemula

## Menambahkan file ke remote repository 
1. setup user dan email
    - git --global user.name <"username">
    - git --global user.email <"email">
2. melakukan inisiasi
    - git init : digunakan untuk membuat hidden file `.git` yang menyimpan semua perubahan dan sinkronisasi dengan github dkk
3. membuat file 
    - Buat sembarang file yang nantinya akan dimasukkan ke dalam github
    - Gunakan command `git status` untuk melihat semua file dan folder yang akan ada dalam git kita 
4. Memasukkan file ke dalam staging 
    - Gunakan command `git add .<nama file>` : akan menambahkan file ke dalam kelompok file yang akan dimasukkan ke dalam box (staging)
5. Memasukkan file kedalam local repository 
    - Gunakan command `git commit -m <commit message>` untuk membuat label dari box (staging)
    - Commit message sebaiknya ditulis dengan detail agar mudah dipahami apa yang sedang ditambahkan, karena ini akan menjadi cara untuk mengetahui version control dari file yang kita tambahkan 
    - Untuk mengecheck apakah kita sudah melakukan commit pada suatu box (kumpulan file pada staging) maka dapat dilakukan dengan command `git log`
6. Mengirim file yang dicommit ke remote repository 
    - Sebelum memindahkan file ke remote repository pastikan git sudah memiliki tujuan repository yang diinginkan 
    - Jika sudah memiliki tujuan repo maka gunakan command `git remote add origin <nama repo>` untuk melakukan setup remote connection 
    - Untuk memindahkan file ke remote repository gunakan command `git push -u origin master`
    
## Mendapatkan versi terbaru dari file yang ada di remote repository 
1. Untuk mendapatkan versi terbaru dari file bisa menggunakan command `git clone`
    - `git clone <alamat remote repository>`
    