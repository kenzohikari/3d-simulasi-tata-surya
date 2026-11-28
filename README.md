# 🌌 Simulasi Interaktif Tata Surya & Galaksi 3D

![Three.js](https://img.shields.io/badge/Three.js-v0.165.0-0a84ff?style=flat-square&logo=threedotjs&logoColor=white)
![WebGL2](https://img.shields.io/badge/WebGL2-8x_MSAA_%2B_SSAA_2x_%2B_Bloom-38bdf8?style=flat-square)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-Liquid_Glass_HUD-0ea5e9?style=flat-square&logo=tailwindcss&logoColor=white)
![Bilingual](https://img.shields.io/badge/Language-ID%20%2F%20EN-10b981?style=flat-square)
![Video Recorder](https://img.shields.io/badge/Recorder-WebCodecs%20MP4-f43f5e?style=flat-square)

Simulasi astronomi interaktif berbasis WebGL (**Three.js**) yang memvisualisasikan mekanika orbit Keplerian dari skala Tata Surya hingga struktur Galaksi Bima Sakti secara *real-time* dalam dua bahasa (**Indonesia / English**). Dilengkapi tekstur permukaan dan *shader* atmosfer prosedural, Bumi hybrid vektor dengan awan siklon & aurora, 8 planet utama, 10 planet katai, 35 satelit alami, 4 komet berekor ganda, 4 wahana antariksa ikonik, ribuan objek sabuk asteroid & TNO, serta peta 3D Galaksi Bima Sakti.

🔗 **Live Demo:** https://kenzohikari.github.io/3d-simulasi-tata-surya/

> [!TIP]
> Pilih planet mana saja lalu tekan **`6`** (atau klik **Atmosfer**) untuk mengintip lengkung cakrawala & atmosfer dari orbit rendah, klik ganda (*double click/tap*) pada objek atau ruang angkasa untuk *zoom* cerdas, atau tekan **`H`** untuk masuk ke **Mode Sinematik** tanpa HUD.

---

## 🚀 Tiga Mode Referensi Kosmik (`M`)

1. **☀️ Mode Heliosentris (Ekliptika 0°):** Tampilan klasik berpusat pada Matahari dengan bidang ekliptika datar untuk mengamati resonansi orbit, inklinasi, rotasi sideris maupun *retrograde*, gerhana, dan sistem satelit tiap planet.
2. **🌀 Mode Heliks Galaktik (Kemiringan 60,2°):** Memvisualisasikan pergerakan Tata Surya yang melaju ~230 km/detik melintasi ruang antarbintang, menarik seluruh 8 planet dalam lintasan pusaran heliks 3D berwarna dengan opsi osilasi vertikal galaktik.
3. **🌌 Mode Peta Galaksi Bima Sakti (SBbc):** Simulasi 75.000 bintang yang berotasi diferensial seperti pusaran air dengan gelombang kepadatan 4 lengan spiral utama (*Perseus, Scutum-Centaurus, Sagittarius-Carina, Norma*), *Orion-Cygnus Spur*, lubang hitam supermasif *Sagittarius A\**, gugus bola *Omega Centauri*, serta 7 galaksi satelit (*LMC, SMC, Sagitarius, Sculptor, Draco, Ursa Minor, Fornax*) dengan kontrol tampil/sembunyi terpisah.

---

## ✨ Fitur Utama

* **🌐 Dukungan Dwibahasa Real-Time (`ID / EN`):** Pengalih bahasa instan antara **Bahasa Indonesia** dan **English** untuk seluruh antarmuka HUD, panel telemetri, 70+ data astrofisika objek & satelit, 15 entitas galaksi, 12 rasi bintang, narasi tur sinematik, hingga pencarian cepat, dengan penyimpanan preferensi otomatis di `localStorage`.
* **🔍 Anti-Aliasing Bertingkat (`8× MSAA`, `Ultra SSAA 2×` & `GLSL fwidth`):** Menggunakan `8× MSAA` default yang adaptif terhadap kemampuan GPU, **toggle opsional `Ultra SSAA (2×)`** khusus desktop (internal hingga 4K dengan *4-tap RGSS downsample pass* gamma-akurat), *fallback* `SMAAPass` untuk browser non-MSAA, serta *in-shader* `fwidth()` AA agar cincin Saturnus, prominensa, dan fotosfer Matahari bebas *shimmer* maupun *Moiré*.
* **🎨 Tema Warna Objek Terpadu & Putar Bebas 360°:** Setiap objek Tata Surya, 5 asteroid utama (dengan Trojan tetap hijau), komet, wahana, 12 rasi bintang, dan entitas Bima Sakti memiliki warna label, bingkai, sorotan saat dipilih, dan garis orbit unik yang serasi, dilengkapi **toggle Putar Objek Bebas 360°** di panel Telemetri untuk inspeksi penuh seluruh permukaan.
* **🌍 Bumi Detail Hybrid (Vektor + Shader 3D):** Peta benua & garis pantai presisi berbasis TopoJSON (`countries-110m`, asinkron dengan *fallback* prosedural saat *offline*) lengkap dengan **toggle Batas Negara & Pantai (Vektor)** di panel Telemetri, siklus siang-malam dengan pita senja terminator, lampu kota keemasan, pantulan *sun-glint* samudra, **awan *3D spherical noise* dengan 4 cekungan siklon tropis musiman di samudra nyata**, serta **Aurora Borealis & Australis** di kutub berbasis LOD jarak kamera agar tetap ringan.
* **☀️ Matahari & 7 Planet Utama Lainnya:** *Shader* plasma konvektif beranimasi dengan kemiringan sumbu 7,25° pada Matahari dan korona bola analitik bebas *flicker*, fitur geologi Merkurius (*Caloris Basin*, dataran *Borealis*, tebing *Rupes*, & kawah bercahaya), pita angin jet zonal beranimasi pada 4 planet raksasa (*Jupiter, Saturnus, Uranus, Neptunus*), *Great Red Spot*, *Great Dark Spot*, siklon kutub Jupiter, heksagon kutub utara Saturnus, serta rotasi diferensial Keplerian pada cincin Saturnus.
* **🌕 35 Satelit Alami & Bayangan Gerhana Analitik:** Mencakup Bulan (*lunar maria* & sinar kawah Tycho/Copernicus), Phobos, Deimos, 4 satelit Galilea, 7 satelit utama Saturnus (termasuk Titan beratmosfer dan Iapetus dua warna), 5 satelit Uranus, 3 satelit Neptunus (termasuk Triton *retrograde*), serta satelit planet katai dengan diferensiasi fitur permukaan es (busur tektonik, *coronae* Miranda, rekonstruksi triaksial Hiʻiaka), bidang orbit ekuatorial, penguncian pasang surut (*tidal locking*), dan bayangan gerhana *real-time*.
* **❄️ 10 Planet Katai & Sistem Cincinnya:** Ceres, Orcus (*Anti-Pluto* + Vanth), Pluto (dengan 5 satelit: Charon, Styx, Nix, Kerberos, Hydra), Salacia (+ Actaea), Haumea (elipsoid triaksial berotasi 3,9 jam + cincin & 2 satelit), Quaoar (sistem cincin ganda di luar batas Roche + Weywot), Makemake (+ MK2), Gonggong (+ Xiangliu), Eris (inklinasi 44° + Dysnomia), dan Sedna.
* **☄️ 4 Komet Ikonik Berekor Ganda Dinamis:** *1P/Halley* (orbit *retrograde* 162,3°), *C/1995 O1 (Hale-Bopp)* (orbit polar 89,4°), *2P/Encke*, dan *67P/Churyumov-Gerasimenko* (inti berlobus ganda) dengan koma bercahaya serta ekor ion biru dan ekor debu yang memanjang otomatis saat mendekati perihelion.
* **🛰️ 4 Wahana Antariksa Ikonik:** *James Webb Space Telescope (JWST)* di titik Lagrange L2 Bumi, *Parker Solar Probe* yang menembus korona Matahari, serta *Voyager 1* (~173 SA / 1 hari cahaya dari Bumi) dan *Voyager 2* (~144,5 SA) pada lintasan pelarian hiperbolik antarbintang.
* **🪨 Populasi Sabuk & TNO (`InstancedMesh` Halus):** Simulasi ribuan objek Sabuk Asteroid Utama (termasuk 4 Vesta, 2 Pallas, 3 Juno, 16 Psyche, 10 Hygiea), Trojan Jupiter (L4 & L5), Sabuk Kuiper (termasuk objek kontak-biner Arrokoth), dan *Scattered Disc* dengan geometri terindeks *smooth normals* yang tetap ringan di GPU desktop maupun *mobile*.
* **✨ 12 Rasi Bintang Bola Langit:** Proyeksi koordinat langit nyata (RA/Dec) untuk *Orion, Ursa Major, Cassiopeia, Crux, Scorpius, Cygnus, Leo, Taurus, Canis Major, Lyra, Aquila,* dan *Gemini* dengan warna khas tiap rasi yang dapat diklik untuk inspeksi astronomi beserta navigasi `Prev / Next / Exit`.
* **⏱️ Sinkronisasi LIVE Real-Time Seamless, Tur Sinematik & Pencarian Cepat:** Tombol **LIVE (`REAL RATE`)** meluncurkan ke-8 planet (bujur J2000), fase Bulan, dan rotasi siang-malam Bumi (UTC) ke posisi langit saat ini secara mulus, disertai tur kamera otomatis lintas bab, pencarian cepat semua objek langit, **6 *preset* sudut kamera pelacakan** (termasuk **Atmosfer** orbit rendah), dan *arc jog-shuttle* waktu.
* **🎬 Perekam Klip Video Full HD (`V`):** Rekam kanvas 3D langsung tanpa HUD maupun garis orbit dalam format **Layar Penuh**, **16:9 Full HD (`1920×1080`)**, atau **9:16 Vertikal / Reels (`1080×1920`)** pada pilihan **30 FPS** atau **60 FPS**.

---

## 🎮 Kontrol Navigasi & Pintasan Keyboard

| Aksi | Mouse / Layar Sentuh | Pintasan Keyboard |
| :--- | :--- | :--- |
| **Putar Kamera (Orbit)** | Klik Kiri / Geser 1 Jari | - |
| **Geser Bebas (Pan)** | Klik Kanan • `Shift`/`Spasi` + Klik Kiri • Klik Tengah • 2 Jari | `W` `A` `S` `D` / Panah + `Q` `E` (+ `Shift` 2,5×) |
| **Zoom Dekat / Jauh** | Scroll Mouse • Cubit 2 Jari • **Double Klik / Double Tap** | `+` / `-` |
| **Fokus & Lacak Objek** | Klik Objek 3D / Label Nama / Pil Bawah | `1` - `6` (Ubah Sudut Kamera Follow & Atmosfer) |
| **Mode Free Cam** | Tombol **Free Cam** (geser bebas 1 jari/klik kiri) | `G` |
| **Pusatkan Tanpa Reset Zoom** | - | `C` / `Home` |
| **Ganti Mode Referensi** | Tombol **Heliosentris / Heliks 60° / Bima Sakti** | `M` |
| **Jeda / Lanjutkan Waktu** | Tombol Play/Pause | `Spasi` |
| **Pencarian Cepat Objek** | Tombol **Cari / Search** | `/` |
| **Ikuti / Lepas Tata Surya** | Tombol **Ikuti Tata Surya** (Mode Bima Sakti) | `F` |
| **Zoom Out / Tampilan Penuh** | Tombol **Zoom Out** | `R` |
| **Lepas Fokus / Keluar Rasi** | Tombol **Release** / **Exit** | `Esc` |
| **Mode Sinematik (Sembunyi HUD)** | Tombol **Sinematik / Cinematic** | `H` |
| **Mulai / Hentikan Rekam Video** | Tombol **REC** -> **Mulai Rekam** | `V` |
| **Layar Penuh (Fullscreen)** | Tombol **Layar Penuh / Fullscreen** | `L` |
| **Ganti Bahasa (`ID / EN`)** | Tombol **`ID` / `EN`** di pojok kanan atas | - |
| **Buka Panduan Kontrol** | Tombol `?` | `?` |

---

## 🛠️ Teknologi yang Digunakan

* **Three.js (`v0.165.0`)**: Rendering 3D WebGL2, *custom GLSL shaders*, `InstancedMesh`, *depth-buffer* dinamis *anti-flicker*, LOD berbasis jarak kamera, serta post-processing **`8× MSAA` + `Ultra SSAA (2×)` RGSS + `GLSL fwidth` AA + `SMAAPass` + `UnrealBloomPass`**
* **TopoJSON (`world-atlas@2/countries-110m`)**: Data batas negara & garis pantai Bumi dengan decoder *zero-dependency* dan *fallback* prosedural
* **Tailwind CSS**: Tata letak antarmuka HUD responsif bergaya *Liquid Glass* (Desktop, Mobile Portrait & Landscape)
* **WebCodecs (`VideoEncoder` + `mp4-muxer`) & `MediaRecorder`**: Perekaman video MP4 langsung dari kanvas WebGL beresolusi Full HD
