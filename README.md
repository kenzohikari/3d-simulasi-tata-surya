# Simulasi Interaktif Tata Surya & Galaksi 3D

Simulasi astronomi interaktif berbasis WebGL (**Three.js**) yang memvisualisasikan mekanika orbit Keplerian dari skala Tata Surya hingga struktur Galaksi Bima Sakti secara *real-time*[cite: 35, 37]. Dilengkapi tekstur permukaan dan *shader* atmosfer prosedural, 8 planet utama, 10 planet katai, 34 satelit alami, 4 komet berekor ganda, ribuan objek sabuk asteroid & TNO, serta peta 3D Galaksi Bima Sakti[cite: 35].

🔗 **Live Demo:** https://kenzohikari.github.io/3d-simulasi-tata-surya/

---

## Tiga Mode Referensi Kosmik (`M`)

1. **Mode Heliosentris (Ekliptika 0°):** Tampilan klasik berpusat pada Matahari dengan bidang ekliptika datar untuk mengamati resonansi orbit, inklinasi, gerhana, dan sistem satelit tiap planet[cite: 35].
2. **Mode Heliks Galaktik (Kemiringan 60,2°):** Memvisualisasikan pergerakan Tata Surya yang melaju ~230 km/detik melintasi ruang antarbintang, menarik seluruh 8 planet dalam lintasan pusaran heliks 3D berwarna dengan opsi osilasi vertikal galaktik[cite: 35].
3. **Mode Peta Galaksi Bima Sakti (SBbc):** Simulasi 75.000 bintang yang berotasi diferensial seperti pusaran air dengan gelombang kepadatan 4 lengan spiral utama (*Perseus, Scutum–Centaurus, Sagittarius–Carina, Norma*), *Orion–Cygnus Spur*, lubang hitam supermasif *Sagittarius A\**, gugus bola *Omega Centauri*, serta 7 galaksi satelit (*LMC, SMC, Sagitarius, Sculptor, Draco, Ursa Minor, Fornax*)[cite: 35].

---

## Fitur Utama

* **Matahari & 8 Planet Utama:** *Shader* plasma konvektif beranimasi pada Matahari, peta benua & tutupan awan Bumi dengan hamburan atmosfer *Rayleigh/Fresnel*, pita angin jet zonal beranimasi pada 4 planet raksasa (*Jupiter, Saturnus, Uranus, Neptunus*), *Great Red Spot*, *Great Dark Spot*, siklon kutub Jupiter, heksagon kutub utara Saturnus, serta rotasi diferensial Keplerian pada cincin Saturnus[cite: 35, 37].
* **34 Satelit Alami & Bayangan Gerhana Analitik:** Mencakup Bulan, Phobos, Deimos, 4 satelit Galilea, 7 satelit utama Saturnus (termasuk Titan beratmosfer dan Iapetus dua warna), 5 satelit Uranus, 3 satelit Neptunus (termasuk Triton *retrograde*), serta satelit planet katai—lengkap dengan simulasi bayangan gerhana matahari dan gerhana bulan secara *real-time*[cite: 35].
* **10 Planet Katai & Sistem Cincinnya:** Ceres, Orcus (*Anti-Pluto* + Vanth), Pluto (dengan 5 satelit: Charon, Styx, Nix, Kerberos, Hydra), Salacia (+ Actaea), Haumea (elipsoid triaksial berotasi 3,9 jam + cincin & 2 satelit), Quaoar (sistem cincin ganda di luar batas Roche + Weywot), Makemake (+ MK2), Gonggong (+ Xiangliu), Eris (inklinasi 44° + Dysnomia), dan Sedna[cite: 35, 37].
* **4 Komet Ikonik Berekor Ganda Dinamis:** *1P/Halley* (orbit *retrograde* 162,3°), *C/1995 O1 (Hale-Bopp)* (orbit polar 89,4°), *2P/Encke*, dan *67P/Churyumov–Gerasimenko* (inti berlobus ganda) dengan koma bercahaya serta ekor ion biru dan ekor debu yang memanjang otomatis saat mendekati perihelion[cite: 35].
* **Populasi Sabuk & TNO (`InstancedMesh`):** Simulasi ribuan objek Sabuk Asteroid Utama (termasuk 4 Vesta, 2 Pallas, 3 Juno, 16 Psyche, 10 Hygiea), Trojan Jupiter (L4 & L5), Sabuk Kuiper (termasuk objek kontak-biner Arrokoth), dan Piringan Tersebar (*Scattered Disc*)[cite: 35, 37].
* **12 Rasi Bintang Bola Langit:** Proyeksi koordinat langit nyata (RA/Dec) untuk *Orion, Ursa Major, Cassiopeia, Crux, Scorpius, Cygnus, Leo, Taurus, Canis Major, Lyra, Aquila,* dan *Gemini* yang dapat diklik untuk inspeksi astronomi[cite: 35].
* **Tur Sinematik, Pencarian Cepat & Kalender Kosmik:** Tur kamera otomatis lintas bab (14 bab Tata Surya & 9 bab Bima Sakti), pencarian cepat semua objek langit, 5 *preset* sudut kamera pelacakan, serta penunjuk tanggal dan tahun kosmik yang tersinkronisasi dengan revolusi orbit[cite: 35, 37].
* **Perekam Klip Video Full HD (`V`):** Rekam kanvas 3D langsung tanpa antarmuka HUD dalam format **Layar Penuh**, **16:9 Full HD (`1920×1080`)**, atau **9:16 Vertikal / Reels (`1080×1920`)** pada pilihan **30 FPS** atau **60 FPS**[cite: 35, 37].

