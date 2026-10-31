# M1 Perencanaan Elisitasi: Pengingat Salat dan Catatan Amalan Harian

Proyek Kelompok Rekayasa Perangkat Lunak (RPL 52338) · Topik 4

## 1. Analisis kelayakan 6 aspek

| Aspek       | Temuan singkat                                                                                                                                                                                                                                                    | Kesimpulan                                        |
|-------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------|
| Teknis      | Android native atau cross-platform (Kotlin/Flutter). Jadwal salat dari API publik. Tampil di atas aplikasi lain memerlukan izin overlay. Notifikasi layar penuh dibatasi di Android versi baru, tetapi lingkup sudah menyediakan cadangan notifikasi layar penuh. | Layak dengan catatan                              |
| Ekonomi     | Biaya pengembangan nyaris nol (tugas kuliah, AI coding assistant). API publik gratis. Penyimpanan lokal di HP, jadi tanpa biaya hosting. Manfaat: membantu ketepatan salat dan pencatatan amalan.                                                                 | Layak                                             |
| Hukum       | Catatan amalan adalah data ibadah yang sensitif secara sifatnya. Perlu persetujuan pengguna, penyimpanan seminimal mungkin, dan data lokal. Izin overlay harus dijelaskan transparan. Tidak memakai konten berhak cipta (doa, ayat) tanpa sumber jelas.           | Layak dengan catatan                              |
| Operasional | Mahasiswa muslim sudah terbiasa memakai alarm atau aplikasi salat. Risiko: pengingat layar penuh dianggap mengganggu, atau pengguna ragu memberi izin overlay. Mentor perlu cara melihat rekap tanpa melanggar privasi.                                           | Layak dengan catatan (dibuktikan lewat elisitasi) |
| Jadwal      | Versi pertama (8-15 kebutuhan inti) dibangun dengan AI dalam 2 pekan (M4). Lingkup sudah dibatasi: Android saja, tanpa penilaian pahala/dosa.                                                                                                                     | Layak                                             |
| Kompetitor  | Lihat tabel di bawah.                                                                                                                                                                                                                                             | Layak, pembeda jelas                              |

### Kompetitor

| Solusi                                                   | Kelebihan                           | Kekurangan                                                                                 |
|----------------------------------------------------------|-------------------------------------|--------------------------------------------------------------------------------------------|
| Aplikasi jadwal salat populer (mis. Muslim Pro, Athan)   | Jadwal akurat, adzan, banyak fitur  | Banyak fitur lain (iklan, premium), pengingat umumnya notifikasi biasa yang mudah terlewat |
| Alarm HP bawaan                                          | Sederhana, tanpa data pribadi       | Manual, tidak ikut jadwal berubah, tidak ada catatan amalan                                |
| Buku atau lembar mutaba'ah + grup WhatsApp (cara manual) | Familiar, tidak butuh aplikasi baru | Rekap manual, mudah lupa, mentor sulit memantau                                            |

**Pembeda ide:** pengingat yang tampil di atas aplikasi lain saat HP dipakai, digabung dengan catatan mutaba'ah sederhana tanpa penilaian pahala/dosa.

## 2. Lingkup awal dan masalah

**Masalah:** mahasiswa sering terlewat atau menunda salat karena asyik memakai HP.

https://docs.google.com/spreadsheets/d/1PJJGRTj3ElCJJvp72nEzv5xCUX-O2NKTwirslk99mg8/edit?usp=sharing **(bersifat sementara)**

**Lingkup awal (masuk):**

- Pengingat waktu salat dari API publik

- Tampilan di atas aplikasi lain dengan cadangan notifikasi layar penuh

- Catatan amalan harian

- Rekap sederhana

**Di luar lingkup:**

- iOS

- Penilaian pahala atau dosa (Tidak akan di masukkan)

- Fitur sosial atau ranking (bersifat local dan tidak mempengaruhi apapun)

- Konten ibadah lengkap (Al-Qur'an, doa, dll.)

## 3. Peta pemangku kepentingan

| Pemangku kepentingan                      | Kepentingan                                                                                | Cara menggali                            |
|-------------------------------------------|--------------------------------------------------------------------------------------------|------------------------------------------|
| Mahasiswa muslim (pengguna harian)        | Tidak terlewat salat, pengingat tidak mengganggu, mencatat amalan praktis, privasi terjaga | Kuesioner + observasi                    |
| Mentor/pembina kerohanian                 | Memantau mutaba'ah binaan efisien, rekap mudah, batas privasi jelas                        | Observasi + kuesioner singkat            |
| (Opsional) Pengelola masjid/musala kampus | Jadwal salat setempat                                                                      | Studi dokumen **[hanya bila relevan]** |

## 4. Rencana elisitasi

| Teknik                               | Pemangku kepentingan      | Narasumber                                   | Target                          | Jadwal                            |
|--------------------------------------|---------------------------|----------------------------------------------|---------------------------------|-----------------------------------|
| Kuesioner (Google Form)              | Mahasiswa muslim          | Mahasiswa semua Angkatan prodi ilmu komputer | 20-30 responden                 | Sebar 29 oktober s.d. 15 november |
| Observasi (lembar observasi)         | Mahasiswa, Mentor/pembina | Mahawsiswa ilmu komputer                     | 3 sesi mahasiswa, 1 sesi mentor | [tanggal], 20-30 menit per sesi |
| Kuesioner singkat (Google Form)      | Mentor/pembina            | Mentor/pembina kerohanian                    | 1-3 orang                       | [tanggal]                       |
| Studi pustaka/kompetitor (pelengkap) | -                        | Aplikasi pembanding                          | 2-3 aplikasi                    | [tanggal]                       |

**Pembagian tugas:** Requirements lead menghubungi narasumber, Analis mengolah rekap, Validator memeriksa kualitas pertanyaan. Semua anggota ikut pelaksanaan. Jadwal harus selesai sebelum 5 November (tenggat M2).

## 5. Instrumen siap pakai

Lampirkan:

- Kuesioner mahasiswa (23 pertanyaan)

- Kuesioner mentor/pembina (10 pertanyaan)

- Lembar observasi (perilaku mahasiswa di sekitar waktu salat dan proses mutaba'ah mentor)

- Pengantar penyebaran kuesioner

- Kalimat persetujuan (sukarela, anonim, izin observasi)

## 6. Pernyataan penggunaan AI (wajib)

Contoh isi: "Kelompok kami menggunakan [nama AI] untuk menyusun kerangka instrumen elisitasi dan merapikan bahasa dokumen M1. Seluruh keputusan lingkup, pemilihan narasumber, dan analisis kelayakan ditinjau dan disesuaikan oleh anggota kelompok. AI tidak digunakan untuk mengarang hasil elisitasi." Sesuaikan dengan penggunaan kalian yang sebenarnya.

## Sebelum dikumpulkan

- Ganti semua **[cek]** dan placeholder dengan hasil riset kalian sendiri, terutama API jadwal salat, aturan izin Android, dan fitur kompetitor.

- Pastikan tidak ada klaim "hasil survei" di M1, karena elisitasi baru dilakukan di M2.

- Unggah ke repo GitHub, lalu kirim tautannya ke e-learning. Tenggat di PDF Kamis 29 Oktober, jadi konfirmasi ke Bu Intan soal keterlambatan.
