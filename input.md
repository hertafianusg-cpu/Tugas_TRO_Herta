**Laporan Proyek**

**Analisis dan Optimasi Sistem Distribusi Barang pada Perusahaan Retail
Optima**

![](./image1.png){width="2.71875in" height="2.71875in"}

Disusun Oleh :

  -----------------------------------------------------------------------
  Nama              : Hertafianus Ge'e
  ----------------- -----------------------------------------------------
  Nim               : 231011401257

  Kelas             : 05TPLM009
  -----------------------------------------------------------------------

Dosen Pengampu : Agung Perdananto, S.Kom., M.Kom

**PROGRAM STUDI TEKNIK INFORMATIKA**

**FAKULTAS ILMU KOMPUTER**

**UNIVERSITAS PAMULANG**

**\
DAFTAR ISI**

**\
**

**PENDAHULUAN**

1.  **Latar Belakang Masalah**

> Perusahaan retail fiktif RetailOptima, yang beroperasi di Indonesia,
> menghadapi tantangan dalam mengelola sistem distribusi barang dari dua
> gudang pusatnya, yaitu Gudang A di Jakarta dan Gudang B di Surabaya,
> ke tiga toko cabang di Bandung (Toko 1), Yogyakarta (Toko 2), dan Bali
> (Toko 3). Biaya transportasi yang tinggi menjadi masalah utama karena
> alokasi pengiriman yang kurang optimal, di mana pemilihan rute dan
> jumlah barang yang dikirim belum meminimalkan biaya secara efektif.
> Dengan kapasitas gudang yang terbatas (500 unit untuk Gudang A dan 400
> unit untuk Gudang B) dan permintaan toko yang harus dipenuhi (300 unit
> untuk Toko 1, 250 unit untuk Toko 2, dan 350 unit untuk Toko 3),
> perusahaan membutuhkan strategi distribusi yang efisien untuk
> mengurangi biaya tanpa melanggar kendala operasional.
>
> Biaya transportasi per unit bervariasi antar rute, misalnya 10 ribu
> Rupiah dari Gudang A ke Toko 1 dan 8 ribu Rupiah dari Gudang B ke Toko
> 3, yang menunjukkan perlunya analisis cermat untuk memilih kombinasi
> rute terbaik. Selain itu, potensi perubahan seperti kenaikan biaya
> transportasi, peningkatan permintaan, atau kebutuhan ekspansi gudang
> menambah kompleksitas masalah, sehingga memerlukan pendekatan berbasis
> data untuk mengevaluasi dampaknya. Kurangnya optimasi ini dapat
> menghambat efisiensi operasional dan daya saing perusahaan di pasar
> retail. Oleh karena itu, proyek ini bertujuan untuk mengembangkan
> model optimasi linier guna meminimalkan biaya transportasi,
> menganalisis sensitivitas terhadap perubahan parameter, dan memberikan
> rekomendasi strategis untuk meningkatkan efisiensi distribusi
> RetailOptima.

2.  **Rumusan Masalah**

```{=html}
<!-- -->
```
1.  Bagaimana merumuskan model matematis untuk mengoptimalkan alokasi
    pengiriman barang guna meminimalkan total biaya transportasi, dengan
    mempertimbangkan kendala kapasitas gudang dan permintaan toko?

2.  Bagaimana menyelesaikan model tersebut secara manual (menggunakan
    metode seperti Northwest Corner) dan dengan perangkat lunak (Python
    dengan PuLP dan Excel Solver), serta bagaimana perbandingan
    hasilnya?

3.  Apa dampak dari perubahan parameter (misalnya, penambahan gudang,
    kenaikan biaya transportasi, atau peningkatan permintaan) terhadap
    solusi optimal, dan skenario mana yang paling realistis untuk
    diterapkan?

4.  Rekomendasi apa yang dapat diberikan kepada RetailOptima untuk
    meningkatkan efisiensi sistem distribusi berdasarkan analisis
    sensitivitas dan hasil optimasi?

