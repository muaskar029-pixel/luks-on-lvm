# Rancangan GitHub Project: Produksi 1 Video Pendek

Rancangan ini dibuat berdasarkan workflow produksi video pendek Senin–Jumat. Setiap pekerjaan dijadikan satu task card agar progres, penanggung jawab, dependensi, dan hasil akhirnya mudah dipantau.

## 1. Pengaturan Project

**Nama project:** `Produksi Video Pendek Mingguan`

**Deskripsi:**

> Board untuk mengelola produksi satu video pendek berdurasi 20–60 detik, mulai dari ide dan praproduksi pada Senin sampai publikasi dan evaluasi pada Jumat.

**Tampilan utama:** Board

**Kolom status:**

1. `Backlog` — tugas belum dijadwalkan.
2. `Todo` — tugas siap dikerjakan pada minggu berjalan.
3. `In Progress` — tugas sedang dikerjakan.
4. `Review` — output sudah dibuat dan menunggu pemeriksaan/persetujuan.
5. `Done` — output sudah memenuhi kriteria penyelesaian.

## 2. Custom Field yang Disarankan

| Field | Tipe | Pilihan/contoh |
| --- | --- | --- |
| Hari | Single select | Senin, Selasa, Rabu, Kamis, Jumat |
| Fase | Single select | Pre-production, Production, Post-production, Publishing |
| Prioritas | Single select | High, Medium, Low |
| Estimasi | Number atau text | 15, 20, 30, 45, 90 menit |
| PIC | Assignee | Nama anggota yang bertanggung jawab |
| Output | Text | Script, storyboard, footage, final video, link publikasi |
| Target selesai | Date | Tanggal tugas harus selesai |

Jika kartu dibuat sebagai GitHub Issue, gunakan label berikut:

- `pre-production`
- `production`
- `post-production`
- `publishing`
- `needs-review`
- `blocked`

## 3. Daftar Task Card

| ID | Judul kartu | Hari | Fase | Estimasi | Dependensi |
| --- | --- | --- | --- | ---: | --- |
| MON-01 | Tentukan Ide dan Content Brief | Senin | Pre-production | 30 menit | — |
| MON-02 | Susun Pointer Script | Senin | Pre-production | 30 menit | MON-01 |
| MON-03 | Buat Storyboard dan Shot List | Senin | Pre-production | 45 menit | MON-02 |
| MON-04 | Susun Checklist Kebutuhan Produksi | Senin | Pre-production | 30 menit | MON-01–MON-03 |
| TUE-01 | Finalisasi Lokasi Shooting | Selasa | Pre-production | 30 menit | MON-04 |
| TUE-02 | Briefing Talent | Selasa | Pre-production | 30 menit | MON-02–MON-03 |
| TUE-03 | Siapkan Peralatan dan Test Footage | Selasa | Pre-production | 30 menit | MON-04, TUE-01 |
| WED-01 | Setup Lokasi, Talent, dan Peralatan | Rabu | Production | 30 menit | Seluruh tugas Selasa |
| WED-02 | Shooting Footage Utama dan Pendukung | Rabu | Production | 90 menit | WED-01 |
| WED-03 | Periksa dan Backup Footage | Rabu | Production | 15 menit | WED-02 |
| THU-01 | Seleksi Footage dan Buat Rough Cut | Kamis | Post-production | 30 menit | WED-03 |
| THU-02 | Edit Video Pendek | Kamis | Post-production | 90 menit | THU-01 |
| THU-03 | Review, Revisi, dan Export Final | Kamis | Post-production | 30 menit | THU-02 |
| FRI-01 | Siapkan Caption, Cover, dan Hashtag | Jumat | Publishing | 20 menit | THU-03 |
| FRI-02 | Upload atau Jadwalkan Video | Jumat | Publishing | 20 menit | FRI-01 |
| FRI-03 | Periksa Upload dan Catat Evaluasi | Jumat | Publishing | 20 menit | FRI-02 |

## 4. Isi Setiap Task Card

### MON-01 — Tentukan Ide dan Content Brief

**Tujuan:** Menentukan dasar dan arah video sebelum penulisan script.

**Checklist:**

- [ ] Tentukan topik video.
- [ ] Tentukan tujuan konten.
- [ ] Tentukan target audiens.
- [ ] Tentukan satu pesan utama.
- [ ] Kumpulkan 2–3 referensi video.

**Output:** Content brief dalam Markdown.

**Selesai jika:** Ide disetujui dan dapat dirangkum dalam satu kalimat yang jelas.

### MON-02 — Susun Pointer Script

**Tujuan:** Menyusun alur pembicaraan video berdurasi 20–60 detik.

**Checklist:**

- [ ] Tulis hook untuk tiga detik pertama.
- [ ] Tulis poin isi utama.
- [ ] Tulis call to action.
- [ ] Perkirakan durasi setiap bagian.
- [ ] Proofread script.

**Output:** Pointer script final dalam Markdown.

**Selesai jika:** Script memiliki hook, satu pesan utama, dan call to action serta sesuai batas durasi.

