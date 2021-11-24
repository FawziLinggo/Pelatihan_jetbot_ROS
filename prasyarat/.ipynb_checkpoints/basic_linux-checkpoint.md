# Perintah Linux Dasar
Ketika mengoperasikan OS Linux, Kita harus menggunakan shell, yaitu interface yang menyediakan akses ke layanan sistem operasi. Sebagian besar distribusi Linux menggunakan antarmuka pengguna grafis (graphic user interface – GUI) sebagai shell-nya, terutama untuk memberikan kemudahan penggunaan bagi para user. 

Dengan demikian, penggunaan command-line interface (CLI) sangat disarankan karena lebih powerful dan efektif. Task atau tugas yang membutuhkan proses dengan banyak langkah melalui GUI dapat dilakukan hanya dalam waktu sekian detik dengan mengetikkan command atau perintah ke CLI.

Sebelum menjabarkan perintah dasar sistem operasi Linux, kita harus membuka baris perintah `(command line)` terlebih dulu. 
### **1. pwd command**
Perintah dasar Linux pwd berfungsi untuk mencari `path` dari direktori (folder) yang Anda gunakan saat ini. Perintah ini akan mengembalikan `path` yang absolut (penuh), yang pada dasarnya merupakan path semua direktori yang diawali dengan garis miring depan `(/)`. Contoh dari path absolut adalah `/home/username`.

### **2 cd command**
Untuk menjelajahi file dan direktori Linux, gunakan perintah cd. Perintah Linux ini memerlukan path penuh atau nama direktori, tergantung pada direktori yang Anda gunakan saat ini.

Misalkan saat ini Anda sedang berada di `/home/username/Documents` dan ingin membuka Photos, subdirektori dari Documents. Untuk melakukannya, Anda hanya perlu mengetikkan command ini: cd Photos.

Contoh lainnya, ketika Anda ingin beralih ke direktori yang sepenuhnya baru, misalnya, `/home/username/Movies`. Dalam contoh ini, ketik cd yang diikuti dengan path absolut direktori: cd `/home/username/Movies`.

Berikut beberapa jalan pintas (shortcut) untuk memudahkan navigasi:

 cd .. (dengan dua tanda titik) untuk memindahkan satu direktori ke atas.

 >cd jika ingin langsung membuka folder home.

 >cd- (dengan tanda penghubung) untuk berpindah ke direktori sebelumnya.

 Satu hal yang perlu diperhatikan, shell Linux sangat sensitif. Jadi, Anda harus mengetikkan nama direktori dengan benar dan tepat.

 ### **3 ls command**
 ls merupakan perintah dasar pada Linux yang digunakan untuk melihat konten atau isi direktori. Secara default, command ini akan menampilkan isi dari direktori yang Anda gunakan saat ini.

 Jika ingin melihat isi direktori lain, ketik Is, disusul dengan path direktori. Contoh, ketik Is `/home/username/Documents` untuk melihat isi Documents.

 Berikut beberapa variasi yang bisa dikombinasikan dengan perintah dasar Linux Is:

 >ls -R akan membuat daftar semua file yang ada di sub-direktori.

 >ls -a akan menampilkan file yang tersembunyi.

 >ls -al akan membuat daftar file dan direktori yang memuat informasi mendetail, seperti permission (hak akses), ukuran (size), pemilik (owner), dll.

 ### **4. cat command**
 cat (akronim dri concatenate) adalah salah satu perintah dasar sistem operasi Linux yang sering digunakan. Perintah ini berfungsi untuk membuat daftar konten atau isi file pada standard output (sdout). Untuk menjalankan command ini, ketik cat yang kemudian diikuti dengan nama dan ekstensi file. Sebagai contoh: cat file.txt.

 Berikut beberapa cara untuk menggunakan perintah cat:

 > cat > filename untuk membuat file baru.

 > cat filename1 filename2>filename3 untuk menggabungkan dua file (1 dan 2) dan menyimpan outputnya di file baru (3).

 > cat filename | tr a-z A-Z >output.txt untuk mengonversi file ke penggunaan huruf besar atau huruf kecil.

 ### **5. mkdir command**
 Untuk membuat direktori baru, Anda bisa menggunakan perintah dasar Linux mkdir. Sebagai contoh, jika Anda mengetik mkdir Music, direktori baru yang muncul disebut Music.