```{=html}
<!-- -->
```
3.  **Tujuan Proyek**

```{=html}
<!-- -->
```
1.  Menemukan alokasi pengiriman optimal yang meminimalkan total biaya
    transportasi.

2.  Menganalisis sensitivitas model terhadap perubahan parameter untuk
    memahami ketahanan solusi.

3.  Memberikan rekomendasi strategis untuk meningkatkan efisiensi
    operasional distribusi RetailOptima.

```{=html}
<!-- -->
```
4.  **Manfaat dan ruang lingkup**

> Proyek \"Analisis dan Optimasi Sistem Distribusi Barang pada
> Perusahaan Retail Fiktif RetailOptima\" menghadirkan solusi yang
> bermanfaat untuk meningkatkan efisiensi operasional perusahaan retail
> fiktif ini. Dengan fokus pada distribusi barang dari dua gudang di
> Jakarta dan Surabaya ke tiga toko cabang di Bandung, Yogyakarta, dan
> Bali, proyek ini berhasil merumuskan strategi pengiriman yang
> meminimalkan biaya transportasi hingga 10,100 ribu Rupiah. Lebih dari
> itu, analisis sensitivitas mengungkap peluang penghematan tambahan
> sebesar 6% jika perusahaan menambah gudang baru, memberikan wawasan
> berharga untuk ekspansi jangka panjang. Solusi ini tidak hanya
> mengoptimalkan rute pengiriman dengan memanfaatkan jalur berbiaya
> rendah, tetapi juga meningkatkan ketahanan perusahaan terhadap
> perubahan seperti kenaikan biaya atau permintaan pasar.
>
> Dari sisi akademis, proyek ini menjadi contoh nyata penerapan
> pemrograman linier, menggunakan metode manual seperti Northwest Corner
> Method serta perangkat lunak seperti Python (PuLP) dan Excel Solver.
> Hasil yang konsisten dari kedua alat ini memperkuat kepercayaan pada
> solusi yang dihasilkan, sekaligus menawarkan pembelajaran praktis bagi
> mahasiswa atau praktisi di bidang riset operasi. Model yang dibuat
> juga fleksibel, memungkinkan adaptasi untuk perusahaan lain dengan
> kebutuhan distribusi serupa, didukung oleh kemampuan otomatisasi
> Python untuk analisis skala besar.
>
> Ruang lingkup proyek ini sengaja dibatasi untuk menjaga fokus pada
> optimasi biaya transportasi. Dengan data fiktif yang
> realistis---kapasitas gudang 500 dan 400 unit, permintaan toko 300,
> 250, dan 350 unit, serta biaya transportasi antara 8 hingga 20 ribu
> Rupiah per unit---proyek ini menangani masalah transportasi secara
> mendalam. Analisis dilakukan melalui pendekatan manual dan dua
> perangkat lunak, dengan tambahan analisis sensitivitas untuk tiga
> skenario: penambahan gudang, kenaikan biaya, dan peningkatan
> permintaan. Hasil disajikan dalam tabel dan grafik batang untuk
> memudahkan pemahaman, meskipun faktor eksternal seperti kemacetan atau
> regulasi lingkungan tidak dimasukkan dalam model awal demi
> kesederhanaan. Asumsi seperti barang homogen dan biaya proporsional
> juga digunakan untuk menjaga analisis tetap terfokus.
>
> Dengan ruang lingkup yang jelas, proyek ini tidak hanya menghasilkan
> solusi praktis yang siap diterapkan oleh RetailOptima, tetapi juga
> membuka peluang untuk pengembangan lebih lanjut, seperti memasukkan
> faktor eksternal atau menyesuaikan model untuk skenario lain. Proyek
> ini menjadi jembatan antara teori optimasi dan aplikasi dunia nyata,
> memberikan manfaat nyata bagi efisiensi dan pengambilan keputusan
> berbasis data.