---

## Kontrol Navigasi & Pintasan Keyboard

| Aksi | Mouse / Layar Sentuh | Pintasan Keyboard |
| :--- | :--- | :--- |
| **Putar / Geser Kamera** | Klik Kiri (Orbit) • Klik Kanan / 2 Jari (Pan) | `W` `A` `S` `D` / Panah + `Q` `E` (Free Cam) |
| **Zoom Dekat / Jauh** | Scroll Mouse / Cubit 2 Jari | — |
| **Fokus & Lacak Objek** | Klik Objek 3D / Label Nama / Pil Bawah | `1` – `5` (Ubah Sudut Kamera Follow) |
| **Mode Free Cam** | Tombol **Free Cam** (geser bebas 1 jari/klik kiri) | `G` |
| **Ganti Mode Referensi** | Tombol **Heliosentris / Heliks 60° / Bima Sakti** | `M` |
| **Jeda / Lanjutkan Waktu** | Tombol Play/Pause | `Spasi` |
| **Pencarian Cepat Objek** | Tombol **Cari** | `/` |
| **Ikuti / Lepas Tata Surya** | Tombol **Ikuti Tata Surya** (Mode Bima Sakti) | `F` |
| **Zoom Out / Tampilan Penuh** | Tombol **Zoom Out** | `R` |
| **Lepas Fokus / Keluar Rasi** | Tombol **Lepas** / **Exit** | `Esc` |
| **Mode Sinematik (Sembunyi HUD)** | Tombol **Sinematik** | `H` |
| **Mulai / Hentikan Rekam Video** | Tombol **Mulai Rekam** | `V` |
| **Buka Panduan Kontrol** | Tombol `?` | `?` |

---

## Teknologi yang Digunakan

* **Three.js (`v0.165.0`)** — Rendering 3D WebGL, custom GLSL shaders, dan post-processing (`UnrealBloomPass`)[cite: 35]
* **Tailwind CSS** — Tata letak antarmuka HUD responsif bergaya *glassmorphism* (Desktop & Mobile)[cite: 35]
* **MediaRecorder & Canvas Capture API** — Perekaman video langsung dari kanvas WebGL beresolusi Full HD[cite: 35]
