---
obsidianUIMode: preview
note_type: theory
judul_materi: Identify the issue
sumber:
  - ibm.skillsbuild
date_learned: 2025-12-30T15:53:00
tags:
---
Link Sumber: [Identify the issue](https://alm.ibm.com/ibm-skillsbuildadult/trainingId/course:4058927/trainingInstanceId/course:4058927_4630722/en-US)

---
```ad-summary

```

# Identify the issue

Jordan telah mengambil peran baru sebagai _Chief Data Officer_ di perusahaan perbankan tersebut. Sebelum Jordan bergabung, perusahaan telah menguji sistem AI baru, yang pertama di jenisnya, untuk membantu grup _PeopleOps_ mereka mengidentifikasi kandidat bernilai tinggi dalam kumpulan promosi jabatan tahun ini.

Sistem tersebut tampaknya berfungsi, sehingga tim membagikan daftar promosi kepada Priscilla, Direktur Operasi Personalia (_People Operations_). Pertama, Priscilla melihat daftar tersebut bersama dengan informasi demografis para kandidat. Saat dia meninjau daftar itu, sesuatu menarik perhatiannya. Priscilla menyadari bahwa jumlah kandidat yang dipromosikan yang memiliki gelar sarjana sangat tidak proporsional. Dia terkejut karena dia secara khusus telah merekomendasikan seorang karyawan tanpa gelar sarjana yang sudah menjalankan tugas di level jabatan berikutnya dan terdengar sangat cocok untuk promosi, tetapi orang tersebut tidak ada dalam daftar promosi. Dia memanggil Jordan untuk memulai penyelidikan.

![](src/07-Identify%20the%20issue-1.png)

Jordan meminta tim data sains untuk menyelidiki kekhawatiran Priscilla. Sebagai langkah awal, tim data sains dengan cepat menganalisis data promosi selama 5 tahun yang digunakan untuk melatih sistem AI tersebut.

Tabel berikut menunjukkan sampel data yang mereka kumpulkan:

| **Atribut Karyawan**     | **Karyawan 1** | **Karyawan 2** | **Karyawan...** |
| ------------------------ | -------------- | -------------- | --------------- |
| ID Karyawan          | 1              | 2              | ...             |
| Departemen Karyawan  | Data & AI      | Data & AI      | ...             |
| Pendidikan Karyawan  | S2 (Masters)   | Tanpa Gelar    | ...             |
| Lama Bekerja (Tahun) | 10             | 12             | ...             |
| Rating Rata-rata     | 3.5/5          | 4.5/5          | ...             |
| Keputusan Promosi    | Ya             | Tidak          | ...             |

Tim menyusun temuan awal mereka dalam sebuah grafik yang menunjukkan data promosi dan tingkat pendidikan kandidat:

![|500](src/07-Identify%20the%20issue-2.png)



Dengan melihat grafik tersebut, Jordan memperhatikan bahwa secara historis terdapat jumlah kandidat dengan gelar sarjana yang jauh lebih banyak dibandingkan kandidat tanpa gelar sarjana dalam kumpulan kandidat akhir untuk promosi. Terpikir oleh mereka bahwa sistem tersebut mungkin memiliki masalah keadilan yang mengakibatkan bias berdasarkan pendidikan.

![](src/07-Identify%20the%20issue-3.png)

Jordan mengumpulkan tim untuk mendiskusikan masalah yang mereka temukan dan merencanakan apa yang perlu dilakukan selanjutnya.

Sebagai langkah pertama untuk mengatasi dilema tersebut, Jordan bertanya kepada tim apakah menurut mereka ada nilai bisnis untuk tetap mempertahankan sistem AI tersebut.

Jordan bertanya, “Apakah menurut kalian kita harus terus menggunakan AI untuk membantu proses promosi?”

Setelah berpikir sejenak, Priscilla menganggukkan kepalanya.

“Jika dilakukan dengan baik dan dengan cara yang dapat dipercaya oleh anggota tim PeopleOps, ini akan menghemat waktu kita dan dapat membantu kita membuat proses promosi menjadi lebih adil,” kata Priscilla.

Jordan, Priscilla, dan Nischal semuanya sepakat bahwa nilai dari AI itu ada, jika diterapkan dengan benar.