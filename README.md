# Avatar Cam

Aplikasi web untuk merekam video dengan **karakter avatar**, bukan wajah aslimu. Kamera HP/laptop hanya dipakai untuk membaca gerakan wajah. Karakternya ikut menoleh, miring, mengangguk, berkedip, dan membuka mulut. Badannya juga ikut bergeser, miring, dan maju-mundur mengikuti bahumu. Yang terekam hanya karakter, tidak ada video wajahmu.

Semua jalan di browser, gratis, dan tidak ada video yang dikirim ke server.

## Isi repo

| File | Fungsi |
|---|---|
| `index.html` | Seluruh aplikasi (gambar karakter sudah tertanam di dalamnya) |
| `README.md` | Panduan ini |

## Pasang di GitHub Pages

Supaya bisa dibuka dari HP lewat alamat `https://...`. Kamera hanya bisa dipakai di alamat HTTPS seperti ini.

### Cara A: lewat laptop (paling mudah)

1. Buka <https://github.com> dan masuk. Kalau belum punya akun, daftar dulu (gratis).
2. Klik **+** di kanan atas, lalu **New repository**.
3. Isi **Repository name**, misalnya `avatar-cam`. Pilih **Public**, lalu klik **Create repository**.
4. Di halaman repo yang kosong, klik **uploading an existing file**.
5. Seret `index.html` dan `README.md` ke kotak upload. Nama `index.html` harus persis begitu.
6. Tunggu upload selesai, lalu klik **Commit changes**.
7. Buka tab **Settings**, lalu menu **Pages** di sebelah kiri.
8. Di bagian **Build and deployment**, pilih **Source: Deploy from a branch**. Pilih **Branch: main** dan folder **/(root)**, lalu klik **Save**.
9. Tunggu 1 sampai 3 menit. Refresh halaman Pages sampai muncul tulisan *Your site is live at ...*.
10. Alamatnya berbentuk `https://NAMAKAMU.github.io/avatar-cam/`. Buka alamat itu.

### Cara B: langsung dari HP

1. Buka **Chrome** di HP, masuk ke <https://github.com>, lalu login.
2. Ketuk menu **⋮** di kanan atas Chrome dan centang **Situs desktop**. Tanpa ini, tombol upload tidak muncul.
3. Ikuti langkah 2 sampai 10 di Cara A.

Kalau file `index.html` ada di HP, ketuk **choose your files** untuk memilihnya.

## Cara pakai di HP

1. Buka alamat GitHub Pages tadi di **Chrome**. Browser bawaan HP kadang tidak mendukung kamera atau perekaman.
2. Ketuk **Mulai kamera**, lalu **Izinkan** saat diminta akses kamera. Pertama kali butuh internet beberapa detik untuk memuat model pelacak wajah.
3. Taruh HP di tempat yang stabil, setinggi wajah, dengan **kepala sampai dada** terlihat kamera depan. Pencahayaan dari depan memberi hasil paling bagus.
4. Begitu kamera menyala, aplikasi otomatis memulai **kalibrasi**: ada hitung mundur 3 detik, lalu diam sekitar 2 detik. Hadap lurus dan jangan bergerak. Kalau mau mengulang, ketuk **Kalibrasi**.
5. Atur **Ukuran kepala**, **Ukuran karakter**, **Sensitivitas gerakan**, **Latar**, dan **Rasio** (9:16 untuk Shorts/Reels/TikTok).
6. Centang **Ikut rekam suara mikrofon** kalau mau suaranya ikut terekam.
7. Ketuk **Rekam**, bicara seperti biasa, lalu ketuk **Berhenti**.
8. Ketuk **Unduh** di bawah pratinjau hasil. Videonya tersimpan di folder **Download** HP.

Tips:
- Jangan pindah ke aplikasi lain atau mengunci layar saat merekam. Perekaman bisa berhenti.
- Latar **Hijau (chroma key)** berguna kalau mau mengganti latar di CapCut.
- Tombol **Preview kamera** hanya untuk melihat apakah wajahmu terdeteksi. Isinya tidak ikut terekam.
- Menambah ke layar utama: ketuk menu **⋮** di Chrome, lalu **Tambahkan ke layar utama**, supaya terbuka seperti aplikasi.

## Kalau ada masalah

| Masalah | Coba ini |
|---|---|
| Kamera tidak mau menyala | Pastikan alamatnya `https://` dan izin kamera untuk situs ini aktif di pengaturan Chrome. |
| Tulisan "Gagal memuat" saat memulai | Cek internet. Model pelacak wajah diunduh dari internet saat pertama dipakai. |
| Karakter miring atau bergeser padahal kamu diam | Ketuk **Kalibrasi**, hadap lurus, dan jangan bergerak selama pemindaian. |
| Muncul pesan "bahu tidak terlihat" | Mundur sedikit atau turunkan HP sampai kepala dan dada masuk kamera, lalu ketuk **Kalibrasi** lagi. |
| Gerakan kurang terasa atau terlalu berlebihan | Geser slider **Sensitivitas gerakan**. |
| Gerakan patah-patah atau lambat | Tutup aplikasi lain, matikan mode hemat baterai, atau pakai rasio 9:16. |
| Wajah tidak terdeteksi | Tambah cahaya dari depan dan dekatkan wajah ke kamera. |
| Video hasil tidak bisa dibuka di CapCut | Hasil rekaman bisa berformat MP4 atau WebM tergantung versi Chrome. Kalau WebM tidak terbaca, ubah ke MP4 dengan aplikasi konverter video. |
| Perlu memperbarui aplikasi | Ganti `index.html` di GitHub (Add file → Upload files, lalu commit). Tunggu 1 sampai 2 menit, lalu muat ulang halaman. |

## Batasan saat ini

- Senyum, alis, dan arah lirikan mata belum ikut bergerak.
- Saat kepala menoleh jauh (tampak samping), kedipan dan gerak mulut tidak ikut.
- Badan ikut bergeser, miring, dan maju-mundur mengikuti bahu. Lengan dan tangan belum ikut bergerak.
- Belum diuji langsung di HP Poco X7. Kalau ada yang aneh, catat di mana, lalu kabari supaya diperbaiki.
