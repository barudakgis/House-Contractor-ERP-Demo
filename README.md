# HC-ERP — Versi Demo

Satu berkas `index.html` berisi seluruh aplikasi: tampilan PWA dan **semua kode server Google Apps Script (.gs) yang sama persis**, dijalankan di browser di atas tiruan Google Sheets. Tidak perlu akun Google, server, atau instalasi.

## Cara pasang (GitHub Pages)
1. Buat repositori baru, misalnya `hcerp-demo`.
2. Unggah `index.html` ke akar repositori.
3. Settings → Pages → Deploy from branch → `main` / root → Save.
4. Bagikan alamat `https://<user>.github.io/hcerp-demo/` ke calon klien (misalnya untuk balasan DM "DEMO").

Bisa juga dibuka langsung dari komputer (klik dua kali `index.html`).

## Yang bisa dicoba
- **Masuk satu klik** sebagai 11 peran: Admin, Direktur, PM, QS, Site Engineer, Pengadaan, Gudang, Keuangan, QC, Marketing, Mandor. Sandi semua akun: `Demo#2026`.
- **Portal Pemilik Rumah**: 0812-1111-0002 (rumah sedang dibangun) dan 0812-1111-0004 (sudah serah terima).
- **Pesan**: pengingat tagihan & approval alert WhatsApp/email disimulasikan, isinya bisa dilihat di tombol "Pesan".
- **Offline**: tombol "Offline" mensimulasikan hilang sinyal; presensi & laporan masuk antrean lalu terkirim otomatis saat online lagi.
- **Reset**: mengembalikan data contoh dari awal.

## Batasan demo
- Data tersimpan hanya di browser pengunjung (IndexedDB), tidak dibagi antarpengunjung.
- WhatsApp, email, lisensi, dan backup Google Drive tidak benar-benar berjalan.
- Semua fitur terbuka (tanpa batas paket).

## Membangun ulang
Dari folder sumber: `python3 build.py && python3 demo/build_demo.py` → `demo/dist/index.html`.
