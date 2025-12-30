---
obsidianUIMode: preview
note_type: theory
judul_materi: How does machine learning approach a problem
sumber:
  - ibm.skillsbuild
date_learned: 2025-12-30T12:43:00
tags:
---
Link Sumber: [How does machine learning approach a problem](https://alm.ibm.com/ibm-skillsbuildadult/trainingId/course:4058918/trainingInstanceId/course:4058918_4630713/en-US)

---
```ad-summary

```

# How does machine learning approach a problem

## Dua cara untuk menyelesaikan masalah dark data

Jika AI tidak bergantung pada instruksi pemrograman untuk bekerja dengan **unstructured data**, bagaimana cara AI melakukannya? **Machine learning** dapat menganalisis **dark data** jauh lebih cepat daripada komputer terprogram. Sebagai contoh, perhatikan masalah pencarian rute melalui lalu lintas kota besar menggunakan sistem navigasi. Ini adalah masalah **dark data** karena penyelesaiannya membutuhkan penanganan peta jalan yang rumit serta variabel yang terus berubah seperti cuaca, kemacetan, dan kecelakaan. Mari kita lihat bagaimana dua sistem berbeda mencoba menyelesaikan masalah ini.

### Komputer Terprogram

![|500](src/18-How%20does%20machine%20learning%20approach%20a%20problem-1.png)

- Peneliti mungkin mengunggah basis data (_database_) lengkap berisi semua kemungkinan rute di kota tersebut ke komputer. Ini adalah kumpulan **structured data** yang sangat besar.
    
- Kemudian mereka harus menambahkan lebih banyak data yang menjelaskan kondisi cuaca dan lalu lintas saat ini. Data ini harus diperbarui setiap beberapa menit untuk seluruh kota!
    
- Lalu mereka menggunakan komputer terprogram untuk mencari di dalam data tersebut sampai menemukan rute dari titik awal ke tujuan. Proyek ini akan membutuhkan sumber daya dan waktu yang sangat besar, jika memang bisa diselesaikan.
    

### AI dengan machine learning

![|500](src/18-How%20does%20machine%20learning%20approach%20a%20problem-2.png)

- AI dengan **machine learning** akan memperlakukan masalah ini seperti memanjat sebuah `tree`. Sistem akan mencoba sebuah rute, seolah-olah mulai dari dasar batang pohon. Saat mencapai sebuah cabang, sistem akan bercabang (`fork`) ke satu arah dan terus melakukannya hingga mencapai jalan buntu atau tujuan yang diinginkan.
    
- Sistem akan melakukan ini berulang kali, lalu membandingkan rute yang berhasil untuk mengidentifikasi rute terpendek. Meskipun pekerjaannya terdengar repetitif, hal ini membutuhkan lebih sedikit sumber daya dan dapat diselesaikan lebih cepat.

## Proses machine learning sangat berbeda

Proses **machine learning** memiliki keuntungan:

- Tidak butuh basis data (_database_) dari semua rute yang memungkinkan. Ia hanya perlu tahu letak tempat-tempat di peta.
    
- Dapat merespons masalah lalu lintas dengan cepat karena tidak perlu menyimpan rute alternatif untuk setiap situasi lalu lintas. Ia mencatat di mana terjadi perlambatan dan menemukan jalan keluar melalui uji coba (_trial and error_).
    
- Bekerja sangat cepat. Sambil mencoba belokan satu per satu, ia dapat menjalankan jutaan kalkulasi kecil.

**Machine learning** memiliki dua keunggulan tambahan:

1. **Machine learning dapat memprediksi.** Mesin dapat menentukan rute mana yang kemungkinan lebih cepat berdasarkan lalu lintas saat ini karena ia membandingkan rute saat membangunnya.
    
2. **Machine learning belajar!** Ia dapat menyadari jika mobil Anda tertunda oleh pengalihan jalan sementara dan menyesuaikan rekomendasinya untuk membantu pengemudi lain.