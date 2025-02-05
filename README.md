# Estimasi Frekuensi Klaim pada Pasien Stroke di Indonesia

## Deskripsi

Dalam penelitian ini, data yang digunakan diperoleh dari BPJS Kesehatan, khususnya data terkait FKRTL (Fasilitas Kesehatan Tingkat Lanjut). Data ini diolah dan ditransformasi untuk memastikan kelengkapan dan relevansi, serta untuk memberikan gambaran lebih terperinci mengenai faktor-faktor yang memengaruhi risiko dan frekuensi klaim pasien stroke di Indonesia. Sebelumnya, data FKRTL disajikan per rujukan, namun setelah transformasi, data disajikan per individu berdasarkan nomor peserta.

Beberapa variabel prediktor yang digunakan dalam penelitian ini antara lain:
- Jenis Kelamin
- Kelas Rawat
- Segmentasi
- Diagnosis
- Regional
- Status
- Lama Perawatan
- Umur

## Tujuan

Penelitian ini bertujuan untuk:
1. Menganalisis pengaruh variabel-variabel di atas terhadap frekuensi klaim pasien stroke.
2. Membangun model regresi negatif binomial untuk memprediksi frekuensi klaim.
3. Memberikan wawasan lebih dalam mengenai faktor-faktor yang berkontribusi pada frekuensi klaim stroke dan menyarankan langkah-langkah preventif.

## Visualisasi Data

Beberapa visualisasi yang digunakan dalam penelitian ini antara lain:
- **Jenis Kelamin**: Boxplot menunjukkan bahwa frekuensi klaim antara pasien laki-laki dan perempuan relatif sama.
- **Kelas Rawat**: Frekuensi klaim cenderung lebih tinggi di kelas rawat 1 dibandingkan kelas rawat 2 dan 3.
- **Segmentasi**: Pasien yang termasuk golongan PPU memiliki frekuensi klaim tertinggi.
- **Diagnosis**: Pasien dengan kode diagnosis 656 memiliki frekuensi klaim tertinggi.
- **Regional**: Frekuensi klaim tertinggi ditemukan di regional 1.
- **Status**: Pasien yang masih hidup memiliki frekuensi klaim lebih tinggi dibandingkan pasien yang meninggal.
- **Lama Perawatan**: Pasien dengan perawatan singkat cenderung memiliki frekuensi klaim lebih tinggi.
- **Umur**: Distribusi frekuensi klaim pasien stroke menunjukkan distribusi yang mendekati normal.

## Uji Overdispersi

Untuk menentukan model yang tepat, dilakukan uji overdispersi pada data frekuensi klaim. Hasil uji menunjukkan bahwa terdapat overdispersi yang signifikan, yang berarti data tidak memenuhi asumsi equidispersi pada model Poisson, sehingga model regresi negatif binomial digunakan.

## Pemodelan Regresi Negatif Binomial

Beberapa model regresi negatif binomial diuji, dan model dengan nilai AIC terendah dipilih sebagai model terbaik. Regrouping variabel dilakukan untuk meningkatkan model, dengan memperhatikan variabel-variabel yang signifikan.

## Hasil

1. Jenis kelamin, kelas rawat, segmentasi, regional, diagnosis, lama perawatan, umur, dan status memiliki pengaruh signifikan terhadap frekuensi klaim pasien stroke.
2. Model regresi negatif binomial dengan variabel prediktor yang telah dikelompokkan menghasilkan model terbaik dengan nilai AIC terendah.
3. Koefisien dari setiap variabel prediktor memberikan gambaran mengenai pengaruhnya terhadap frekuensi klaim.
