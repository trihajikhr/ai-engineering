---
obsidianUIMode: preview
note_type: theory
judul_materi: Reinforcement learning
sumber:
  - ibm.skillsbuild
date_learned: 2025-12-30T13:09:00
tags:
---
Link Sumber: [Reinforcement learning](https://alm.ibm.com/ibm-skillsbuildadult/trainingId/course:4058918/trainingInstanceId/course:4058918_4630713/en-US)

---
```ad-summary

```

# Reinforcement learning

**Reinforcement learning** adalah model _machine learning_ yang mirip dengan _supervised learning_, tetapi algoritma tidak dilatih menggunakan data sampel. Model ini belajar sambil berjalan dengan menggunakan **trial and error** (uji coba).

Urutan hasil yang sukses diperkuat untuk mengembangkan rekomendasi terbaik bagi suatu masalah. Inti dari metode ini adalah memberi "hadiah" (_reward_) untuk perilaku yang benar dan "hukuman" (_punishment_) untuk perilaku yang salah.

![Image of reinforcement learning feedback loop with agent and environment](https://encrypted-tbn1.gstatic.com/licensed-image?q=tbn:ANd9GcTr7XdjxMFUPyl9DgxyFVoSd7aWIrMwVXbSVj3DTtKHAIfEdAiA2mtnvQ6Dt93L1xPqVYGBCOoWx7JaW6cE7aLcM5m7uN0xuBiarz2KSeg6BuudClU)

Apa maksudnya memberi "hadiah" pada mesin?

Memberi hadiah berarti memberikan penguatan positif kepada sistem (agent) saat melakukan hal yang benar, dan penguatan negatif saat melakukan hal yang salah. Dengan cara ini, mesin akan mencari strategi yang memaksimalkan total hadiah yang diterimanya.

Metode ini sangat populer digunakan dalam:

- Melatih robot untuk berjalan atau menghindari rintangan.
- Mengoptimalkan strategi dalam permainan (seperti catur atau video game).
- Mengelola logistik dan rantai pasokan.

Saat mesin belajar melalui uji coba (_trial and error_), ia melakukan **prediksi**, lalu membandingkannya dengan data dalam **corpus** (kumpulan data) miliknya.

- Setiap kali perbandingannya **positif**, mesin menerima umpan balik numerik positif, atau **reward** (hadiah).
    
- Setiap kali perbandingannya **negatif**, mesin menerima umpan balik numerik negatif, atau **penalty** (hukuman).
    

Seiring berjalannya waktu, prediksi mesin akan menjadi lebih akurat. Hal ini dilakukan secara **otomatis** berdasarkan umpan balik tersebut, bukan melalui campur tangan manusia.