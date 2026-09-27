# DompetKu V4

Aplikasi keuangan pribadi mobile-first, offline-first, dan siap dipasang sebagai PWA.

## Fitur V4
- Dashboard ringkasan bulan berjalan
- Pemasukan, Pengeluaran, Tabungan/Investasi
- Perbulan dengan Target Rp, Target % otomatis, Realisasi, Selisih, Status
- Pengeluaran dengan pencarian dan filter kategori
- Tabungan/investasi dengan saldo awal + transaksi tabungan
- Grafik pengeluaran per kategori, pemasukan vs pengeluaran, dan realisasi anggaran
- Kategori, metode/sumber uang, dan sumber pemasukan dapat dibuat sendiri
- Dark mode
- Sembunyikan nominal
- Backup dan restore JSON
- PIN lokal 4–6 digit menggunakan SHA-256 Web Crypto
- Ikon aplikasi + manifest PWA + service worker offline
- Migrasi otomatis dari DompetKu V2/V3
- Tidak ada data contoh bawaan

## Menjalankan
Buka melalui web server lokal, bukan `file://`, agar service worker dapat bekerja.

Contoh:

```bash
python3 -m http.server 8000
```

Lalu buka `http://localhost:8000/`.

## Catatan keamanan
PIN adalah kunci akses lokal pada aplikasi ini, bukan pengganti keamanan tingkat sistem operasi. Data utama disimpan di `localStorage` perangkat. Gunakan fitur Ekspor untuk membuat cadangan JSON.
