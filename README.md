# ZVRA Performance Valorant

Toolkit tweak Windows buat optimasi ringan sebelum main Valorant — prioritas CPU, RAM threshold, cleanup, dan latency tweak. Semua dikumpulkan dalam satu halaman biar gampang diakses.

## Cara Pakai

1. Buka `ZVRA_Performance_Valorant.html` di browser (double-click file-nya, atau akses lewat GitHub Pages kalau sudah di-enable).
2. Pilih tweak yang mau dipakai, klik tombol **Download**.
3. File `.reg` → klik kanan → **Merge** → Yes.
   File `.bat` / `.cmd` → klik kanan → **Run as administrator**.
4. Restart PC setelah import registry biar perubahan efektif.

> Website ini 100% jalan di browser (client-side). Tidak ada data yang dikirim atau disimpan ke server manapun.

## Isi Toolkit

| Kategori | Deskripsi |
|---|---|
| **RAM Threshold (1GB–32GB)** | Atur `SvcHostSplitThresholdInKB` sesuai RAM fisik PC |
| **Valorant Priority** | Atur prioritas CPU proses Valorant (High / Above Normal / Normal) |
| **Valorant Safe Optimization** | Game priority, disable Game DVR, transparency, Xbox services — printer & Bluetooth tidak disentuh |
| **Disable Memory Compression** | Matikan kompresi RAM Windows |
| **Latency Tweaks** | Disable Dynamic Tick & HPET |
| **Clean Temporary Files** | Hapus folder Temp, Windows Temp, dan Prefetch |
| **Reset to Default** | Balikin RAM threshold ke nilai default |

## ⚠️ Peringatan

- **Buat System Restore Point dulu** sebelum menjalankan script apapun (Search → "Create a restore point" → Create).
- Semua tweak di sini dipilih agar **tidak mematikan service yang biasa dipakai kerja** (printer, Bluetooth). Kalau ragu, buka dulu isi file `.reg`/`.bat` pakai Notepad sebelum dijalankan — semuanya plain text.
- Efek tweak ini **kecil–menengah** (bantu stabilitas & latency), bukan lompatan FPS besar. Faktor terbesar tetap: driver GPU, power plan, dan aplikasi background yang berat.
- Gunakan dengan risiko sendiri (**use at your own risk**). Repo ini sengaja tidak menyertakan tweak yang mematikan proteksi keamanan Windows (process mitigation) karena risikonya terlalu besar dibanding manfaatnya.

## Struktur Repo

```
ZVRA_Performance_Valorant.html   ← website utama, jalankan/buka ini
README.md
```

---
Dibuat berdasarkan kumpulan tweak dari ZVRA & BareFox.
