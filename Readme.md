🚀 Leadership Ala Gen Z — Presentasi Web Interaktif

Presentasi tentang kepemimpinan untuk generasi muda, dibuat sebagai halaman web. Awalnya ini file PowerPoint biasa. Sekarang bisa dibuka di browser, dengan transisi antar-slide, animasi bertahap, dan beberapa bagian yang bisa diklik langsung saat presentasi.

Seluruh proyek hanya satu file HTML. Tidak perlu instalasi, tidak perlu server, dan tidak ada proses build. Kamu cukup membukanya di browser.

✨ Fitur

Tampilan dan animasi

Transisi antar-slide berupa geser, blur, dan zoom. Arahnya mengikuti maju atau mundur, jadi terasa seperti berpindah halaman sungguhan.
Isi tiap slide muncul satu per satu, tidak langsung semuanya.
Latar berupa bola gradien yang melayang pelan dan ikut bergeser mengikuti kursor.
Kartu terangkat saat di-hover, ikon bergerak naik-turun, dan banner "LEADERSHIP ≠ JABATAN" berpendar.
Slide penutup menampilkan confetti.
Mendukung prefers-reduced-motion. Pengguna yang mematikan animasi di perangkatnya tidak akan dipaksa melihat gerakan.

Interaktif

Slide 4 (Leader vs Boss): tiga tombol (Boss, Bandingkan, Leader) untuk menyorot salah satu sisi perbandingan.
Slide 6 (4 langkah Problem Solving): STOP → THINK → COMMUNICATE → SOLVE menyala berurutan otomatis. Tiap kartu juga bisa diklik manual.

Navigasi

Progress bar di bagian atas dan titik indikator di bawah.
Link langsung ke slide tertentu lewat hash, misalnya ...html#4 langsung membuka slide 4.
Responsif, jadi nyaman dibuka di laptop maupun HP.
🎮 Cara Mengoperasikan
Aksi Cara
Slide berikutnya →, ↓, Spasi, Page Down, atau tombol →
Slide sebelumnya ←, ↑, Page Up, atau tombol ←
Ke slide pertama / terakhir Home / End
Layar penuh F atau tombol ⛶
Lompat ke slide tertentu Klik titik indikator di bawah
Di HP / tablet Geser (swipe) kiri atau kanan
▶️ Cara Menjalankan
Unduh file leadership-ala-gen-z.html.
Klik dua kali untuk membukanya di browser (Chrome, Edge, Firefox, atau Safari).
Tekan F untuk layar penuh, lalu presentasikan.

Font memakai Google Fonts, jadi sebaiknya sambungan internet aktif saat pertama kali dibuka. Kalau offline, tampilan tetap berjalan dengan font bawaan sistem, hanya saja hurufnya sedikit berbeda.

🗂️ Daftar Slide
No Slide Isi singkat
01 Latar Belakang Mengapa leadership penting, dan kenapa bukan soal jabatan
02 Perkenalan Siapa pembicara, lengkap dengan foto
03 Pembahasan Apa itu leadership: memengaruhi, mengarahkan, menginspirasi, berkomunikasi
04 Perbandingan Leader vs Boss (interaktif)
05 Strategi Memimpin diri sendiri dan memimpin tim
06 Problem Solving 4 langkah saat masalah terjadi (animasi berurutan)
07 Era Digital Leadership di era teknologi dan AI
08 Penutup Pesan akhir, ucapan terima kasih, dan confetti
🛠️ Cara Mengubah Isi

Semuanya ada di satu file, jadi cukup buka leadership-ala-gen-z.html dengan editor teks apa saja (misalnya VS Code).

Mengubah teks. Cari kata yang ingin diganti. Setiap slide adalah satu blok <section class="slide">...</section> yang isinya mudah dibaca.

Mengubah warna. Semua warna utama dikumpulkan di bagian atas CSS, pada :root:

css
:root{
--bg:#14080b; /_ latar belakang _/
--acc:#f43f5e; /_ warna aksen utama (rose) _/
--acc2:#fb923c; /_ aksen kedua (oranye) _/
--wine:#671c2a; /_ maroon untuk kartu dan bola latar _/
}

Mengubah urutan animasi. Elemen yang muncul bertahap punya atribut style="--i:N". Semakin besar angkanya, semakin lambat elemen itu muncul. Tukar angkanya untuk mengatur ulang urutan.

Menambah slide. Salin satu blok <section class="slide" data-k="09 / Judul">...</section>, ubah isinya, lalu tempel sebelum penutup </main>. Titik indikator dan progress bar akan menyesuaikan sendiri.

Mengganti foto atau logo. Gambar disematkan langsung ke dalam HTML dalam format base64 (src="data:image/jpeg;base64,..."), sehingga file tetap mandiri dan bisa dikirim satu-satunya. Untuk menggantinya, ubah gambar barunya jadi base64 lalu tempel di atribut src. Atau, kalau lebih mudah, taruh gambar di folder yang sama dan tulis src="foto.jpg". Dengan cara kedua, kirimkan juga file gambarnya bersama HTML.

🧱 Teknologi
HTML, CSS, dan JavaScript murni (vanilla), tanpa framework dan tanpa library tambahan.
Font Plus Jakarta Sans dari Google Fonts.
Animasi memakai CSS transition dan @keyframes. JavaScript hanya mengatur navigasi, tombol interaktif, dan confetti.
📁 Struktur Proyek
.
├── leadership-ala-gen-z.html # seluruh presentasi (HTML + CSS + JS + gambar)
└── README.md # dokumentasi ini
👤 Pembuat

Muhammad Rezky Ayyriel Ramadhan Mahasiswa Informatika, Universitas Teknologi Digital Indonesia (UTDI) Yogyakarta

Konten materi dan desain awal berasal dari presentasi PowerPoint Leadership Ala Gen Z, yang kemudian diubah menjadi versi web interaktif ini.

"Leadership bukan tentang menjadi yang paling tinggi. Leadership adalah tentang membawa orang lain untuk maju."