### MON-03 — Buat Storyboard dan Shot List

**Tujuan:** Menerjemahkan script menjadi rancangan visual dan daftar pengambilan gambar.

**Checklist:**

- [ ] Bagi script menjadi beberapa adegan.
- [ ] Tentukan visual untuk setiap adegan.
- [ ] Tentukan jenis shot dan sudut kamera.
- [ ] Tandai dialog, voice-over, atau teks layar.
- [ ] Buat daftar footage utama dan footage pendukung.

**Output:** Storyboard dan shot list dalam Markdown, JPG, atau PDF.

**Selesai jika:** Setiap bagian script memiliki rencana visual dan shot yang jelas.

### MON-04 — Susun Checklist Kebutuhan Produksi

**Tujuan:** Memastikan semua kebutuhan shooting sudah teridentifikasi.

**Checklist:**

- [ ] Tentukan kebutuhan talent.
- [ ] Tentukan kebutuhan lokasi.
- [ ] Catat kamera, mikrofon, dan pencahayaan.
- [ ] Catat properti dan pakaian.
- [ ] Simpan referensi visual.

**Output:** Checklist praproduksi dalam Markdown.

**Selesai jika:** Tidak ada kebutuhan utama pada storyboard yang belum masuk daftar.

### TUE-01 — Finalisasi Lokasi Shooting

**Tujuan:** Memastikan lokasi sesuai dengan kebutuhan visual dan teknis.

**Checklist:**

- [ ] Konfirmasi izin dan ketersediaan lokasi.
- [ ] Periksa pencahayaan.
- [ ] Periksa tingkat kebisingan.
- [ ] Tentukan titik kamera dan posisi talent.
- [ ] Ambil foto referensi lokasi.

**Output:** Foto lokasi dan checklist kesiapan.

**Selesai jika:** Lokasi tersedia, aman, cukup terang, dan memungkinkan perekaman audio yang jelas.

### TUE-02 — Briefing Talent

**Tujuan:** Memastikan talent memahami konsep dan kebutuhan shooting.

**Checklist:**

- [ ] Kirim pointer script dan storyboard.
- [ ] Jelaskan pesan dan gaya penyampaian.
- [ ] Konfirmasi pakaian dan properti pribadi.
- [ ] Konfirmasi waktu serta lokasi shooting.
- [ ] Pastikan talent memahami dialog atau poin bicara.

**Output:** Catatan briefing dan konfirmasi talent.

**Selesai jika:** Talent telah mengonfirmasi jadwal dan memahami perannya.

### TUE-03 — Siapkan Peralatan dan Test Footage

**Tujuan:** Memastikan perangkat produksi berfungsi sebelum hari shooting.

**Checklist:**

- [ ] Isi daya perangkat dan siapkan penyimpanan.
- [ ] Periksa kamera dan pengaturan video vertikal.
- [ ] Tes mikrofon dan level audio.
- [ ] Tes pencahayaan.
- [ ] Rekam dan periksa test footage singkat.

**Output:** Checklist peralatan dan test footage.

**Selesai jika:** Gambar dan audio test footage memenuhi standar serta semua peralatan siap dibawa.

### WED-01 — Setup Lokasi, Talent, dan Peralatan

**Tujuan:** Menyiapkan seluruh set sebelum perekaman dimulai.

**Checklist:**

- [ ] Tata lokasi dan properti.
- [ ] Tempatkan kamera dan pencahayaan.
- [ ] Pasang dan tes mikrofon.
- [ ] Briefing ulang talent secara singkat.
- [ ] Rekam tes terakhir.

**Output:** Set shooting siap digunakan.

**Selesai jika:** Framing, pencahayaan, audio, talent, dan properti sudah sesuai storyboard.

### WED-02 — Shooting Footage Utama dan Pendukung

**Tujuan:** Merekam seluruh materi video sesuai storyboard dan shot list.

**Checklist:**

- [ ] Rekam footage utama.
- [ ] Ambil beberapa versi untuk shot penting.
- [ ] Rekam footage pendukung atau B-roll.
- [ ] Periksa fokus dan audio secara berkala.
- [ ] Tandai take terbaik.

**Output:** Footage utama dan pendukung dalam MP4.

**Selesai jika:** Semua shot wajib tersedia dan kualitas gambar serta audio dapat digunakan.

### WED-03 — Periksa dan Backup Footage

**Tujuan:** Menghindari kehilangan atau kekurangan materi setelah shooting.

**Checklist:**

- [ ] Periksa seluruh file dapat dibuka.
- [ ] Cocokkan footage dengan shot list.
- [ ] Pisahkan atau tandai take terbaik.
- [ ] Buat minimal satu salinan cadangan.

**Output:** Folder footage lengkap dan backup.

**Selesai jika:** Semua shot wajib tersedia di penyimpanan utama dan cadangan.

### THU-01 — Seleksi Footage dan Buat Rough Cut

**Tujuan:** Membentuk struktur awal video dari footage terbaik.

**Checklist:**

