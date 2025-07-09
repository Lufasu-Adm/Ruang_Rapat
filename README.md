# 📅 Sistem Peminjaman Ruang Rapat

Aplikasi ini merupakan sistem manajemen peminjaman ruang rapat berbasis web yang dikembangkan dengan Laravel. Sistem mendukung multi-role (User, Admin, dan Super Admin) serta terintegrasi dengan manajemen divisi dan data ruangan.

---

## 🚀 Fitur Utama

- ✅ **Autentikasi dan Role**
  - Role: `user`, `admin`, `super admin`
  - Setiap role memiliki tampilan dan hak akses berbeda

- ✅ **Manajemen Ruangan**
  - Tambah, edit, dan hapus ruangan (khusus admin dan super admin)
  - Setiap ruangan terhubung dengan satu divisi

- ✅ **Peminjaman Ruangan**
  - Formulir peminjaman dengan input waktu, tanggal, dan keperluan
  - Riwayat peminjaman per user

- ✅ **Dashboard Kustom**
  - Tampilan berbeda untuk user, admin, dan super admin
  - Jam analog dekoratif dan info hari/tanggal

- ✅ **Manajemen Divisi (Super Admin)**
  - Tambah divisi beserta admin dan user-nya secara otomatis

---

## 🏗️ Struktur Proyek

```
├── app/
│   └── Http/
│       └── Controllers/
│           ├── AuthController.php
│           ├── BookingController.php
│           ├── RoomController.php
│           └── SuperAdminController.php
├── resources/
│   ├── views/
│   │   ├── bookings/
│   │   ├── admin/
│   │   └── superadmin/
│   └── css/
│       ├── app.css
│       ├── admin.css
│       └── superadmin.css
├── database/
│   ├── migrations/
│   └── seeders/
```

---

## ⚙️ Cara Instalasi

1. Clone repository
   ```bash
   git clone https://github.com/Lufasu-Adm/Ruang_Rapat.git
   cd Ruang_Rapat
   ```

2. Install dependency Laravel dan frontend
   ```bash
   composer install
   npm install && npm run dev
   ```

3. Salin file konfigurasi `.env`
   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

4. Buat database dan sesuaikan `.env`

5. Jalankan migrasi dan seeder dummy
   ```bash
   php artisan migrate --seed
   ```

6. Jalankan server lokal
   ```bash
   php artisan serve
   ```

---

## 🧪 Akun Dummy (Seeder)

| Role         | Email                                  | Password  |
|--------------|----------------------------------------|-----------|
| Super Admin  | superadmin@example.com                 | password  |
| Admin Divisi | admin_divisi_akuntansi.example.com     | password  |
| User Divisi  | user_divisi_akuntansi.example.com      | password  |

---

## 🛠️ Teknologi

- Laravel 10
- Blade Template
- PHP 8+
- MySQL/PostgreSQL
- CSS murni (tanpa framework)
- Git & GitHub

---

## 👨‍💻 Tentang Pengembang

> Proyek ini dibuat oleh **Jordan dan Kelompok KP** untuk kebutuhan **Kerja Praktik di PT PAL Indonesia**  
> Tahun: **2025**  
> Tujuan: Efisiensi dan digitalisasi peminjaman ruang rapat antar-divisi.

---

## 📄 Lisensi

Repositori ini hanya untuk keperluan edukasi dan penggunaan internal PT PAL. Tidak untuk didistribusikan tanpa izin.
