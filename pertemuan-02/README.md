# pertemuan-02

## 4. Routing dan Pemetaan URL
| URL/Route | Controller | Method | Parameter | View |
|---|---|---|---|---|
| / | Home | index | - | home/index.php |
| home/index | Home | index | - | home/index.php |
| home/info/mvc | Home | info | mvc | home/info.php |
| info/routing | Home | info | routing | home/info.php |
| mahasiswa/(:num) | Home | mahasiswa | $1 | home/mahasiswa.php |

**Penjelasan Pemetaan Rute Modifikasi ATM:**
- **Route (`mahasiswa/(:num)`):** Menangkap permintaan URL yang diawali kata `mahasiswa/` dan diikuti oleh angka variabel `(:num)` (misalnya NIM `2522500012`).
- **Controller (`Home`):** Menunjuk ke kelas `Home` pada berkas `application/controllers/Home.php`.
- **Method (`mahasiswa`):** Mengeksekusi fungsi/method `mahasiswa()` di dalam Controller `Home`.
- **Parameter (`$1`):** Nilai angka NIM dari URL ditangkap oleh wildcard `(:num)` dan dikirim sebagai argumen ke method `mahasiswa($nim)`.
- **View (`home/mahasiswa.php`):** Controller mengolah data profil (NIM: 2522500012, Nama: Fariq Akbar Al Fawakih, Kelas: SI3A) lalu memuat tampilan akhir pada file View `home/mahasiswa.php`.