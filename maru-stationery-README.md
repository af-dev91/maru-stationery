# Maru Stationery

Aplikasi web sistem penjualan ATK (alat tulis kantor) untuk toko **Maru Stationery**.

Dibuat dengan HTML, CSS, dan JavaScript murni dalam satu berkas (`index.html`), sehingga tidak membutuhkan instalasi, server, atau database.

**Dikembangkan oleh Azzam Al Fayyadh - SMA Neg. 2 Kendari**

## Fitur

**Pembeli**
- Daftar akun baru, lalu masuk
- Katalog produk dengan pencarian dan filter kategori
- Keranjang belanja (ubah jumlah, hapus item, batas sesuai stok)
- Checkout dengan data pengiriman dan metode pembayaran
- Riwayat dan status pesanan

**Admin toko**
- Dashboard: jumlah produk, total stok, pesanan, dan pendapatan
- Kelola produk: tambah, ubah, dan hapus
- Kelola pesanan: ubah status (Diproses, Dikirim, Selesai, Dibatalkan)
- Stok otomatis berkurang saat checkout dan kembali saat pesanan dibatalkan

## Akun demo

| Peran   | Email                          | Kata sandi  |
|---------|--------------------------------|-------------|
| Admin   | admin@marustationery.id        | admin123    |
| Pembeli | pembeli@marustationery.id      | pembeli123  |

Pembeli baru juga bisa mendaftar sendiri lewat tab **Daftar Pembeli**.

## Catatan penting

- Data (produk, pesanan, akun) disimpan di **browser** masing-masing (localStorage). Artinya, pesanan yang dibuat di satu perangkat tidak otomatis terlihat di perangkat lain. Ini cocok untuk demo, tugas, dan presentasi.
- Untuk toko sungguhan dengan banyak pengguna, diperlukan backend dan database (misalnya Firebase, Supabase, atau server sendiri).
- Kata sandi pada versi ini disimpan apa adanya untuk keperluan demo. Jangan gunakan pola ini untuk data pengguna nyata.
- Ganti akun admin demo sebelum aplikasi dipakai sungguhan (cukup ubah bagian `SEED_USERS` di `index.html`).

---

## Cara publish gratis di GitHub Pages

GitHub Pages gratis untuk repository **publik**. Anda tidak perlu kartu kredit.

### Langkah 1: Buat akun GitHub
1. Buka https://github.com lalu klik **Sign up**.
2. Isi email, kata sandi, dan nama pengguna (username). Nama pengguna akan menjadi bagian alamat website Anda, misalnya `azzam-dev`.
3. Verifikasi email Anda.

### Langkah 2: Buat repository baru
1. Setelah masuk, klik tombol **+** di pojok kanan atas, lalu pilih **New repository**.
2. Isi **Repository name**, misalnya `maru-stationery`.
3. Pilih **Public**.
4. Centang **Add a README file** (opsional, boleh tidak dicentang).
5. Klik **Create repository**.

### Langkah 3: Unggah file
1. Di halaman repository, klik **Add file** lalu **Upload files**.
2. Seret file `index.html` (dan `README.md` jika ada) ke area unggah.
3. Di bagian bawah, klik **Commit changes**.

Pastikan `index.html` berada di **halaman utama repository** (bukan di dalam folder).

### Langkah 4: Aktifkan GitHub Pages
1. Buka tab **Settings** di repository.
2. Di menu kiri, pilih **Pages**.
3. Pada bagian **Build and deployment** → **Source**, pilih **Deploy from a branch**.
4. Pada **Branch**, pilih **main** lalu folder **/ (root)**.
5. Klik **Save**.

### Langkah 5: Buka websitenya
1. Tunggu sekitar 1–3 menit.
2. Refresh halaman **Pages**. Akan muncul pesan seperti: *Your site is live at https://USERNAME.github.io/maru-stationery/*
3. Buka alamat tersebut. Ganti `USERNAME` dengan nama pengguna GitHub Anda.

Alamat ini bisa dibagikan kepada siapa pun.

### Cara memperbarui website
Setiap kali Anda mengubah `index.html`, ulangi **Langkah 3** dengan mengunggah ulang file tersebut (GitHub akan menggantinya). Perubahan biasanya tampil dalam 1–3 menit.

### Alternatif: lewat Git (untuk yang sudah terbiasa)
```bash
git init
git add index.html README.md
git commit -m "Publish Maru Stationery"
git branch -M main
git remote add origin https://github.com/USERNAME/maru-stationery.git
git push -u origin main
```
Lalu aktifkan Pages seperti pada Langkah 4.

### Jika ada kendala
- **Halaman 404**: pastikan nama file tepat `index.html` (huruf kecil) dan berada di root repository.
- **Tampilan belum berubah**: tunggu beberapa menit, lalu tekan Ctrl+F5 (atau Cmd+Shift+R di Mac).
- **Pilihan menu GitHub berbeda**: antarmuka GitHub kadang berubah. Cari menu **Pages** di Settings.

---

## Struktur berkas

```
maru-stationery/
├── index.html   # seluruh aplikasi (HTML, CSS, JavaScript)
└── README.md    # panduan ini
```
