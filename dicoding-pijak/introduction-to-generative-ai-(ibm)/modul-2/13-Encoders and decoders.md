---
obsidianUIMode: preview
note_type: theory
judul_materi: Encoders and decoders
sumber:
  - ibm.skillsbuild
date_learned: 2025-12-30T14:52:00
tags:
---
Link Sumber: [Encoders and decoders](https://alm.ibm.com/ibm-skillsbuildadult/trainingId/course:4058859/trainingInstanceId/course:4058859_4630654/en-US)

---
```ad-summary

```

# Encoders and decoders

![|500](src/13-Encoders%20and%20decoders-1.png)


Bayangkan Anda berada dalam tim koki terampil yang bekerja sama untuk membuat resep yang kompleks. Tujuan tim Anda adalah menciptakan hidangan lezat yang menangkap beragam jenis bahan. Hal ini sangat mirip dengan bagaimana LLM memproses berbagai elemen linguistik. Dalam skenario ini, **encoder** mewakili para koki yang bertanggung jawab menyiapkan bahan-bahan mentah. Sama seperti bahan-bahan yang melalui pemilihan, pemotongan, dan perendaman (_marinating_) yang cermat, _encoder_ melakukan tokenisasi dan _embedding_, mengubah setiap kata menjadi komponen yang berbeda dan penuh rasa.

![|500](src/13-Encoders%20and%20decoders-2.png)

Setelah bahan-bahan siap, mereka diserahkan kepada koki utama yang bertindak sebagai **decoder**, yang berada di pusat dapur. Berbekal pemahaman mendalam tentang profil rasa, _decoder_ menyusun hidangan tersebut. Mirip dengan kemampuan koki untuk fokus pada bahan tertentu saat memasukkannya ke dalam resep, _decoder_ menggunakan mekanisme perhatian (_attention_) yang unik. Ia memperhatikan berbagai representasi yang telah dikodekan, menambah dan menyesuaikannya secara **autoregresif**, persis seperti bagaimana seorang koki mencicipi dan menyempurnakan hidangan di setiap langkahnya.

![|500](src/13-Encoders%20and%20decoders-3.png)

Keindahan dari analogi kuliner ini terletak pada tarian kolaboratif yang ada antara _encoder_ dan _decoder_. _Encoder_ mempersiapkan bahan-bahan dengan cermat, memberikan palet rasa yang beragam kepada _decoder_. _Decoder_, pada gilirannya, menggabungkan elemen-elemen ini secara kreatif untuk menghasilkan hidangan yang unik dan padu, menunjukkan interaksi komponen yang rumit dalam dunia model bahasa.

Mari pelajari lebih dalam bagaimana _encoder_ dan _decoder_ bekerja.

## Encoder

_Encoder_ menerima urutan input dan mengubahnya menjadi representasi yang menangkap maknanya. Urutan input ini bisa berupa kalimat, paragraf, atau data berurutan lainnya. Sebagai contoh, mari kita perhatikan kalimat: "Saya suka buku."

Inovasi kunci dari transformer adalah mekanisme **multi-head self-attention**. Dalam langkah ini, _encoder_ menghitung jumlah tertimbang dari semua token lainnya, menyoroti pentingnya setiap token dalam kaitannya dengan token saat ini. Hal ini memungkinkan model untuk menangkap hubungan kontekstual antar kata dan memahami ketergantungan dalam urutan tersebut. Misalnya, _encoder_ mungkin mempelajari bahwa kata "suka" berhubungan dengan "Saya" dan "buku" dalam kalimat tersebut. Aspek **multi-head** berarti bahwa _self-attention_ dilakukan beberapa kali secara paralel, masing-masing dengan parameter terpelajari yang berbeda. Ini memungkinkan model untuk fokus pada aspek yang berbeda dari input.

Setelah _self-attention_, _encoder_ menerapkan jaringan saraf **feedforward** untuk mentransformasi lebih lanjut representasi yang telah diperhatikan tersebut. Jaringan ini memperkenalkan non-linearitas dan membantu menangkap hubungan yang lebih kompleks dalam urutan. Jaringan saraf _feedforward_ terdiri dari beberapa lapisan dengan parameter yang dapat dipelajari.

Dengan menerapkan mekanisme _self-attention_ dan transformasi berikutnya menggunakan jaringan saraf _feedforward_, _encoder_ secara efisien menangkap makna dan hubungan dalam urutan input. Representasi yang telah dikodekan ini kemudian dapat digunakan oleh _decoder_ untuk menghasilkan urutan output atau untuk melakukan berbagai tugas turunan lainnya.

**Encoder** adalah komponen atau modul yang memproses data input dan mengubahnya menjadi representasi terstruktur yang dapat dipahami dan digunakan oleh model.

## Decoder

**Decoder** mengambil urutan input yang telah dikodekan oleh _encoder_ dan menghasilkan urutan output. Proses ini dimulai dengan "token awal" (_start token_) sebagai input pertama. _Decoder_ menghasilkan token output satu per satu, di mana setiap token dipengaruhi oleh token yang dihasilkan sebelumnya dan hasil pengodean dari _encoder_. Proses ini berlanjut hingga kondisi tertentu terpenuhi, seperti mencapai panjang maksimum atau menghasilkan token akhir (_end token_).

Berikut adalah mekanisme utama di dalam _decoder_:

- **Masked Self-Attention:** Berbeda dengan _encoder_ yang melihat semua kata sekaligus, _decoder_ menggunakan mekanisme **masking** (penyembunyian). Ini memastikan setiap token hanya bisa melihat token-token sebelumnya dalam urutan output. Hal ini penting untuk menjaga sifat **autoregresif**, sehingga model tidak "mencontek" kata di masa depan saat sedang berlatih.
    
- **Encoder-Decoder Attention:** _Decoder_ memiliki lapisan perhatian tambahan yang memungkinkannya melihat kembali hasil dari _encoder_. Mekanisme ini membantu _decoder_ mempertimbangkan informasi relevan dari input asli saat menyusun output, sehingga terjadi penyelarasan (_alignment_) yang tepat antar keduanya.
    
- **Feedforward Neural Network:** Sama seperti _encoder_, _decoder_ menggunakan jaringan ini untuk memproses representasi token lebih lanjut, menambahkan non-linearitas untuk menangkap hubungan yang rumit.
    

Interaksi antara _encoder_ dan _decoder_ dirancang agar model dapat menangkap hubungan antar token dengan sangat efektif. Dengan memanfaatkan mekanisme _attention_, Transformer jauh lebih unggul dibandingkan arsitektur sebelumnya dalam memahami konteks.


![|500](src/13-Encoders%20and%20decoders-4.png)

Komponen _encoder_ dan _decoder_ pada model Transformer menggunakan _self-attention_ dan jaringan saraf _feed-forward_ untuk memproses dan menghasilkan data berurutan secara efektif.

Dengan memanfaatkan mekanisme ini, model mampu menangkap hubungan dan ketergantungan yang rumit di dalam urutan input maupun output. Hal ini memungkinkan AI untuk menghasilkan hasil yang berkualitas tinggi dan relevan secara kontekstual.