-- Materi Yang Dipresentasikan --

ReactJS Performance Optimization Techniques :

1. Menjaga Status Komponen Tetap Lokal Jika Perlu
   Pembaruan status dalam komponen induk merender komponen induk dan turunannya. Jadi, untuk memastikan rendering ulang komponen  
   hanya terjadi bila diperlukan, kita dapat mengekstrak bagian kode yang peduli dengan status komponen, menjadikannya lokal untuk bagian
   kode tersebut.
2. Memoizing Komponen React Untuk Mencegah Rendering Yang Tidak Perlu
   Tidak seperti teknik kinerja sebelumnya di mana refactoring kode kami memberi kami peningkatan kinerja, di sini kami menukar
   ruang memori dengan waktu. Jadi, kita hanya boleh memoize komponen jika diperlukan. Memoization adalah strategi optimasi
   yang menyimpan operasi yang di-cache komponen, menyimpan hasilnya dalam memori, dan mengembalikan hasil yang di-cache
   untuk input yang sama.
3. Pemisahan Kode Adalah Teknik Optimasi Penting Lainnya Untuk Aplikasi React
   Secara default, ketika aplikasi React dirender di browser, file "bundel" yang berisi seluruh kode aplikasi dimuat dan disajikan kepada
   pengguna sekaligus. File ini dihasilkan dengan menggabungkan semua file kode yang diperlukan untuk membuat aplikasi web berfungsi.
   Ide bundling berguna karena mengurangi jumlah permintaan HTTP yang dapat ditangani halaman. Namun, seiring pertumbuhan aplikasi,
   ukuran file meningkat, sehingga meningkatkan file bundel.
4. Windowing Atau Daftar Virtualisasi Di React
   Bayangkan kita memiliki aplikasi tempat kita merender beberapa baris item pada sebuah halaman. Baik item yang ditampilkan di viewport
   browser atau tidak, item tersebut dirender di DOM dan dapat memengaruhi kinerja aplikasi kita. Dengan konsep windowing, kita dapat
   merender ke DOM hanya bagian yang terlihat oleh pengguna. Kemudian, saat menggulir, item daftar yang tersisa dirender saat mengganti
   item yang keluar dari viewport. Teknik ini dapat sangat meningkatkan kinerja rendering daftar besar.
5. Memuat Gambar Dengan Lambat Di React
   Untuk mengoptimalkan aplikasi yang terdiri dari beberapa gambar, kita dapat menghindari rendering semua gambar sekaligus untuk
   meningkatkan waktu buka halaman. Dengan lazy loading, kita bisa menunggu sampai setiap gambar akan muncul di viewport
   sebelum kita merendernya di DOM. Mirip dengan konsep windowing yang disebutkan di atas, gambar lazy loading mencegah
   pembuatan node DOM yang tidak perlu, meningkatkan kinerja aplikasi React kami.

Kekurangan ReactJS :

1. Laju Pembangunan Yang Tinggi
   Laju pembangunan yang tinggi memiliki keuntungan dan kerugian. Jika terjadi kerugian, karena lingkungan terus berubah begitu cepat,
   beberapa pengembang merasa tidak nyaman untuk mempelajari kembali cara-cara baru dalam melakukan sesuatu secara teratur.
   Mungkin sulit bagi mereka untuk mengadopsi semua perubahan ini dengan semua pembaruan berkelanjutan.
   Mereka perlu selalu diperbarui dengan keterampilan mereka dan mempelajari cara-cara baru dalam melakukan sesuatu.
2. Dokumentasi Yang Buruk
   Ini adalah kekurangan lain yang umum terjadi pada teknologi yang terus diperbarui. Teknologi React memperbarui dan mempercepat
   dengan sangat cepat sehingga tidak ada waktu untuk membuat dokumentasi yang tepat. Untuk mengatasinya, pengembang menulis
   instruksi mereka sendiri dengan mengembangkan rilis baru dan alat dalam proyek mereka saat ini.
3. View Bagian
   ReactJS hanya mencakup Lapisan UI aplikasi dan tidak ada yang lain. Jadi, Anda masih perlu memilih beberapa teknologi lain
   untuk mendapatkan satu set perkakas lengkap untuk pengembangan dalam proyek tersebut.
4. JSX Sebagai Pembatas
   ReactJS menggunakan JSX. Ini adalah ekstensi sintaks yang memungkinkan HTML dengan JavaScript dicampur bersama.
   Pendekatan ini memiliki keuntungan tersendiri, tetapi beberapa anggota komunitas pengembangan menganggap sebagai
   penghalang terutama bagi pengembang baru. Pengembang mengeluh tentang kompleksitasnya dalam kurva pembelajaran.

Kelebihan ReactJS :

1. JSX
   JSX merupakan singkatan dari Javascript Syntax XML. Adanya JSX memungkinkan untuk menuliskan HTML didalam Javascript,
   sehingga JSX dapat menyederhanakan seluruh proses penulisan komponen website dan aspek HTML.
2. Javascript Library
   ReactJS menawarkan pustaka Javascript yang sangat kaya, sehingga dapat memberikan lebih banyak fleksibilitas kepada
   para pengembang untuk memilih seperti yang mereka inginkan.
3. Reusable Components
   Components merupakan fitur yang menjadi dasar dari Framework ReactJS. Setiap Components memiliki logikanya sendiri
   dan dapat digunakan kembali dimana pun ketika membutuhkannya.
4. SEO Friendly
   SEO merupakan singkatan dari Search Engine Optimization. Framework ReactJS sangat menonjol terhadap SEO karena
   ReactJS dijalankan pada Server dan Virtual DOM yang akan dikembalikan kepada browser sebagai halaman biasa.
5. Virtual DOM
   Pada ReactJS diciptakan sebuah struktur cache data didalam memori untuk menghitung berapa banyak perubahan dibuat
   yang selanjutnya akan diperbarui oleh browser.

## License

MIT licensed

Copyright (C) 2011-2021 Hakim El Hattab, https://hakim.se
