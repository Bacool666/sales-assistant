# Sales Assistant — MVP PWA

Aplikasi prototipe PWA berbahasa Indonesia untuk mengelola toko, order, simulasi inbox, draft persetujuan, pengingat internal, dan laporan.

## Fitur saat ini
- Dashboard ringkasan.
- Database toko: tambah, edit, hapus, cari.
- Manajemen order dan total dus.
- WhatsApp Center simulasi pesan masuk dan draft balasan.
- Persetujuan draft (hanya status lokal; tidak mengirim pesan).
- Daftar toko yang belum order hari ini dan draft pengingat.
- Laporan dan ekspor CSV.
- Backup dan restore JSON.
- PWA manifest dan service worker untuk penggunaan offline setelah di-host melalui HTTPS.
- Penyimpanan browser lokal (localStorage).

## Menjalankan
Untuk pengujian, jalankan server web lokal dari folder ini, misalnya:

```bash
python -m http.server 8000
```

Buka `http://localhost:8000` pada browser. Untuk pemasangan PWA pada Android, deploy folder ini ke hosting HTTPS lalu buka URL-nya di Chrome Android → menu → Tambahkan ke layar utama / Install app.

## Batasan penting
Ini adalah MVP lokal, bukan integrasi WhatsApp aktif. Inbox chat hanya simulasi. Tombol persetujuan tidak mengirim pesan. Belum ada autentikasi multi-user, server backend, sinkronisasi cloud, API Meta, atau OpenAI API. Jangan masukkan data sensitif atau token API ke versi ini. Integrasi produksi harus menggunakan WhatsApp Business Platform resmi, proses Coexistence jika nomor memenuhi syarat, backend aman, dan mekanisme persetujuan yang tervalidasi.
