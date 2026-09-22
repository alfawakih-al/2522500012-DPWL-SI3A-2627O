# pertemuan-01

Soal.1 kesinambungan PWD–DPW–DPWL
jawaban:

-PWD (Dasar): Belajar pondasinya dulu—HTML, CSS, JS, PHP dasar, MySQL, sama validasi form.   
-DPW (Terstruktur): Naik kelas ke PHP yang lebih rapi—mulai pakai modularisasi, MySQLi, prepared statement, sistem login/sesi, dan CRUD.   
-DPWL (Arsitektur MVC): Menggabungkan semua ilmu tadi ke pola MVC biar kodenya makin terstruktur—lengkap dengan routing, integrasi database, pengujian, dan Git/GitHub.

Soal.2 perbedaan PHP terstruktur dan MVC
jawaban:

-PHP Terstruktur: Kodenya dicampur jadi satu di satu file—HTML, logic, sama query database nyatu semua. Gampang buat projek kecil, tapi makin lama makin berantakan.

-MVC: Kodenya dipisah-pisah. Model urus database, View urus tampilan HTML, Controller yang atur alurnya. Jauh lebih rapi dan gampang dirawat kalau projeknya makin gede.

soal.3 fungsi Model, View, dan Controller
jawaban:

-Model: Ngaruh ke data dan database. Tugasnya ngambil, nyimpan, sama ngolah data.

-View: Urusan tampilan. Tugasnya cuma nampilin data ke layar lewat HTML/CSS biar bisa dilihat user.

-Controller: Otaknya/penghubungnya. Tugasnya nerima permintaan dari user, minta data ke Model, terus ngirim hasilnya ke View.

soal.4 alur request–response MVC
jawaban:

1.User Request: User ngeklik tombol atau akses URL di browser.
2.Controller: Request pertama kali masuk ke Controller. Controller baca apa yang diminta user.
3.Model: Controller minta data yang dibutuhkan ke Model, lalu Model ngambil/ngolah data dari database.Controller: Model balikin data ke Controller.
4.View: Controller ngirim data tadi ke View buat disusun jadi tampilan HTML.
5.User Response: View yang udah berisi data dikirim balik ke browser user.

soal.5 pemetaan satu atau beberapa bagian/fitur aplikasi DPW ke Model, Controller, dan View disertai alasan
jawaban:

-Model (UserModel.php): Menangani validasi username dan password ke database users.

Alasan: Semua urusan query SQL, pemeriksaan data, dan koneksi database adalah tugas Model.

-Controller (AuthController.php): Menerima data form, memanggil fungsi di Model, lalu mengatur sesi (session) jika login berhasil.

Alasan: Controller bertindak sebagai logika utama yang mengatur alur proses dan keputusan aplikasi.

-View (login_view.php): Menampilkan formulir input username, password, tombol submit, dan pesan kesalahan (error).

Alasan: View hanya fokus pada struktur HTML dan tampilan visual untuk Pengguna (user).

soal.6 Kesimpulan P1
jawaban:

1.Gak Mulai dari Nol: Materi DPWL itu cuma kelanjutan dari PWD dan DPW. Ilmu HTML, CSS, PHP, dan MySQL yang udah dipelajari sebelumnya tetep dipakai, tapi sekarang ditata ulang biar lebih rapi.

2.Pindah ke Pola MVC: Kita belajar buat enggak numpuk semua kodingan dalam satu file lagi. Kodingan dipecah jadi tiga bagian: Model (data/database), View (tampilan/HTML), dan Controller (penghubung/logika).

3.Pentingnya Git & GitHub: Kerja praktik di mata kuliah ini langsung pakai alat standar industri. Kita pakai Git lewat VS Code buat simpan riwayat kodingan dan nge-push tugas ke GitHub biar rapi dan gampang dikelola.