>
 Berikut beberapa command mkdir tambahan:

 > Untuk membuat direktori baru di dalam direktori lain, gunakan command dasar Linux mkdir Music/Newfile.

 > Gunakan opsi p (parents) untuk membuat direktori di antara dua direktori yang sudah ada. Misalnya, mkdir -p Music/2020/Newfile untuk membuat file baru “2020”.

 ### **6. rmdir command**
 Jika ingin menghapus direktori, gunakan perintah rmdir. Namun, rmdir hanya boleh digunakan untuk menghapus direktori kosong.

 ### **7. rm command**
 rm adalah perintah dasar pada Linux yang berfungsi untuk menghapus direktori beserta isinya. Jika hanya ingin menghapus direktorinya saja – alternatif command selain rmdir – gunakan rm -r.

 > Catatan: Saat menggunakan command ini, Anda harus berhati-hati dan cek kembali direktori di mana Anda berada saat ini. Sekali command rm dijalankan, maka semuanya akan terhapus dan tidak bisa dikembalikan.

 ### **8. touch command**
 touch adalah perintah dasar Linux yang memperbolehkan Anda membuat file baru yang kosong melalui baris perintah Linux. Sebagai contoh, ketik touch `/home/username/Documents/Web.html` untuk membuat file HTML berjudul Web di bawah direktori Documents.

 ### **9. grep command**
 Perintah dasar Linux lain yang sangat berguna untuk menyelesaikan task harian adalah grep. Dengan command ini, Anda bisa melakukan pencarian di semua teks di dalam file yang diberikan.

 Sebagai contoh, ketik grep blue notepad.txt untuk mencari kata blue di file notepad. Baris yang memuat kata yang dicari akan ditampilkan sepenuhnya.

 ### **10. sudo command**
 sudo merupakan singkatan dari `“SuperUser Do”` dan berfungsi untuk menjalankan task yang memerlukan hak akses (permission) administrative atau root. Namun, kami tidak menyarankan penggunaan command sudo untuk task harian karena bisa terjadi error kapan saja bila Anda melakukan kesalahan.

 ### **11. diff command** 
 diff adalah perintah dasar Linux yang membandingkan konten atau isi dua file berdasarkan baris demi baris. Setelah menganalisis file, perintah ini akan menghasilkan output berupa line atau baris yang tidak cocok. Programmer sering menggunakan command ini ketika mereka perlu membuat perubahan program, alih-alih menulis kembali semua kode source.

 Format paling sederhana dari command dasar Linux ini adalah diff file1.ext file2.ext.

 ### **12. chmod command**
 chmod adalah perintah dasar Linux lainnya yang digunakan untuk membaca, menulis, dan menjalankan permission (hak akses) file dan direktori. Karena perintah ini cukup sulit, maka untuk menjalankannya

 ### **13. ping command**

 Command ping berfungsi untuk mengecek status konektivitas ke server. Misalnya, dengan menambahkan `ping google.com`, command akan mengecek apakah Anda sudah terhubung ke Google atau belum dan juga mengukur waktu respons.

 ### **14. wget command**
 Perintah dasar Linux ini sangat berguna – Anda bahkan bisa mengunduh file dari internet dengan bantuan command wget. Anda hanya perlu mengetikkan wget yang diikuti dengan link unduhan.

 ### **15. history command**
 Kalau sudah lihai menggunakan Linux, Anda bisa menjalankan ratusan command atau perintah setiap hari. Misalnya, penggunaan command history untuk mengecek kembali (review) command yang sudah ditambahkan sebelumnya.

 ### **16. echo command**
 Perintah dasar Linux ini digunakan untuk memindahkan beberapa data ke dalam satu file. Misalnya, jika ingin menambahkan teks, “Hello, my name is John” ke file yang bernama name.txt, yang perlu diketik adalah `echo Hello, my name is John >> name.txt`.

 ### **17. zip, unzip command**
 Gunakan perintah zip untuk meng-compress file ke arsip zip dan perintah unzip untuk mengekstrak file zip ke arsip zip.

 ## **Tips dan Trik**
 unakan command `clear` untuk membersihkan terminal jika di dalamnya sudah terdapat banyak sekali command.

 Coba tombol `TAB` untuk mengisi secara otomatis (autofill) apa yang sedang Anda ketikkan. Sebagai contoh, jika ingin mengetik `Documents`, mulailah dengan menambahkan command terlebih dulu (misalnya `cd Docu`, kemudian tekan tombol TAB) dan terminal akan melengkapinya. Hasilnya akan seperti ini: cd Documents.

 `Ctrl+C` dan `Ctrl+Z` digunakan untuk memberhentikan command apa pun yang saat ini sedang dijalankan. `Ctrl+C` akan memberhentikan command dengan aman, sedangkan `CTRL+Z` akan memaksa command untuk berhenti.

 Bila Anda secara tidak sengaja `‘membekukan’` terminal dengan menekan `Ctrl+S`, untuk membatalkan `‘pembekuan’` tersebut cukup tekan Ctrl+Z.

 `Ctrl+A` membawa Anda ke awal baris, sedangkan `Ctrl+E` mengarahkan Anda ke akhir baris.

 Anda bisa menjalankan banyak command atau perintah di dalam satu command dengan menggunakan `“;”` untuk memisahkan command-command tersebut. Misalnya, `Command1; Command2; Command3`. Atau gunakan `&&` jika Anda hanya ingin menjalankan command selanjutnya setelah command pertama berhasil dijalankan.

 ## *Kesimpulan*
 Perintah dasar Linux membantu user atau penggunanya untuk menjalankan task dengan mudah dan efektif. Memang bukan hal yang mudah untuk mengingat semua perintah Linux di atas. Namun, semuanya akan teratasi bila Anda terus berlatih dan berlatih.


