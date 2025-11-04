## Profil
|  |  |
| -------- | --- |
| *Nama* |Ananda Rahmadani |
| *Nim* |312310461 |
| *Kelas* | TI.23.A.5 |
| *Mata Kuliah* | Pemograman-Visual-Desktop |

# ☕ KOPI JAYA MANDIRI

Aplikasi manajemen internal berbasis web yang digunakan untuk mengatur data sistem, menu, dan pengguna di lingkungan PT. KOPI JAYA MANDIRI.  
Aplikasi ini dikembangkan menggunakan IIS sebagai web server, dengan dukungan database SQL Server dan MongoDB.

---

## ⚙️ Teknologi yang Digunakan

- **IIS (Internet Information Services)** – sebagai web server untuk menjalankan aplikasi.
- **ASP.NET / Node.js** – digunakan sebagai backend untuk mengatur logika bisnis dan komunikasi dengan database.
- **SQL Server Management Studio (SSMS)** – sebagai database utama untuk menyimpan data menu, pengguna, dan konfigurasi sistem.
- **MongoDB** – digunakan untuk menyimpan data non-relasional seperti log aktivitas atau konfigurasi tambahan.

---

## 🧭 Fitur Utama

- **Dashboard**  
  Menampilkan ringkasan data dan status sistem secara real-time.

- **Sistem Manager**  
  Mengatur modul aplikasi, pengguna, dan hak akses sistem.

- **Master Data**  
  Mengelola data utama seperti produk, pelanggan, atau data pendukung lainnya.

- **Administration Tools**  
  Berisi beberapa submenu penting seperti:
  - **Configuration** – Pengaturan sistem dan parameter global.
  - **Standard Messages** – Menyimpan pesan atau notifikasi bawaan aplikasi.
  - **App Management** – Mengatur komponen aplikasi, termasuk:
    - **Menu Management** → Mengelola daftar menu yang muncul di sidebar aplikasi.
    - **User Identity** → Mengelola data pengguna dan peran (role).
  - **Database Utility** – Mengelola koneksi dan struktur database.
  - **Utilities** – Alat tambahan untuk pengembang.

- **Developer Area**  
  Area khusus untuk pengujian dan pengembangan fitur baru.

---

## 🧩 Menu Management

### Menu List
Menampilkan daftar menu yang sudah terdaftar dalam sistem.  
Setiap menu memiliki beberapa informasi penting seperti ID, nama menu, parent menu (jika submenu), urutan tampil, dan status aktif.

### Menu Editor
Digunakan untuk menambah atau mengedit menu.  
Field yang dapat diisi antara lain:
- **Menu Id** → kode unik untuk setiap menu.  
- **Name** → nama menu yang tampil di sidebar.  
- **Parent** → menu induk (jika menu ini merupakan submenu).  
- **Level** → tingkat menu (0 = utama, 1 = submenu).  
- **Sequence** → urutan tampil menu di sidebar.  
- **Link** → alamat halaman tujuan menu.  
- **Icon** → ikon menu menggunakan FontAwesome.  
- **Tag1 / Tag2** → digunakan untuk memberi warna atau kategori.  
- **Status** → menentukan apakah menu aktif atau tidak.

---

## 🚀 Cara Menjalankan Aplikasi

1. Pastikan **IIS**, **SQL Server**, dan **MongoDB** sudah terpasang dan aktif.
2. Buka **IIS Manager**, tambahkan site baru dengan path ke folder proyek.
3. Atur koneksi database di file konfigurasi (`web.config` atau `appsettings.json`).
4. Import database SQL yang sudah disediakan (`.sql` atau `.bak` file).
5. Jalankan aplikasi melalui browser, misalnya:  
   `http://localhost/kopijayamandiri`
6. Login menggunakan akun administrator default (jika tersedia).

---

## 📦 Database

- **SQL Server** digunakan untuk menyimpan data utama seperti menu, pengguna, hak akses, dan transaksi.
- **MongoDB** digunakan untuk data non-relasional seperti log aktivitas, cache, atau konfigurasi tambahan sistem.

---

---

## 📝 Catatan

Jika tampilan menu tidak muncul setelah menambah data baru, pastikan:
- Menu memiliki status aktif (enabled).  
- Field **Parent** dan **Sequence** telah diatur dengan benar.  
- Cache aplikasi di-refresh (bisa melalui IIS atau reload browser).

---


## 🧾 Kesimpulan

Aplikasi **KOPI JAYA MANDIRI** dirancang sebagai sistem manajemen internal yang membantu pengelolaan data perusahaan secara terstruktur dan efisien.  
Dengan memanfaatkan **IIS** sebagai web server, **SQL Server** sebagai basis data utama, serta **MongoDB** sebagai pendukung penyimpanan data non-relasional, aplikasi ini mampu memberikan performa yang stabil, fleksibel, dan mudah dikembangkan.

Fitur-fitur seperti **Menu Management**, **User Identity**, dan **Master Data** memungkinkan administrator untuk mengatur tampilan dan akses sistem secara dinamis tanpa perlu mengubah kode program secara langsung.  
Kombinasi ini menjadikan aplikasi lebih adaptif terhadap perubahan kebutuhan organisasi.

---

## 🔚 Penutup

Pembuatan aplikasi **KOPI JAYA MANDIRI** merupakan langkah penting dalam penerapan sistem informasi berbasis web yang profesional dan modern.  
Diharapkan proyek ini dapat menjadi dasar untuk pengembangan sistem yang lebih besar di masa depan, serta memberikan manfaat nyata bagi efisiensi kerja dan pengelolaan data perusahaan.

Terima kasih kepada semua pihak yang telah berkontribusi dalam proses pengembangan dan pengujian aplikasi ini.  
Semoga dokumentasi ini dapat membantu dalam memahami struktur, fitur, serta cara kerja sistem secara keseluruhan.

---

## MOCK UP :
<img width="2927" height="1342" alt="login" src="https://github.com/user-attachments/assets/42d817d6-cdf3-46c0-8092-5cc3e28ae782" />
<img width="10749" height="2931" alt="Dasboard" src="https://github.com/user-attachments/assets/2c938c13-5244-455e-a106-c0e22af725d3" />
<img width="7001" height="3513" alt="AspNet Identity_User Identity " src="https://github.com/user-attachments/assets/4241fc54-5104-4bb1-9b6c-8cb1d0fbea7f" />
<img width="7001" height="2969" alt="AspNet Identity_User Identity 2" src="https://github.com/user-attachments/assets/ba9134ad-7af6-42e4-993f-eaa9c997e093" />
<img width="7001" height="2969" alt="AspNet Identity_User Identity 2" src="https://github.com/user-attachments/assets/ef7236df-2a43-4b4b-8dcd-6a00e4952d8c" />
<img width="7040" height="2899" alt="Setup_User Management" src="https://github.com/user-attachments/assets/76c11322-608f-410e-8f71-ae95dfa6d4e7" />

## LINK YT : https://youtu.be/xHaXIsf5Ih0?si=-pyBJzEpnt6xVl8G 

## 👩‍💻 Developer

**Ananda Rahmadani**  
© 2025 PT. KOPI JAYA MANDIRI  
