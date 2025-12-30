---
obsidianUIMode: preview
note_type: theory
judul_materi: Transformers
sumber:
  - ibm.skillsbuild
date_learned: 2025-12-30T14:48:00
tags:
---
Link Sumber: [Transformers](https://alm.ibm.com/ibm-skillsbuildadult/trainingId/course:4058859/trainingInstanceId/course:4058859_4630654/en-US)

---
```ad-summary

```

# Transformers

Setelah mempelajari apa itu _foundation models_ dan _large language models_, kini saatnya memahami lebih dalam cara kerjanya. Mari kita lihat bagaimana **Transformer** merevolusi tugas pemrosesan bahasa alami (NLP).

**Transformer** merujuk pada jenis arsitektur jaringan saraf tertentu yang dirancang untuk memproses data berurutan, seperti urutan bahasa alami.

Arsitektur ini pertama kali diperkenalkan dalam makalah "Attention Is All You Need" oleh Vaswani dkk. pada tahun 2017 dan sejak itu menjadi fondasi bagi berbagai model NLP mutakhir. Sebelum munculnya arsitektur Transformer, metode tradisional mengandalkan _recurrent neural networks_ (RNN) dan _convolutional neural networks_ (CNN).

**Recurrent Neural Network (RNN)** adalah kelas jaringan saraf yang menyertakan koneksi berbobot di dalam satu lapisan (berbeda dengan jaringan _feed-forward_ tradisional, di mana koneksi hanya berlanjut ke lapisan berikutnya).

Skenario singkat di atas merangkum bagaimana RNN memproses informasi dari waktu ke waktu, belajar dari input, dan membuat prediksi berdasarkan memorinya. Dengan meninjau dan menyesuaikan strategi secara konsisten berdasarkan umpan balik, model menjadi lebih siap, serupa dengan bagaimana RNN menyempurnakan prediksinya melalui pemrosesan lebih banyak data.

RNN umumnya digunakan untuk NLP dan pengenalan ucapan, sedangkan CNN lebih sering digunakan untuk tugas klasifikasi dan visi komputer. **Convolutional Neural Network (CNN)** adalah ekstensi dari jaringan saraf tiruan (ANN) dan dominan digunakan untuk tugas berbasis pengenalan gambar.

Transformer menggunakan teknik matematika modern yang disebut **attention** atau **self-attention**. _Self-attention_ memungkinkan model memilih dan menentukan seberapa besar nilai setiap kata atau token dalam sebuah kalimat saat memprosesnya (saat melakukan _encoding_ atau _decoding_).

Hal ini membuatnya sangat ahli dalam menangkap hubungan antar kata, berbeda dengan RNN yang bergantung pada pemrosesan berurutan. Dengan cara ini, model dapat menangkap ketergantungan jarak jauh dan informasi kontekstual dalam urutan tersebut, yang sangat penting dalam tugas-tugas NLP.

---

Model transformer terdiri dari dua bagian utama: **encoder** dan **decoder**. _Encoder_ memproses urutan input dan menghasilkan urutan status tersembunyi (_hidden states_), sedangkan _decoder_ mengambil urutan ini sebagai input dan menghasilkan urutan output. Dengan melatih model pada korpus data yang besar, _encoder_ belajar untuk mengodekan teks dengan cara yang menangkap informasi dan pola penting, sementara _decoder_ belajar untuk menghasilkan teks output yang benar secara semantik dan tata bahasa.

Selanjutnya, kita akan melihat lebih dekat cara kerja _encoder_ dan _decoder_.