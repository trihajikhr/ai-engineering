---
obsidianUIMode: preview
note_type: theory
judul_materi: Foundation models
sumber:
  - ibm.skillsbuild
date_learned: 2025-12-30T14:27:00
tags:
---
Link Sumber: [Foundation models](https://alm.ibm.com/ibm-skillsbuildadult/trainingId/course:4058859/trainingInstanceId/course:4058859_4630654/en-US)

---
```ad-summary

```

# Foundation models

Dalam lanskap kecerdasan buatan saat ini, istilah "**foundation model**" sering digunakan secara bergantian dengan "**large language model**" (LLM). Hal ini karena model bahasa adalah contoh paling jelas dari sistem dengan kemampuan luas yang dapat disesuaikan untuk berbagai aplikasi.

Berikut adalah poin-poin penting untuk memahaminya:

- **Foundation Models:** Adalah model bahasa yang telah dilatih sebelumnya (_pre-trained_) dan berfungsi sebagai dasar untuk berbagai tugas pemahaman dan pembuatan bahasa di tahap selanjutnya.
    
- **Pre-training:** Model seperti BERT atau GPT dilatih pada kumpulan teks yang sangat besar sehingga memiliki pemahaman bahasa yang bersifat umum.
    
- **Downstream Tasks:** Ini adalah proses mengambil model yang sudah dilatih tersebut, lalu menyetelnya (_fine-tuning_) untuk aplikasi NLP (pemrosesan bahasa alami) yang spesifik.
    

Cara Kerjanya:

Seperti yang ditunjukkan dalam ilustrasi materi Anda, foundation model dilatih menggunakan kumpulan data besar yang tidak berlabel. Melalui self-supervised learning (pembelajaran mandiri) dan fine-tuning, model dapat menerapkan informasi umum yang telah dipelajarinya ke tugas-tugas khusus.

**Keuntungannya:**

- Mengurangi waktu untuk melabeli data secara manual.
    
- Mempercepat proses pemrograman model.
    
- Memudahkan berbagai industri untuk menerapkan AI pada spektrum aplikasi yang lebih luas.
    

![](src/08-Foundation%20models-1.png)

Untuk menjelaskan lebih lanjut arti dari membangun sesuatu yang lebih spesifik di atas dasar yang lebih luas (itulah mengapa disebut **foundation** atau fondasi), perhatikan contoh ChatGPT.

Pada ChatGPT versi awal, model LLM bernama **GPT-3.5** berfungsi sebagai _foundation model_. OpenAI menggunakan beberapa data khusus percakapan (_chat-specific data_) untuk menciptakan versi GPT-3.5 yang telah dimodifikasi, yang dikhususkan agar bekerja sangat baik sebagai _chatbot_. Versi modifikasi inilah yang kemudian menjadi ChatGPT.

_Foundation models_ berusaha membangun kerangka kerja berbasis fungsi yang lebih luas, melampaui batasan bahasa, untuk menciptakan ruang bagi sistem baru di masa depan.

Berikut adalah dua contoh penting _foundation models_ di berbagai domain:

### NLP (Pemrosesan Bahasa Alami)

- **Model Granite (IBM):** Seperti Granite.13b.instruct dan Granite.13b.chat, menggunakan arsitektur "decoder" untuk memprediksi kata berikutnya dalam urutan secara akurat.
    
- **BERT (Google):** Model fondasi yang terkenal karena kemampuannya memahami konteks teks secara dua arah (_bidirectional_).
    
- **GPT (OpenAI):** Seri GPT (GPT-2, GPT-3) sangat terkenal dalam pembuatan dan pemahaman teks.
    
- **RoBERTa (Meta/Facebook):** Versi pengembangan dari BERT yang mencapai hasil terbaik di berbagai tolok ukur NLP.
    
- **T5 (Google):** Menganggap semua tugas NLP sebagai masalah "teks-ke-teks".
    

### Computer Vision (Visi Komputer)

- **ResNet:** Model dasar untuk klasifikasi gambar yang menangani jaringan saraf dalam secara efisien.
    
- **Inception (Google):** Efektif untuk pengenalan gambar dan deteksi objek.
    
- **EfficientNet:** Dirancang untuk klasifikasi gambar dengan fokus pada efisiensi sumber daya komputasi.
    
- **DALL-E (OpenAI):** Model teks-ke-gambar yang menggunakan teknik _deep learning_.
    
- **Stable Diffusion:** Model teks-ke-gambar menggunakan _latent diffusion model_.

