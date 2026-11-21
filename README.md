# Simulasi 3D Tata Surya & Objek Trans-Neptunus (TNO)

Simulasi interaktif 3D Tata Surya berbasis WebGL (**Three.js**) yang mencakup Matahari, 8 planet utama beserta satelit alaminya, Sabuk Asteroid, Trojan Jupiter (L4 & L5), Sabuk Kuiper, Scattered Disc, serta 10 planet katai yang telah ditemukan.

🔗 **Live Demo:** https://kenzohikari.github.io/3d-simulasi-tata-surya/

## Fitur Utama

* **Matahari & 8 Planet Utama:** Shader plasma animasi dengan efek *bloom*, kemiringan sumbu rotasi (*axial tilt*), orientasi orbit 3D (*ascending node* $\Omega$), sistem cincin Saturnus (dengan bayangan cincin-planet analitik) dan Uranus.
* **Satelit Alami & Cincin Planet Katai:** Mencakup satelit utama tiap planet hingga bulan dan sistem cincin milik Pluto, Haumea, dan Quaoar.
* **Populasi Sabuk & TNO:** Ribuan objek Sabuk Asteroid Utama, Trojan Jupiter, Sabuk Kuiper, dan Scattered Disc berbasis `InstancedMesh`.
* **10 Planet Katai:** Ceres, Orcus, Pluto, Salacia, Haumea, Quaoar, Makemake, Gonggong, Eris, dan Sedna.
* **Mode Tur Sinematik & Telemetri:** Kamera pelacak otomatis, filter kategori navigasi, dan panel data astrofisika tiap objek.
* **Perekam Klip Video Full HD:** Rekam kanvas 3D langsung dalam resolusi **Full HD 16:9 (`1920×1080`)**, **9:16 Vertikal / Reels (`1080×1920`)**, atau ukuran layar dengan pilihan **30 & 60 FPS** tanpa antarmuka HUD.

## Kontrol Navigasi

* **Klik Kiri + Geser:** Putar sudut pandang kamera.
* **Scroll Mouse:** Perbesar / perkecil (*zoom*).
* **Klik Objek / Tab Bawah:** Fokus dan lacak benda langit secara *real-time*.
* **Tombol `Spasi`:** Jeda / lanjutkan simulasi waktu.
* **Tombol `H`:** Sembunyikan antarmuka untuk Mode Sinematik penuh.
* **Tombol `V`:** Mulai / hentikan perekaman klip video.
* **Tombol `R`:** Kembalikan kamera ke tampilan penuh Tata Surya.
