# **PRD Portofolio Landing Page: Roihatul Azizah**

**Versi:** 1.0 (draf awal)  \|  **Tanggal:** 13 November 2026  \|  **Penyusun:** Roihatul Azizah  \|  **Platform pembuatan:** Antigravity  \|  **Hosting:** Netlify  
Bagian yang ditandai **\[Asumsi\]** belum dikonfirmasi dan dapat diubah. Daftar pertanyaan yang masih terbuka ada di bagian 14\.

## **1\. Ringkasan**

Landing page portofolio satu halaman untuk melamar pekerjaan dan magang di bidang teknologi pendidikan, produk digital, dan pengembangan web berbantuan AI. Halaman ini mengumpulkan CV, sembilan tugas dan proyek bootcamp, capstone, skripsi, serta karya media dalam satu tautan yang mudah dibuka rekruter. Struktur dan kesan visualnya terinspirasi dari portofolio referensi di Behance (“Sabrina’s Portfolio 2026”): cover bertahun, perkenalan diri, daftar isi per kategori, proyek pilihan, dan halaman studi kasus. Referensi dipakai sebagai inspirasi struktur saja, bukan untuk menyalin tata letak, teks, atau aset.

## **2\. Masalah yang diselesaikan**

> * Bukti kemampuan tersebar di banyak tempat: dua situs Netlify, satu situs capstone, repositori GitLab, dan enam folder Google Drive. Rekruter harus membuka banyak tautan untuk memahami satu orang.  
> * CV dua halaman tidak memuat tampilan produk, alur pengguna, atau hasil yang dapat dicoba langsung.  
> * Profil Roihatul bersifat lintas bidang (teknologi pendidikan, pengembangan web berbantuan AI, UI/UX, administrasi dan fasilitasi kelas). Tanpa narasi yang jelas, profil ini mudah terbaca sebagai tidak fokus.  
> * Folder Drive tidak memberi kesan pertama yang rapi dan tidak menjelaskan peran Roihatul di tiap proyek.

## **3\. Tujuan dan non-tujuan**

### **Tujuan**

> 1. Dalam 10 detik pertama, pengunjung tahu siapa Roihatul, posisi yang dilamar, dan satu bukti terkuat (Capstone Terbaik 2 Future Innovators Bootcamp 2026).  
> 2. Pengunjung dapat membuka proyek unggulan dalam satu klik dari halaman utama.  
> 3. Setiap proyek punya studi kasus pendek: masalah, peran, solusi, hasil, dan tautan yang bisa dicoba.  
> 4. Seluruh tampilan konsisten karena mengikuti satu design system (bagian 12).  
> 5. Halaman cepat, terbaca di ponsel, dan memenuhi kontras WCAG 2.1 AA.

### **Non-tujuan (versi 1.0)**

> * Tidak ada blog, CMS, atau panel admin. Konten disimpan sebagai berkas data di repositori.  
> * Tidak ada login, database, atau pembayaran. Supabase tidak diperlukan.  
> * Tidak menggantikan CV. Halaman ini melengkapinya, dan CV tetap tersedia sebagai PDF.

## **4\. Pengguna dan skenario**

| Pengguna | Yang dicari | Skenario utama |
| :---- | :---- | :---- |
| Rekruter atau HR | Kecocokan dengan lowongan, bukti hasil, kontak | Membuka tautan dari email lamaran, memindai halaman kurang dari semenit, mengunduh CV. |
| Hiring manager (produk, web, edtech) | Kualitas proses: PRD, user story, peran di proyek, tautan aplikasi yang berjalan | Membuka satu studi kasus, mencoba aplikasi, melihat repositori atau laporan. |
| Mentor, penyelenggara bootcamp, komunitas | Perkembangan dan pencapaian | Melihat capstone, penghargaan, dan pengalaman relawan. |

## **5\. Posisi dan narasi**

