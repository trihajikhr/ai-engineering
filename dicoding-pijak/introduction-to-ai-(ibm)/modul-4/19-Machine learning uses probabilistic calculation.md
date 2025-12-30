---
obsidianUIMode: preview
note_type: theory
judul_materi: Machine learning uses probabilistic calculation
sumber:
  - ibm.skillsbuild
date_learned: 2025-12-30T12:53:00
tags:
---
Link Sumber: [Machine learning uses probabilistic calculation](https://alm.ibm.com/ibm-skillsbuildadult/trainingId/course:4058918/trainingInstanceId/course:4058918_4630713/en-US)

---
```ad-summary

```

# Machine learning uses probabilistic calculation

![|500](src/19-Machine%20learning%20uses%20probabilistic%20calculation-1.png)

Ada dua cara lain untuk membedakan sistem klasik dan _machine learning_. Satu bersifat **deterministik** dan yang lainnya bersifat **probabilistik**.

Mari kita pelajari arti kedua kata tersebut.

Dalam sistem **deterministik** (deterministic), harus ada struktur rute yang ditentukan sebelumnya dalam jumlah besar—basis data (_database_) raksasa berisi berbagai kemungkinan tempat mesin memilih. Jika rute tertentu menuju ke tujuan, maka mesin menandainya sebagai "YA". Jika tidak, mesin menandainya sebagai "TIDAK". Ini pada dasarnya adalah pemikiran biner: hidup atau mati, ya atau tidak. Inilah esensi dari sebuah program komputer. Jawabannya adalah benar (_true_) atau salah (_false_), bukan nilai kepercayaan.

_Machine learning_ bersifat **probabilistik** (probabilistic). Ia tidak pernah mengatakan "YA" atau "TIDAK". _Machine learning_ bersifat analog (seperti gelombang yang naik turun secara bertahap) daripada biner (seperti panah yang menunjuk ke atas dan ke bawah). _Machine learning_ menyusun setiap rute yang memungkinkan ke tujuan dan membandingkannya secara _real time_, termasuk semua variabel seperti perubahan lalu lintas. Jadi, sistem _machine learning_ tidak mengatakan, "Ini adalah rute tercepat." Ia akan mengatakan sesuatu seperti, "Saya memiliki tingkat keyakinan 84% bahwa rute ini akan mengantar Anda sampai di sana dalam waktu tersingkat." Anda mungkin pernah melihat ini saat menggunakan sistem navigasi GPS modern yang menawarkan dua atau tiga pilihan beserta estimasi waktu.

### Penjelasan Lebih Lanjut

Seperti yang telah Anda pelajari, GPS menawarkan berbagai rute untuk dipilih. **Machine learning** memberikan ruang bagi manusia untuk membuat keputusan akhir. Anda, atau seorang ahli, dapat memilih rute mana yang akan diambil berdasarkan hasil yang mungkin terjadi dan pengalaman pribadi.

Pertimbangkan bagaimana sistem **machine learning** bekerja dengan pertanyaan medis sebelumnya. Saat seorang dokter mempertimbangkan cara merawat pasien kanker, AI menyerap seluruh catatan medis Anda ditambah setiap makalah penelitian tentang kanker tersebut yang diterbitkan dalam beberapa tahun terakhir. Hal ini hanya memakan waktu beberapa detik. Namun, AI tidak mengatakan, "Lakukan ini" atau "Lakukan itu". Itu akan menjadi solusi deterministik yang menyingkirkan dokter dan pasien dari keputusan tersebut.

Sebaliknya, AI memberikan pernyataan probabilistik seperti, "Ada kemungkinan 92% bahwa perawatan ini akan berhasil, dan kemungkinan 87% bahwa perawatan lain ini akan berhasil. Berikut adalah hal-hal yang terlibat dalam menjalankan setiap opsi perawatan." Kini dokter dapat berkonsultasi dengan Anda dan bersama-sama membuat pilihan. Dengan kata lain, AI, dokter, dan Anda telah membentuk kemitraan di mana mesin memprediksi, tetapi manusia yang menilai!

### Jika machine learning hanya menawarkan probabilitas, siapa yang membuat keputusan akhir?

Ini bisa menjadi pertanyaan antara hidup dan mati. Bayangkan Anda memiliki penyakit serius dan dokter memberikan pilihan. Apakah Anda ingin dokter Anda yang meresepkan pengobatan, atau Anda menginginkan pengobatan yang menurut sistem _machine learning_ paling mungkin berhasil?

### Apakah akal sehat masuk akal?

![|500](src/19-Machine%20learning%20uses%20probabilistic%20calculation-2.png)

Ternyata dalam berbagai bidang, mulai dari kedokteran dan pendidikan hingga studi sosial dan pemerintahan, keputusan terbaik dibuat dengan menggunakan keseimbangan antara kekuatan manusia dan mesin. Namun ingat, ada kemampuan lain yang sulit dipahami tetapi vital yang juga harus dipertimbangkan: akal sehat (_common sense_).

Akal sehat mengandalkan banyak generalisasi kompleks yang bercampur dengan rasa kasih sayang dan abstraksi. Saat ini, hanya manusia yang dapat menggunakan akal sehat dengan baik. Masalahnya, akal sehat sering kali tercemar oleh bias yang dapat mendistorsi penilaian Anda. Sistem AI dapat menyeimbangkan hal ini. Selama sistem AI disediakan dan dilatih dengan data yang tidak bias, mereka dapat memberikan rekomendasi yang bebas dari bias. Kemitraan antara manusia dan mesin dapat menghasilkan keputusan yang bijaksana.