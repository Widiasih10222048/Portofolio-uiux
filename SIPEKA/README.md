# SIPEKA - Sistem Pakar Estimasi Kematian

Perancangan sistem pakar berbasis web untuk memperkirakan **Postmortem Interval (PMI)**, yaitu estimasi waktu kematian korban tindak pidana, dari kondisi fisik jenazah.

Tugas kelompok mata kuliah Sistem Pakar, STT Cipasung, 2026. **Status:** tahap perancangan (prototipe Figma).

[Lihat prototipe Figma](https://www.figma.com/design/2MzW82ESDdZUVoIlT4nYeK/SIPEKA?node-id=0-1&t=ejyUn4ZGymcPWZbj-1)

## Peran Saya
- **Bab A (Penilaian):** masalah, tujuan sistem, dan kebutuhan resource.
- **Bab B (Akuisisi Pengetahuan):** kebutuhan, sumber, dan cara mendapatkan pengetahuan pakar.
- **Desain Figma:** seluruh 9 layar untuk 2 peran pengguna (pengguna dan admin).
- **Dokumentasi:** USE Case dan Flowchart.

## Masalah
POLRI mencatat 3.347 perkara pembunuhan dalam 4 tahun (puncak 1.076 kasus pada 2021), sedangkan dokter forensik di Indonesia baru 283 orang pada 2022 dan sebarannya belum merata. Sistem pakar membantu memberi estimasi awal PMI saat akses ke dokter forensik terbatas.

## Layar (Figma)
| Layar | Fungsi |
|---|---|
| Masuk | Login dengan kode otoritas, kunci keamanan, dan biometrik |
| Beranda | Sambutan dan panduan teknis |
| Riwayat Analisis | Arsip hasil PMI dan cetak Visum et Repertum |
| Analisis Jenazah | Input 4 parameter klinis dan hasil estimasi |
| Ruang Admin | Parameter Henssge, kredensial, audit trail |
| Penambahan Akun | Pendaftaran akun oleh admin |
| Basis Pengetahuan | Kelola gejala klinis |
| Daftar Aturan | Kelola aturan IF-THEN |
| Profil | Data akun dan ubah password |

![Analisis Jenazah](screens/04-analisis-jenazah.png)

*Data pada layar adalah contoh untuk prototipe.*

## SDLC
Dokumen disusun berurutan seperti model Waterfall:

| Tahap | Bab | Status |
|---|---|---|
| Analisis kebutuhan | A (bagian saya) | Selesai |
| Akuisisi pengetahuan | B (bagian saya) | Selesai |
| Perancangan | C, UI/UX oleh saya | Selesai |
| Implementasi | - | Belum dibangun |
| Pengujian | D | Rencana selesai |
| Dokumentasi (Bagian Saya) | E | Selesai |
| Pemeliharaan | F | Rencana selesai |

## Ringkasan Sistem (Tim)
Metode inferensi *Forward Chaining* dengan parameter algor mortis, livor mortis, rigor mortis, dekomposisi, dan faktor pakaian. Teknologi rencana: HTML, CSS, JavaScript, PHP, MySQL.