**Headline:** Educational Technologist \| AI Web Programming (sesuai CV).  
**Pesan inti:** Lulusan Kurikulum dan Teknologi Pendidikan UNNES (IPK 3,72) yang membangun aplikasi pembelajaran web, dari PRD sampai deployment, bersama AI coding agent sambil membaca, menguji, dan meninjau kode sendiri.  
**Urutan bukti, dari yang terkuat:**

> 1. Capstone Terbaik 2, Future Innovators Bootcamp (Ioda Academy x Plan International Indonesia), lewat LMS full-stack.  
> 2. Skripsi: aplikasi web pembelajaran computational thinking dengan gamifikasi (XP, streak, leaderboard, hint bertingkat).  
> 3. Sembilan tugas dan proyek bootcamp dengan PRD, user story Given-When-Then, RBAC, payment gateway, dan deployment.  
> 4. Dampak media: 306 ribu tayangan pada satu reels, 1.561 followers Instagram program Kampus Mengajar Angkatan 7\.  
> 5. Volunteer of the Month, Juli 2026, Hari Senin.

**Keterbukaan soal AI:** halaman menyebut bahwa proyek dibangun bersama Antigravity dan menjelaskan bagian yang dikerjakan sendiri (PRD, ERD, logika gamifikasi, peninjauan kode, pengujian). Sikap ini sama dengan yang tertulis di CV.

## **6\. Lingkup versi 1.0**

### **Termasuk**

> * Satu halaman dengan navigasi anchor dan halaman detail untuk tiap studi kasus.  
> * Tampilan responsif (360 px sampai 1440 px), mode terang dan gelap.  
> * Tombol unduh CV (PDF), tautan LinkedIn, GitHub, dan email.  
> * Meta tag SEO dan gambar pratinjau Open Graph supaya tautan tampil rapi saat dibagikan.  
> * Bahasa Indonesia sebagai bahasa utama. **\[Asumsi\]** Versi Inggris ditunda ke versi 1.1.

### **Tidak termasuk**

> * Form kontak dengan penyimpanan data. Kontak lewat tautan email dan LinkedIn. **\[Asumsi\]**  
> * Animasi 3D, video latar, atau pustaka animasi berat.

## **7\. Struktur halaman dan kebutuhan fungsional**

| No | Seksi | Isi | Sumber |
| :---- | :---- | :---- | :---- |
| 00 | Navbar | Nama, anchor ke seksi, tombol “Unduh CV”, pengalih tema terang atau gelap. Tetap di atas saat scroll. | CV |
| 01 | Hero (cover) | Label “Portofolio 2023 sampai 2026”, nama, headline, satu kalimat pembuka, tombol “Lihat proyek” dan “Unduh CV”, foto. | CV, foto Roihatul |
| 02 | Tentang | Dua paragraf pendek: latar edtech, cara kerja bersama AI, minat belajar dan mengubah materi menjadi pengalaman interaktif. | Ringkasan profesional CV |
| 03 | Angka ringkas | IPK 3,72; Capstone Terbaik 2; 9 tugas dan proyek bootcamp; 306 ribu tayangan reels; 1.561 followers. | CV |
| 04 | Daftar isi proyek | Empat kategori bernomor, mengikuti pola “Table of Contents” pada referensi: Aplikasi Web, Riset dan Skripsi, Proyek Bootcamp, Desain dan Media. Klik kategori menggulir ke kelompok proyeknya. | Daftar proyek |
| 05 | Proyek unggulan | Tiga kartu besar. **\[Asumsi\]** LMS Pijar Aksara, aplikasi skripsi, Dapur Nia. | Bagian 8 |
| 06 | Semua proyek | Grid kartu dengan filter kategori. Tiap kartu membuka halaman studi kasus. | Bagian 8 |
| 07 | Pengalaman dan pendidikan | Linimasa: Hari Senin, Talentiv, Kampus Mengajar 7, Tim Media UNNES Awards 2024, Madin dan Bimbel Khoiro Ummah, UNNES. | CV |
| 08 | Skill dan tools | Dikelompokkan: pengembangan web berbantuan AI, produk dan desain, fasilitasi dan administrasi. Tidak memakai bar persentase. | Informasi tambahan CV |
| 09 | Pelatihan dan penghargaan | Future Innovators Bootcamp, Bootcamp Kilat UI/UX dan Product Management HARISENIN, Bootcamp Canva MudaCanva, Bootcamp UI/UX SpecialSkill, Volunteer of the Month. | CV |
| 10 | Kontak dan footer | Ajakan singkat, email, LinkedIn, GitHub, tombol unduh CV, tahun hak cipta. | CV |

