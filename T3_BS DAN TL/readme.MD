##  Tugas membuat tampilan ig

Proyek ini adalah implementasi sederhana tampilan **profil Instagram** menggunakan **HTML**, dengan dua pendekatan framework CSS: **Bootstrap 5** dan **Tailwind CSS**.  

Tujuan proyek ini adalah untuk berlatih membuat layout responsif, grid foto, serta interaksi dasar dengan link gambar.  
Dengan membandingkan Bootstrap dan Tailwind, kita bisa memahami kelebihan dan perbedaan dua framework CSS populer ini.

---

## Fitur Utama
1. **Header**
   - Menampilkan nama akun.
   - Tombol Edit Profil dengan tampilan berbeda di desktop dan mobile.

2. **Profil User**
   - Foto profil berbentuk lingkaran.
   - Nama pengguna.
   - Bio singkat.
   - Statistik: jumlah Postingan, Pengikut, dan Mengikuti.

3. **Feed Foto**
   - Terdiri dari 12 foto (`1.jpg` sampai `12.jpg`).
   - Grid responsif:
     - 2 kolom di HP.
     - 3 kolom di tablet.
     - 4 kolom di desktop.
   - Efek hover zoom.
   - Klik foto membuka gambar asli di tab baru.

4. **Responsif**
   - Tampilan mobile-first.
   - Elemen berubah otomatis mengikuti ukuran layar.

---

## Teknologi yang Digunakan

### Versi Bootstrap
- **Bootstrap 5.3.3 (CDN)**.
- Sistem grid menggunakan `row` dan `col`.
- Komponen card (`card`) untuk feed foto.
- Utility class seperti `d-flex`, `justify-content-center`, `text-center`, dan `btn`.
- Styling tambahan di `assets/css/custom.css`.

### Versi Tailwind
- **Tailwind CSS (CDN)**.
- Utility-first classes seperti `grid`, `flex`, `rounded-full`, `hover:scale-105`.
- Styling langsung di HTML.
- Tidak membutuhkan file CSS tambahan besar.

---

## Perbedaan Bootstrap vs Tailwind dalam Proyek Ini

| Aspek                | Bootstrap                                      | Tailwind                                     |
|-----------------------|------------------------------------------------|----------------------------------------------|
| Grid Foto             | `row` + `col-sm-6 col-lg-3`                   | `grid grid-cols-2 md:grid-cols-3 lg:grid-cols-4` |
| Tombol Edit Profil    | `btn btn-primary`                              | `px-4 py-2 bg-blue-500 text-white rounded-lg` |
| Efek Hover Foto       | CSS tambahan di `custom.css`                   | `hover:scale-105 transition`                 |
| Responsif             | Breakpoint Bootstrap (`sm`, `md`, `lg`)        | Breakpoint Tailwind (`sm:`, `md:`, `lg:`)    |

## Kesimpulan

Proyek ini menunjukkan bagaimana satu layout sederhana bisa dibangun dengan dua pendekatan berbeda:

Bootstrap dengan komponen siap pakai dan class utility bawaan.

Tailwind dengan pendekatan utility-first yang lebih fleksibel dan langsung di HTML.

Keduanya sama-sama efektif untuk membangun layout responsif. Bootstrap lebih cepat untuk pemula karena banyak komponen siap pakai, sedangkan Tailwind memberi kebebasan styling yang lebih detail.

Proyek ini sangat cocok sebagai latihan dasar untuk memahami responsive design, grid foto, dan interaksi dasar web.