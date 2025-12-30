---
obsidianUIMode: preview
note_type: theory
judul_materi: Large language models
sumber:
  - ibm.skillsbuild
date_learned: 2025-12-30T14:29:00
tags:
---
Link Sumber: [Large language models](https://alm.ibm.com/ibm-skillsbuildadult/trainingId/course:4058859/trainingInstanceId/course:4058859_4630654/en-US)

---
```ad-summary

```

# Large language models

Large language models (LLMs) adalah jenis mesin AI generatif yang dirancang untuk memproses dan menghasilkan teks. Model-model ini bekerja dengan menyisir dataset yang sangat luas, lalu menggunakan pengetahuan tersebut untuk menghasilkan konten teks baru yang meniru gaya dan nada dari materi aslinya. Contoh populer termasuk GPT-4 (OpenAI), PaLM (Google), dan LLaMA (Meta).

Terdapat dua jenis LLM:

- **Proprietary LLMs (Milik Perusahaan):** Dimiliki dan dikendalikan oleh perusahaan tertentu. Hanya bisa digunakan oleh pelanggan yang membeli lisensi atau berlangganan (contoh: GPT-4).
    
- **Open-source LLMs (Sumber Terbuka):** Tersedia untuk publik secara gratis di bawah lisensi terbuka. Siapa saja dapat mengunduh, menjalankan, dan terkadang memodifikasinya (contoh: LLaMA).
    

### Hubungan LLM dengan Foundation Models

LLM adalah salah satu bentuk _foundation model_ yang paling umum. Mereka dilatih pada data teks dalam skala terabyte (unlabeled data) agar memiliki pemahaman bahasa yang luas sebelum akhirnya disesuaikan untuk tugas spesifik melalui _tuning_.

### Keuntungan dan Risiko

Kedua jenis LLM ini memiliki manfaat masing-masing, namun penggunaannya juga membawa risiko yang harus dikelola:

1. **Bias:** Karena dilatih dari data internet, model bisa meniru prasangka manusia.
    
2. **Kepercayaan:** Penting untuk memastikan output yang dihasilkan akurat dan tidak menyesatkan.
    
3. **Etika:** Diperlukan pedoman industri untuk memastikan AI berkontribusi positif tanpa menyebabkan bahaya.

---

**Cara Kerja Large Language Models (LLM)**

GPT atau _generative pre-trained transformer_ adalah sebuah _large language model_ atau LLM yang dapat menghasilkan teks seperti manusia, dan saya telah menggunakan GPT dalam berbagai bentuknya selama bertahun-tahun. Dalam video ini, kita akan: pertama, bertanya apa itu LLM? Kedua, kita akan menjelaskan bagaimana cara kerjanya. Dan ketiga, kita akan bertanya apa saja aplikasi bisnis dari LLM.

Mari kita mulai dengan yang pertama: **apa itu large language model?** Jadi, _large language model_ adalah sebuah contoh dari sesuatu yang lain, yang disebut _foundation model_. Sekarang, _foundation models_ dilatih sebelumnya pada data yang tidak terlabel dan bersifat _self-supervised_ dalam jumlah besar, artinya model tersebut belajar dari pola-pola dalam data dengan cara yang menghasilkan _output_ yang dapat digeneralisasi dan diadaptasi.

Dan _large language models_ adalah contoh dari _foundation models_ yang diterapkan secara khusus pada teks dan hal-hal yang menyerupai teks. Saya berbicara tentang hal-hal seperti kode komputer. Sekarang, _large language models_ dilatih pada kumpulan data teks yang besar seperti buku, artikel, dan percakapan. Dan dengarlah, ketika kita mengatakan "besar", model-model ini bisa berukuran puluhan gigabyte dan dilatih pada data teks yang sangat banyak. Kita berbicara tentang kemungkinan petabyte data di sini. Untuk memberikan perspektif, sebuah file teks yang berukuran, katakanlah, satu gigabyte, dapat menyimpan sekitar 178 juta kata. Banyak sekali kata hanya dalam satu GB. Dan ada berapa gigabyte dalam satu petabyte? Itu sekitar satu juta. Ya, itu benar-benar teks yang sangat banyak.

LLM juga termasuk di antara model-model terbesar dalam hal jumlah parameter. Sebuah **parameter** adalah nilai yang dapat diubah oleh model secara mandiri saat ia belajar, dan semakin banyak parameter yang dimiliki sebuah model, semakin kompleks model tersebut. GPT-3, misalnya, dilatih sebelumnya pada korpus data sebesar 45 terabyte dan menggunakan 175 miliar parameter LLM.

Baiklah, jadi **bagaimana cara kerjanya?** Kita bisa memikirkannya seperti ini: LLM sama dengan tiga hal – **data**, **arsitektur**, dan terakhir, kita bisa menganggapnya sebagai **pelatihan**. Ketiga hal itu benar-benar komponen dari sebuah LLM. Sekarang, kita sudah membahas tentang jumlah data teks yang sangat besar yang masuk ke dalamnya. Adapun untuk arsitekturnya, ini adalah sebuah jaringan saraf (_neural network_), dan untuk GPT, itu adalah sebuah **transformer**.

Arsitektur transformer memungkinkan model untuk menangani urutan data seperti kalimat atau baris kode, dan transformer dirancang untuk memahami konteks dari setiap kata dalam sebuah kalimat dengan mempertimbangkannya dalam kaitannya dengan setiap kata lainnya. Hal ini memungkinkan model untuk membangun pemahaman yang komprehensif tentang struktur kalimat dan makna kata-kata di dalamnya. Kemudian arsitektur ini dilatih pada semua data yang sangat banyak ini. Selama pelatihan, model belajar untuk memprediksi kata berikutnya dalam sebuah kalimat. Jadi, "langit itu" (_the sky is_), ia dimulai dengan tebakan acak. "Langit itu serangga" (_the sky is bug_). Tetapi pada setiap iterasi, model menyesuaikan parameter internalnya untuk mengurangi perbedaan antara prediksinya dan hasil yang sebenarnya. Dan model terus melakukan ini secara bertahap meningkatkan prediksi katanya sampai ia dapat secara andal menghasilkan kalimat yang koheren. Lupakan tentang "serangga", ia bisa tahu bahwa itu adalah "biru".

Sekarang, model tersebut dapat **disetel halus (fine-tuned)** pada kumpulan data yang lebih kecil dan lebih spesifik. Di sini model menyempurnakan pemahamannya agar mampu melakukan tugas spesifik ini dengan lebih akurat. _Fine-tuning_ inilah yang memungkinkan model bahasa umum menjadi ahli dalam tugas tertentu.

Oke, jadi bagaimana semua ini masuk ke poin nomor tiga, **aplikasi bisnis?** Untuk aplikasi layanan pelanggan, bisnis dapat menggunakan LLM untuk membuat chatbot cerdas yang dapat menangani berbagai pertanyaan pelanggan, membebaskan agen manusia untuk masalah yang lebih kompleks.

Bidang bagus lainnya adalah pembuatan konten. Itu bisa mendapatkan keuntungan dari LLM yang dapat membantu menghasilkan artikel, email, postingan media sosial, dan bahkan skrip video YouTube. Hmm, itu sebuah ide yang bagus sekarang.

LLM bahkan dapat berkontribusi pada pengembangan perangkat lunak, dan mereka dapat melakukannya dengan membantu menghasilkan dan meninjau kode. Dan itu baru permukaannya saja. Seiring _large language models_ terus berevolusi, kita pasti akan menemukan lebih banyak aplikasi inovatif dan itulah mengapa saya sangat terpikat dengan _large language models_.

Jika Anda memiliki pertanyaan, silakan tulis di bawah dan jika Anda ingin melihat lebih banyak video seperti ini di masa mendatang, silakan sukai dan berlangganan. Terima kasih telah menonton.