### **Kebutuhan fungsional**

> 1. Konten proyek, profil, dan pengalaman dibaca dari berkas data (content/projects.json, content/profile.json), bukan ditulis langsung di komponen.  
> 2. Setiap tautan eksternal dibuka di tab baru dan diberi label jenisnya (Live, Repositori, Laporan, Video, Canva).  
> 3. Gambar yang gagal dimuat menampilkan placeholder dengan teks alternatif. Data proyek yang kosong menampilkan pesan “Studi kasus segera hadir”.  
> 4. Filter kategori dapat dipakai dengan keyboard dan mengumumkan hasilnya ke pembaca layar.  
> 5. Tema mengikuti pengaturan sistem pada kunjungan pertama, lalu mengingat pilihan pengunjung.  
> 6. Animasi masuk dimatikan saat pengunjung memakai pengaturan “reduce motion”.

## **8\. Konten proyek**

Usulan: sesi 2, 3, dan 4 digabung menjadi satu studi kasus Dapur Nia (PRD, aplikasi, deployment) agar tidak terlihat berulang. Kolom “Perlu dilengkapi” diisi lewat form yang dikirim terpisah.

| Studi kasus | Kategori | Tautan yang sudah ada | Perlu dilengkapi |
| :---- | :---- | :---- | :---- |
| LMS Lembaga Kursus Pijar Aksara (Capstone Terbaik 2\) | Aplikasi Web | [Web](https://insletabagkarungijaksara.mihatul.site/), [GitLab](https://gitlab.com/jongroihatulazizah1201-ui/lms_lembaga_kursus_pijar_aksara), [Video demo dan laporan](https://drive.google.com/drive/u/0/folders/1OkDIa5ZBsDG97QgKl03YwbSqVfsnk6nR) | Tangkapan layar, akun demo (jika ada), peran persis |
| Aplikasi Web Pembelajaran Computational Thinking (skripsi) | Riset dan Skripsi | Belum ada tautan | Tautan aplikasi atau video, tangkapan layar, izin menampilkan data siswa (jika ada) |
| Dapur Nia: PRD, aplikasi katering, deployment (sesi 2, 3, 4\) | Proyek Bootcamp | [Drive sesi 2](https://drive.google.com/drive/u/0/folders/1BIGFdgrwKFhalo6paBA7XvKDhLGW6NC5), [Drive sesi 3](https://drive.google.com/drive/u/0/folders/1jxmHeTI9suggBnXgR_ZyEA3D_3ybTrWK), [Web sesi 4](https://dapurniasection1.netlify.app/) | Ringkasan masalah dan hasil, tangkapan layar |
| Portal HRIS Sedap | Proyek Bootcamp | [Drive sesi 5](https://drive.google.com/drive/u/0/folders/1u29wuCFiZTLMQh4EAi2SLe-9jP61YPt3) (termasuk papan Canva) | Tautan aplikasi (jika ada), ringkasan, tangkapan layar |
| Bimbel Langkah Juara | Proyek Bootcamp | [Drive sesi 6](https://drive.google.com/drive/u/0/folders/1fWCbFe2BvwgzhU9IhE8Z-3n5wdEqnL_2) | Tautan aplikasi, ringkasan, tangkapan layar |
| Bengkel Cemerlang Jaya (payment gateway) | Proyek Bootcamp | [Drive sesi 9](https://drive.google.com/drive/u/0/folders/1xPv_um8Ju9po-FZI7z73-Z0PrJYDu9em) | Tautan aplikasi, ringkasan alur pembayaran, tangkapan layar |
| Landing Page Toko Buku | Aplikasi Web | [Web](https://bright-granita-5c6995.netlify.app/) | Ringkasan, keputusan soal catatan token limit (bagian 14\) |
| Desain dan media: papan Canva sesi 7, prototipe MINPUS (Figma), konten Kampus Mengajar | Desain dan Media | [Drive sesi 7](https://drive.google.com/drive/u/0/folders/1t4UbO7sQQ3k_wvtQll215dqC6XUUzrrl) | Tautan Figma, contoh konten, tangkapan layar |

### **Template studi kasus**

> 1. Judul, satu kalimat ringkasan, dan gambar utama.  
> 2. Metadata: peran, periode, tech stack, konteks (bootcamp, skripsi, atau tugas).  
> 3. Masalah dan pengguna.  
> 4. Yang dikerjakan sendiri dan yang dikerjakan bersama AI coding agent.  
> 5. Solusi: 3 sampai 5 tangkapan layar dengan keterangan.  
> 6. Hasil: penghargaan, angka, atau pelajaran.  
> 7. Tautan: Live, Repositori, Laporan, Video.  
> 8. Navigasi ke proyek berikutnya.

## **9\. Gaya penulisan konten**

> * Bahasa Indonesia yang lugas, sudut pandang orang pertama, kalimat pendek.  
> * Setiap klaim disertai fakta: angka, penghargaan, atau tautan yang bisa dibuka.  
> * Peran ditulis dengan kata kerja yang spesifik (menyusun PRD, merancang logika gamifikasi, meninjau kode), bukan “terlibat dalam”.  
> * Hambatan proses, seperti batas token pada proyek Toko Buku, ditulis sebagai pelajaran kerja (membagi tugas menjadi sesi pendek dan mengatur prompt), bukan sebagai keluhan. **\[Asumsi\]**  
> * Nomor telepon tidak ditampilkan sebagai teks di halaman publik untuk mengurangi spam. **\[Asumsi\]**

## **10\. Kebutuhan non-fungsional**

| Aspek | Target |
| :---- | :---- |
| Performa (ponsel, jaringan 4G) | LCP 2,5 detik atau kurang, CLS 0,1 atau kurang, INP 200 ms atau kurang. Skor Lighthouse 90 atau lebih untuk Performance, Accessibility, Best Practices, dan SEO. |
| Aksesibilitas | Kontras teks minimal 4,5:1, semua gambar punya teks alternatif, fokus keyboard terlihat, urutan heading benar, target sentuh minimal 44 px. |
| Responsif | Diuji di 360, 768, 1024, dan 1440 px. Tidak ada scroll horizontal. |
| Ukuran gambar | Format WebP atau AVIF, lebar sesuai kebutuhan, lazy-load di bawah lipatan pertama. |
| SEO dan berbagi | Judul dan deskripsi per halaman, gambar Open Graph 1200 x 630 px, sitemap, favicon. |
| Keandalan tautan | Semua tautan eksternal diperiksa sebelum rilis. Folder Drive dan papan Canva diatur “Anyone with the link” agar dapat dibuka pengunjung. |
| Privasi | Analitik ringan tanpa cookie pelacak lintas situs. Tidak menyimpan data pengunjung. |

## **11\. Arsitektur dan cara kerja di Antigravity**

**\[Asumsi\]** Stack: Next.js dengan ekspor statis, Tailwind CSS, konten dalam JSON atau MDX, deploy ke Netlify. Stack ini sama dengan yang sudah dipakai di capstone dan skripsi, tanpa Supabase karena halaman tidak menyimpan data.

### **Struktur folder proyek**

> * /content: profile.json, projects.json, experience.json  
> * /public/assets/photos: foto Roihatul (folder yang akan dibuat sendiri)  
> * /public/assets/projects/\<slug\>: tangkapan layar tiap proyek  
> * /public/cv: berkas CV PDF  
> * /docs: PRD ini dan pedoman design system sebagai sumber acuan agen

### **Aturan kerja bersama agen**

> 1. PRD dan design system disimpan di /docs dan dirujuk di setiap sesi.  
> 2. Satu milestone per sesi, dengan kriteria selesai yang jelas, supaya sesi pendek dan tidak menghabiskan token.  
> 3. Setiap hasil dibaca, dijalankan, dan diuji sebelum lanjut ke milestone berikutnya.  
> 4. Warna, ukuran huruf, dan spasi hanya diambil dari token (bagian 12), tidak ditulis ulang di komponen.

## **12\. Pedoman design system**

**\[Asumsi\]** Arah visual ini draf awal berdasarkan struktur referensi dan bidang edtech. Warna, font, dan nuansa disesuaikan setelah preferensi visual dikonfirmasi.

### **12.1 Arah visual**

> * Editorial dan hangat: judul besar, nomor seksi, banyak ruang kosong, kartu dengan sudut membulat.  
> * Satu warna utama untuk aksi dan tautan, satu warna aksen untuk penekanan kecil. Aksen tidak dipakai sebagai warna teks.  
> * Tampilan terang dan gelap memakai token yang sama dengan nilai berbeda.

### **12.2 Warna (token)**

| Token | Terang | Gelap | Dipakai untuk |
| :---- | :---- | :---- | :---- |
| bg | \#FBF7F2 | \#14121C | Latar halaman |
| surface | \#FFFFFF | \#1D1A29 | Kartu, navbar |
| ink | \#1F1B2E | \#F4F1FA | Teks utama |
| muted | \#5B566B | \#B5AFC7 | Teks pendukung, keterangan |
| primary | \#4B3FE0 | \#A79BFF | Tombol utama, tautan, fokus |
| on-primary | \#FFFFFF | \#14121C | Teks di atas tombol utama |
| accent | \#FF7A59 | \#FF9175 | Penanda kecil, garis, nomor seksi (bukan teks isi) |
| border | \#E7E0D6 | \#2E2A3D | Garis kartu dan pemisah |
| success | \#1B7A50 | \#5BCB95 | Status berhasil |
| error | \#B3261E | \#FF8A80 | Status gagal |

Rasio kontras yang sudah dihitung (terang): ink pada bg 15,7:1; muted pada bg 6,6:1; primary pada bg 6,4:1; on-primary pada primary 6,8:1. Gelap: ink pada bg 16,6:1; muted pada bg 8,8:1; primary pada bg 7,8:1. Semua di atas 4,5:1. Nilai gelap untuk success, error, dan border perlu diperiksa ulang saat diterapkan di komponen.

### **12.3 Tipografi**

> * Judul: Bricolage Grotesque, bobot 700\. Isi: Inter, bobot 400 dan 600\. Label dan nomor seksi: JetBrains Mono, bobot 500, huruf kapital, jarak antarhuruf 0,08 em. Semua dimuat dari Google Fonts dengan fallback sistem (sans-serif dan monospace).  
> * Skala (desktop / ponsel): Display 64/68 dan 40/44; H1 44/50 dan 32/38; H2 32/40 dan 26/34; H3 22/30 dan 20/28; isi 16/26; keterangan 14/22; label 12/16.  
> * Panjang baris isi maksimal 70 karakter.

### **12.4 Spasi, grid, dan bentuk**

> * Satuan dasar 4 px. Skala spasi: 4, 8, 12, 16, 24, 32, 48, 64, 96, 128\.  
> * Lebar konten maksimal 1120 px. Grid 12 kolom di desktop (jarak 24 px), 8 kolom di tablet, 4 kolom di ponsel (jarak 16 px).  
> * Breakpoint: 640, 1024, 1280 px.  
> * Jarak antarseksi 96 px (desktop) dan 64 px (ponsel).  
> * Radius: 8 px (chip, input), 16 px (kartu), 24 px (gambar besar), penuh (tombol dan tag).  
> * Bayangan: satu level lembut untuk kartu saat hover. Selain itu hanya garis border 1 px.

### **12.5 Komponen**

| Komponen | Aturan |
| :---- | :---- |
| Tombol | Tiga varian: utama (isi primary), sekunder (garis primary), teks. Tinggi 44 px, padding horizontal 20 px. Status: normal, hover, fokus, ditekan, nonaktif. |
| Header seksi | Nomor (label mono, warna accent), judul H2, satu kalimat pengantar maksimal dua baris. |
| Kartu proyek | Gambar rasio 16:10, chip kategori, judul H3, satu kalimat ringkasan, chip tech stack maksimal empat. Seluruh kartu dapat diklik. Hover: naik 4 px dan bayangan lembut. |
| Chip dan tag | Tinggi 28 px, radius penuh, teks 12 px. Chip kategori memakai latar tipis dari primary, chip stack memakai garis border. |
| Kartu angka | Angka besar (H1), keterangan 14 px di bawahnya. Empat sampai lima kartu dalam satu baris di desktop, dua kolom di ponsel. |
| Linimasa | Garis vertikal border, titik accent, judul peran, organisasi, periode, dua sampai empat poin. |
| Navbar | Tinggi 64 px, latar surface dengan garis bawah border. Di ponsel berubah menjadi menu lipat. |
| Status data | Tiga kondisi wajib ada untuk daftar proyek dan gambar: memuat (kerangka abu-abu), kosong (pesan dan tautan kembali), gagal (pesan dan tombol coba lagi). |

### **12.6 Gambar dan ikon**

> * Foto profil: satu gaya pemotongan, latar polos atau senada dengan bg, teks alternatif “Foto Roihatul Azizah”.  
> * Tangkapan layar proyek: bingkai perangkat yang sama untuk semua, rasio 16:10, minimal 1280 px lebar sebelum dikompres.  
> * Ikon: Lucide, garis 1,5 px, ukuran 20 atau 24 px, warna mengikuti teks.

### **12.7 Gerak**

> * Durasi 150 sampai 250 ms, easing ease-out. Tidak ada animasi di atas 400 ms.  
> * Efek masuk saat scroll: geser naik 12 px dan memudar, jeda antarelemen 60 ms, hanya sekali per elemen.  
> * Pengaturan “reduce motion” mematikan semua gerak selain perubahan warna.

### **12.8 Aksesibilitas**

> * Cincin fokus 2 px warna primary dengan offset 2 px pada semua elemen interaktif.  
> * Satu H1 per halaman, urutan heading tidak melompat.  
> * Informasi tidak disampaikan hanya lewat warna.  
> * Tautan “Lihat selengkapnya” diberi teks lengkap untuk pembaca layar, misalnya “Lihat studi kasus LMS Pijar Aksara”.

## **13\. Metrik keberhasilan**

| Metrik | Cara ukur | Target |
| :---- | :---- | :---- |
| Kualitas teknis | Lighthouse mobile sebelum rilis | 90 atau lebih untuk empat kategori |
| Kejelasan 10 detik | Uji lima detik dengan tiga orang di luar proses pembuatan: tanya siapa pemilik halaman dan apa posisi yang dilamar | Ketiganya menjawab benar |
| Akses ke proyek unggulan | Pengujian manual | Satu klik dari halaman utama |
| Tautan berfungsi | Pemeriksaan semua tautan eksternal | Seluruhnya terbuka tanpa login |
| Penggunaan halaman | Analitik dengan parameter UTM pada tautan di email lamaran | Dicatat sejak hari pertama. Target angka ditetapkan setelah 30 hari, berdasarkan data awal |
| Hasil lamaran | Catatan pribadi: jumlah lamaran yang mencantumkan tautan, jumlah panggilan wawancara | Dibandingkan dengan lamaran sebelum portofolio ada |

## **14\. Milestone dan kriteria selesai**

| Milestone | Hasil | Selesai bila |
| :---- | :---- | :---- |
| M0 Persiapan | Repositori, folder aset, berkas konten terisi, PRD dan design system di /docs | Semua berkas konten valid dan seluruh tautan proyek sudah dicek |
| M1 Fondasi | Token design system, font, tema terang dan gelap, layout dasar, navbar, footer | Tidak ada warna atau ukuran yang ditulis di luar token |
| M2 Bagian atas halaman | Hero, Tentang, angka ringkas | Terbaca baik di 360 px dan 1440 px, kontras memenuhi 4,5:1 |
| M3 Proyek | Daftar isi proyek, unggulan, grid dengan filter, halaman studi kasus | Delapan studi kasus tampil dari data, tiga status data (memuat, kosong, gagal) teruji |
| M4 Pelengkap | Pengalaman, skill, pelatihan, kontak, unduh CV | Isi sesuai CV, tombol unduh membuka PDF terbaru |
| M5 Rilis | Aksesibilitas, SEO, performa, Open Graph, deploy Netlify | Target bagian 10 tercapai dan tautan publik berjalan |

### **User story utama (Given-When-Then)**

> 1. **Melihat identitas.** Diberikan rekruter membuka halaman di ponsel, ketika halaman selesai dimuat, maka nama, headline, foto, dan tombol “Lihat proyek” dan “Unduh CV” tampak tanpa scroll.  
> 2. **Membuka proyek unggulan.** Diberikan pengunjung berada di halaman utama, ketika ia mengklik kartu LMS Pijar Aksara, maka halaman studi kasus terbuka dengan tautan Web, GitLab, dan Video demo.  
> 3. **Memfilter proyek.** Diberikan grid semua proyek, ketika pengunjung memilih kategori “Proyek Bootcamp”, maka hanya proyek berkategori itu yang tampil dan jumlahnya diumumkan ke pembaca layar.  
> 4. **Gambar gagal dimuat.** Diberikan koneksi lambat, ketika gambar proyek gagal dimuat, maka placeholder dengan teks alternatif tampil dan tata letak tidak bergeser.  
> 5. **Mengunduh CV.** Diberikan pengunjung di halaman mana pun, ketika ia mengklik “Unduh CV”, maka berkas PDF terbaru terunduh atau terbuka di tab baru.

## **15\. Risiko dan pertanyaan terbuka**

### **Risiko**

> * Folder Drive atau papan Canva yang tidak publik membuat tautan tidak bisa dibuka rekruter.  
> * Terlalu banyak proyek dengan bobot sama membuat bukti terkuat tenggelam. Mitigasi: tiga proyek unggulan dan penggabungan sesi Dapur Nia.  
> * Batas token di Antigravity menghentikan pekerjaan di tengah milestone. Mitigasi: satu milestone per sesi dan PRD sebagai acuan tetap.  
> * Kemiripan dengan referensi. Mitigasi: hanya struktur seksi yang dipakai, sedangkan tata letak, teks, dan aset dibuat sendiri.

### **Pertanyaan yang perlu dijawab**

> 1. Posisi atau jenis peran yang paling ingin dilamar, dan apakah CV versi magang adalah versi yang dipakai? iya  
> 2. Tiga proyek unggulan: apakah sesuai asumsi (LMS Pijar Aksara, skripsi, Dapur Nia)? iya, nanati aku tambah juga hasil beberapa hobby desain ku  
> 3. Preferensi visual: tiga kata mood, warna yang disukai atau dihindari, mode terang, gelap, atau keduanya, bagian dari referensi yang paling disukai.  
> 4. Jumlah dan gaya foto, dan apakah foto diambil baru. iya  
> 5. Bahasa situs: Indonesia saja, atau Indonesia dan Inggris. indonesia saja  
> 6. Stack: Next.js ekspor statis (asumsi) atau HTML, CSS, JavaScript biasa.   
> 7. Domain: memakai subdomain di mihatul.site atau alamat Netlify. netlify  
> 8. Catatan token limit pada proyek Toko Buku: ditampilkan sebagai pelajaran, diubah, atau dihapus. gak usah ada  
> 9. Apakah nomor WhatsApp ditampilkan, dan dalam bentuk apa (tombol tanpa teks nomor, atau teks). icon dan nomor  
> 10. Apakah aplikasi skripsi boleh ditampilkan, dan apakah ada tautan atau video yang dapat dibagikan. gak perlu  
> 11. Peran dan tech stack untuk masing-masing proyek bootcamp, bila berbeda dari yang tertulis di CV.