---
obsidianUIMode: preview
note_type: theory
judul_materi: What is generative AI
sumber:
  - ibm.skillsbuild
date_learned: 2025-12-30T14:11:00
tags:
---
Link Sumber: [What is generative AI](https://alm.ibm.com/ibm-skillsbuildadult/trainingId/course:4058859/trainingInstanceId/course:4058859_4630654/en-US)

---
```ad-summary

```

# What is generative AI

![](src/05-What%20is%20generative%20AI-1.png)

AI, _machine learning_, dan _deep learning_ bekerja beriringan untuk memungkinkan sistem AI tidak hanya memahami tetapi juga menghasilkan konten dan respons. Gen-AI menggunakan kemampuan _deep learning_ untuk menciptakan konten baru, seperti gambar, teks, dan bahkan seluruh percakapan. Hal ini dilakukan dengan memahami dan menyimulasikan pola dari data yang ada.

Karena _machine learning_ dan _deep learning_ cenderung digunakan secara bergantian, penting untuk memahami perbedaan antara keduanya.

### Machine learning

Machine learning adalah bidang yang berkembang pesat dengan berbagai aplikasi dan merupakan bagian mendasar dari banyak teknologi yang kita gunakan saat ini, mulai dari asisten suara hingga sistem rekomendasi dan kendaraan otonom.

_Machine learning_ adalah cabang dari kecerdasan buatan dan ilmu komputer yang berfokus pada penggunaan data dan algoritma untuk meniru cara manusia belajar, serta secara bertahap meningkatkan akurasinya.

Model-model _machine learning_ terbagi dalam tiga kategori utama:

- **Supervised learning (Pembelajaran Terawasi):** Menggunakan kumpulan data berlabel untuk melatih algoritma guna mengklasifikasikan data atau memprediksi hasil secara akurat.
    
- **Unsupervised learning (Pembelajaran Tidak Terawasi):** Menggunakan algoritma _machine learning_ untuk menganalisis dan mengelompokkan kumpulan data yang tidak berlabel, dengan sedikit atau tanpa kebutuhan campur tangan manusia.
    
- **Semi-supervised learning (Pembelajaran Semi-terawasi):** Menggunakan kumpulan data pelatihan yang berisi data berlabel dan tidak berlabel.
    

Pemilihan pendekatan _machine learning_ mana yang akan digunakan bergantung pada masalah spesifik, ketersediaan data berlabel, dan hasil yang diinginkan. Setiap kategori memiliki kekuatan dan kelemahannya sendiri, dan sangat penting untuk memilih pendekatan yang tepat untuk tugas yang dihadapi.

### Deep learning

Gen-AI merujuk pada kemampuan model deep learning untuk mengambil data mentah dan menghasilkan output yang serupa tetapi tidak identik dengan data aslinya.

_Deep learning_ adalah bagian dari _machine learning_, yang pada dasarnya merupakan jaringan saraf (_neural network_) dengan tiga lapisan atau lebih.

_Deep learning_ berbeda dari _machine learning_ tradisional dalam pendekatannya menangani data dan metode pembelajaran. Sementara _machine learning_ biasanya bergantung pada data terstruktur dan berlabel dengan fitur-fitur yang telah ditentukan sebelumnya dan diatur ke dalam tabel, _deep learning_ unggul dalam memproses data tidak terstruktur, seperti teks dan gambar, tanpa memerlukan prapemrosesan yang ekstensif. Ini berarti _deep learning_ mengotomatiskan ekstraksi fitur, mengurangi ketergantungan pada pakar manusia, dan merampingkan proses penanganan data.
### Generative AI

Model generatif telah digunakan selama bertahun-tahun dalam statistik untuk menganalisis data numerik. Namun, kebangkitan deep learning membuka berbagai kemungkinan baru, memungkinkan model-model ini menangani jenis data yang lebih rumit seperti gambar dan ucapan. Salah satu kelas model pertama yang mencapai keberhasilan lintas domain ini adalah variational autoencoders, atau VAE, yang diperkenalkan pada tahun 2013. VAE merupakan kemajuan yang nyata, berfungsi sebagai model deep learning pertama yang digunakan secara luas untuk menghasilkan gambar dan ucapan yang realistis.


#### Transcript

Apa itu model Generative AI?

Selama beberapa bulan terakhir, model bahasa besar atau LLM seperti ChatGPT telah mengguncang dunia. Baik itu menulis puisi atau membantu merencanakan liburan Anda berikutnya, kita melihat perubahan besar dalam performa AI dan potensinya untuk mendorong nilai bagi perusahaan.

Nama saya Kate Soule. Saya manajer senior strategi bisnis di IBM Research dan hari ini saya akan memberikan gambaran singkat tentang bidang baru AI yang sedang muncul ini dan bagaimana bidang ini dapat digunakan dalam pengaturan bisnis untuk menghasilkan nilai.

Sekarang, model bahasa besar sebenarnya adalah bagian dari kelas model yang berbeda yang disebut **foundation models** (model fondasi).1 Istilah _foundation model_ sebenarnya pertama kali dicetuskan oleh tim dari Stanford ketika mereka melihat bahwa bidang AI sedang mengerucut pada paradigma baru.2 Sebelumnya, aplikasi AI dibangun dengan melatih mungkin sekumpulan model AI yang berbeda, di mana setiap model AI dilatih pada data yang sangat spesifik untuk melakukan tugas yang sangat spesifik. Mereka memprediksi bahwa kita akan mulai pindah ke paradigma baru. Di mana kita akan memiliki kemampuan fondasi atau _foundation model_ yang akan mendorong semua kasus penggunaan dan aplikasi yang sama ini. Jadi aplikasi yang sama persis dengan yang kita bayangkan sebelumnya dengan AI konvensional, model yang sama ini dapat menjalankan sejumlah aplikasi tambahan lainnya. Intinya adalah model ini dapat ditransfer ke sejumlah tugas apa pun yang memberikan model ini "kekuatan super" untuk dapat ditransfer ke berbagai tugas yang berbeda dan menjalankan berbagai fungsi yang berbeda karena ia telah dilatih dalam jumlah yang sangat besar secara tidak terawasi (_unsupervised_) pada data yang tidak terstruktur.

Dan apa artinya itu dalam domain bahasa pada dasarnya adalah sekumpulan kalimat—dan saya berbicara tentang terabyte data di sini—untuk melatih model ini. Awal kalimat saya mungkin "tidak ada gunanya menangisi tumpahan" dan akhir kalimat saya mungkin "susu" (_milk_), dan saya mencoba membuat model saya memprediksi kata terakhir dari kalimat tersebut berdasarkan kata-kata yang dilihatnya sebelumnya. Kemampuan generatif dari model yang memprediksi dan menghasilkan kata berikutnya berdasarkan kata-kata sebelumnya yang dilihat sebelumnya inilah alasan mengapa _foundation models_ sebenarnya adalah bagian dari bidang AI yang disebut **generative AI**.

Karena kita menghasilkan sesuatu yang baru, dalam hal ini kata berikutnya dalam sebuah kalimat, dan meskipun model-model ini dilatih untuk melakukan tugas generasi pada intinya (memprediksi kata berikutnya dalam kalimat), kita sebenarnya dapat mengambil model-model ini dan jika Anda memasukkan sedikit data berlabel ke dalam persamaan tersebut, Anda dapat menyetelnya (_tune_) untuk melakukan tugas NLP tradisional seperti klasifikasi atau pengenalan entitas bernama (_named entity recognition_)—hal-hal yang biasanya tidak Anda kaitkan sebagai model atau kemampuan berbasis generatif. Proses ini disebut "**tuning**", di mana Anda dapat menyetel _foundation model_ Anda.3 Dengan memasukkan sedikit data, Anda memperbarui parameter model Anda dan sekarang ia dapat melakukan tugas bahasa alami yang sangat spesifik. Jika Anda tidak memiliki data atau hanya memiliki sangat sedikit titik data, Anda masih dapat mengambil _foundation models_ ini dan mereka sebenarnya bekerja sangat baik dalam domain data berlabel rendah melalui proses yang disebut "**prompting**" atau "**prompt engineering**".

Anda dapat menerapkan model-model ini untuk beberapa tugas yang sama persis. Contoh penggunaan _prompting_ pada model untuk melakukan tugas klasifikasi adalah: Anda bisa memberikan model sebuah kalimat lalu mengajukan pertanyaan, apakah kalimat ini memiliki sentimen positif atau sentimen negatif? Model akan mencoba menyelesaikan pembuatan kata-kata dalam kalimat tersebut dan kata alami berikutnya dalam kalimat tersebut adalah jawaban untuk masalah klasifikasi Anda. Jadi, ia akan merespons positif atau negatif tergantung di mana ia memperkirakan sentimen kalimat tersebut berada. Dan model-model ini bekerja secara mengejutkan dengan baik ketika diterapkan pada pengaturan dan domain baru ini. Sekarang, di sinilah banyak keuntungan dari _foundation models_ berperan.

Jika kita berbicara tentang keuntungan, keuntungan utamanya adalah **performa**. Model-model ini telah melihat begitu banyak data—sekali lagi, Data dengan huruf D kapital, terabyte data—sehingga pada saat mereka diterapkan pada tugas-tugas kecil, mereka dapat secara drastis mengungguli model yang hanya dilatih pada beberapa titik data saja. Keuntungan kedua dari model-model ini adalah **peningkatan produktivitas**.4 Seperti yang saya katakan tadi, melalui _prompting_ atau _tuning_, Anda membutuhkan jauh lebih sedikit data berlabel untuk mencapai model spesifik tugas dibandingkan jika Anda harus memulai dari awal, karena model Anda memanfaatkan semua data tidak berlabel yang dilihatnya dalam prapelatihan saat kita membuat tugas generatif ini.

Bersamaan dengan keuntungan ini, ada juga beberapa kerugian yang penting untuk diingat. Yang pertama adalah **biaya komputasi**. Hukuman karena model ini melihat begitu banyak data adalah biaya pelatihannya sangat mahal, sehingga sulit bagi perusahaan kecil untuk melatih _foundation model_ sendiri. Mereka juga mahal karena ukurannya yang sangat besar, mencapai miliaran parameter, sehingga biaya untuk menjalankan inferensi (penggunaan) juga sangat mahal.5 Anda mungkin memerlukan beberapa GPU sekaligus hanya untuk meng-hosting model-model ini dan menjalankan inferensi, menjadikannya metode yang lebih mahal daripada pendekatan tradisional.

Kerugian kedua dari model-model ini adalah pada sisi **kepercayaan** (_trustworthiness_). Sama seperti data yang menjadi keuntungan besar bagi model-model ini karena telah melihat begitu banyak data tidak terstruktur, hal itu juga mendatangkan biaya. Terutama dalam domain seperti bahasa, banyak dari model ini dilatih pada dasarnya dari data bahasa yang diambil (_scraped_) dari internet dan jumlah datanya sangat banyak.6 Bahkan jika Anda memiliki seluruh tim anotator manusia, Anda tidak akan bisa memeriksa setiap titik data untuk memastikan bahwa data tersebut tidak bias dan tidak mengandung ujaran kebencian atau informasi beracun lainnya—dan itu baru asumsi jika Anda benar-benar tahu datanya apa. Seringkali, untuk banyak model sumber terbuka (_open-source_) yang dipublikasikan, kita bahkan tidak tahu kumpulan data apa yang digunakan untuk melatih model tersebut, yang menyebabkan masalah kepercayaan.

Jadi, IBM mengakui potensi besar dari teknologi ini, tetapi rekan-rekan saya di IBM Research sedang mengerjakan berbagai inovasi berbeda untuk mencoba meningkatkan efisiensi model-model ini serta kepercayaan dan keandalannya agar lebih relevan dalam pengaturan bisnis.

Semua contoh yang saya bicarakan sejauh ini hanya dari sisi bahasa, tetapi kenyataannya, ada banyak domain lain di mana _foundation models_ dapat diterapkan.7 Seperti yang kita tahu, kita telah melihat _foundation models_ pada visi seperti model DALLE 2, yang mengambil data teks dan menggunakannya untuk menghasilkan gambar kustom.8 Kita telah melihat model untuk kode dengan produk seperti Copilot yang dapat membantu melengkapi kode saat sedang ditulis.

IBM sedang berinovasi di semua domain ini, baik itu model bahasa yang kami bangun ke dalam produk seperti Watson Assistant dan Watson Discovery, model visi yang kami bangun ke dalam produk seperti Maximo Visual Inspection, atau model kode Ansible yang kami bangun bersama mitra kami di Red Hat di bawah Project Wisdom. Kami berinovasi di semua domain ini dan lebih banyak lagi. Kami sedang mengerjakan bidang kimia. Sebagai contoh, kami baru saja menerbitkan dan merilis MoLFormer, yaitu sebuah _foundation model_ untuk mendorong penemuan molekul bagi berbagai terapi target, dan kami sedang mengerjakan model untuk perubahan iklim dengan membangun _earth science foundation models_, menggunakan data geospasial untuk meningkatkan penelitian iklim.

Saya harap Anda menemukan video ini informatif dan bermanfaat. Jika Anda tertarik untuk mempelajari lebih lanjut, khususnya bagaimana IBM berupaya memperbaiki beberapa kerugian ini dengan membuat _foundation models_ lebih tepercaya dan lebih efisien, silakan lihat tautan di bawah ini.

Terima kasih.

---

Ada beberapa model bahasa besar (_large language models_) yang dikembangkan oleh berbagai organisasi dan peneliti. Beberapa contoh model bahasa besar meliputi:

- **Granite oleh IBM:** Arsitektur khusus _decoder_ yang dirancang untuk tugas generatif, seperti peringkasan, pembuatan konten, dan ekstraksi wawasan.
    
- **GPT-3 (Generative Pre-trained Transformer 3) oleh OpenAI:** GPT merujuk pada kelas model termasuk GPT-2, GPT-3, dan GPT-4. Sistem percakapan yang dibangun di atas GPT-3 dan disesuaikan menggunakan teknik _supervised learning_ dan _reinforcement learning_.
    
- **T5 (Text-to-Text Transfer Transformer) oleh Google AI:** Arsitektur berbasis _transformer_ yang menggunakan pendekatan teks-ke-teks untuk tugas termasuk penerjemahan, menjawab pertanyaan, dan klasifikasi.
    
- **BERT oleh Google AI:** Teknik _machine learning_ berbasis _transformer_ untuk pemrosesan bahasa alami (_NLP_), yang dilatih sebelumnya pada pemodelan bahasa dan tugas prediksi kalimat.
    
- **RoBERTa (A Robustly Optimized BERT Pretraining Approach) oleh Meta:** Perluasan dari BERT yang dilatih pada kumpulan data yang lebih besar dengan kalimat yang lebih panjang, dan menghapus tugas prediksi kalimat.
    
- **ALBERT (A Lite BERT) oleh Google Research:** Model pembelajaran representasi bahasa _self-supervised_ yang dirancang untuk mengurangi biaya komputasi prapelatihan sambil tetap mempertahankan performa.
    
- **LLaMA oleh Meta:** Model bahasa _auto-regressive_ berdasarkan arsitektur _transformer_ yang hadir dalam berbagai ukuran: parameter 7B, 13B, 33B, dan 65B. LLaMA dirilis di bawah lisensi non-komersial.
    

Bidang pemrosesan bahasa alami telah mengalami kemajuan signifikan berkat model-model ini, yang telah digunakan dalam berbagai aplikasi seperti pembuatan teks, analisis sentimen, penerjemahan, dan lain-lain.

Seiring teknologi di balik kecerdasan buatan terus berkembang, AI digunakan di lebih banyak industri daripada sebelumnya, termasuk pembuatan konten dan layanan kesehatan. Kemajuan ini mendorong inovasi dan mengubah cara kita berinteraksi dengan sistem yang digerakkan oleh AI.