- [ ] Impor dan susun seluruh footage.
- [ ] Pilih take terbaik.
- [ ] Susun footage sesuai pointer script.
- [ ] Buang bagian yang tidak diperlukan.
- [ ] Pastikan durasi awal mendekati 20–60 detik.

**Output:** Rough cut dan project file editing.

**Selesai jika:** Alur video sudah utuh dan dapat dipahami tanpa efek tambahan.

### THU-02 — Edit Video Pendek

**Tujuan:** Menyelesaikan aspek visual dan audio video.

**Checklist:**

- [ ] Rapikan cutting dan pacing.
- [ ] Tambahkan subtitle.
- [ ] Tambahkan musik dan sound effect seperlunya.
- [ ] Sesuaikan warna dan volume audio.
- [ ] Tambahkan elemen visual yang diperlukan.

**Output:** Draft video MP4 vertikal 9:16.

**Selesai jika:** Video berdurasi 20–60 detik, audio jelas, subtitle terbaca, dan pesan utama tersampaikan.

### THU-03 — Review, Revisi, dan Export Final

**Tujuan:** Memastikan video siap dipublikasikan tanpa kesalahan teknis atau isi.

**Checklist:**

- [ ] Review dari awal sampai akhir.
- [ ] Proofread subtitle dan teks layar.
- [ ] Periksa posisi teks terhadap antarmuka platform.
- [ ] Terapkan revisi yang disetujui.
- [ ] Export final 1080 × 1920 piksel.

**Output:** Final video MP4.

**Selesai jika:** Video telah disetujui, tidak memiliki kesalahan teks, dan memenuhi standar hasil akhir.

### FRI-01 — Siapkan Caption, Cover, dan Hashtag

**Tujuan:** Menyiapkan seluruh aset pendukung publikasi.

**Checklist:**

- [ ] Tulis caption yang sesuai isi video.
- [ ] Buat atau pilih cover.
- [ ] Pilih hashtag yang relevan.
- [ ] Tentukan platform dan waktu publikasi.
- [ ] Periksa kembali call to action.

**Output:** Caption Markdown dan cover JPG.

**Selesai jika:** Paket publikasi siap digunakan tanpa penulisan tambahan.

### FRI-02 — Upload atau Jadwalkan Video

**Tujuan:** Mempublikasikan video di platform yang telah ditentukan.

**Checklist:**

- [ ] Pilih file final yang benar.
- [ ] Masukkan caption dan hashtag.
- [ ] Pasang cover.
- [ ] Periksa pengaturan publikasi.
- [ ] Upload atau jadwalkan video.

**Output:** Video terpublikasi atau terjadwal.

**Selesai jika:** Video dapat diakses pada akun dan waktu publikasinya tercatat.

### FRI-03 — Periksa Upload dan Catat Evaluasi

**Tujuan:** Memastikan hasil publikasi benar dan menyimpan pembelajaran untuk produksi berikutnya.

**Checklist:**

- [ ] Putar video dari platform setelah upload.
- [ ] Periksa kualitas gambar, audio, subtitle, caption, dan cover.
- [ ] Simpan link publikasi.
- [ ] Catat masalah yang ditemukan.
- [ ] Catat satu perbaikan untuk video berikutnya.

**Output:** Link publikasi dan catatan evaluasi singkat.

**Selesai jika:** Link tersimpan, video tampil dengan benar, dan evaluasi telah dicatat.

## 5. Urutan Pembuatan Manual di GitHub

1. Buat project baru bernama `Produksi Video Pendek Mingguan`.
2. Gunakan tampilan Board dan buat lima status: Backlog, Todo, In Progress, Review, dan Done.
3. Tambahkan custom field Hari, Fase, Prioritas, Estimasi, PIC, Output, dan Target selesai.
4. Buat 16 draft task berdasarkan daftar kartu di atas.
5. Salin bagian tujuan, checklist, output, dan kriteria selesai ke deskripsi setiap kartu.
6. Atur Hari, Fase, estimasi, PIC, dan tanggal target masing-masing kartu.
7. Pindahkan semua tugas minggu berjalan ke Todo.
8. Saat bekerja, pindahkan kartu ke In Progress; setelah output dibuat, pindahkan ke Review.
9. Kartu hanya dipindahkan ke Done setelah kriteria “Selesai jika” terpenuhi.

## 6. Target Harian

| Hari | Jumlah kartu | Total estimasi | Hasil akhir harian |
| --- | ---: | ---: | --- |
| Senin | 4 | 2 jam 15 menit | Ide, script, storyboard, dan checklist produksi terkunci |
| Selasa | 3 | 1 jam 30 menit | Lokasi, talent, dan peralatan siap |
| Rabu | 3 | 2 jam 15 menit | Footage lengkap dan memiliki backup |
| Kamis | 3 | 2 jam 30 menit | Final video siap upload |
| Jumat | 3 | 1 jam | Video terpublikasi dan evaluasi tercatat |
| **Total** | **16** | **9 jam 30 menit** | **Satu video pendek selesai** |
