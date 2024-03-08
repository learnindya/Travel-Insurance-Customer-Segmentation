# Travel-Insurance-Customer-Segmentation
Hanya 35.73% pelanggan yang membeli asuransi perjalanan pada tahun 2019. Tim memiliki tujuan untuk meningkatkan persentase conversion rate menjadi 40%.
Kondisi awal perusahaan tidak memiliki profil pelanggan. Perusahaan hanya menjual 1 paket asuransi.

# Goal
Membuat segmentasi pelanggan.

# Tentang dataset
Rentang umur pelanggan adalah 25-35, termasuk golongan usia produktif yang muda.

Pelanggan didominasi oleh karyawan swasta dan wiraswasta, lulusan universitas, tidak mengidap penyakit kronis, tidak sering bepergian dengan pesawat dan belum pernah traveling keluar negeri.

Pelanggan dengan frekuensi terbanyak berusia 28 tahun, dengan Pendapatan Tahunan 800.000, dan memiliki 4 Anggota Keluarga.

# Data Pre-processing
- Feature encoding: 'GraduateOrNot', 'FrequentFlyer', 'EverTravelledAbroad', 'Employment Type'
- Feature extraction: 'TravelExperience'
- Standardization

# Modeling
- K-means clustering
- Agglomerative
Rand score: 0.9846731276790616
K-Means clustering dipilih karena komputasinya lebih cepat.

# Insight
**Cluster 0:**

Karakteristik:

*   Rata-rata pelanggan bekerja di bidang swasta/wiraswasta.
*   Rata-rata bukan lulusan universitas.
*   Memiliki pendapatan di bawah rata-rata.
*   Jarang bepergian domestik dan internasional.

Interpretasi: Pelanggan di cluster ini dapat dikategorikan sebagai pelanggan berpenghasilan rendah dengan mobilitas rendah. Cluster ini perlu didorong untuk membeli paket asuransi yang sesuai dengan keuangannya dan fokuskan pada perjalanan domestik.

**Cluster 1:**

Karakteristik:
*   Rata-rata pelanggan bekerja di bidang swasta/wiraswasta.
*   Rata-rata adalah lulusan universitas.
*   Memiliki pendapatan rata-rata.
*   Jarang bepergian domestik dan internasional.

Interpretasi: Pelanggan di cluster ini dapat dikategorikan sebagai pelanggan berpenghasilan sedang dengan mobilitas rendah. Cluster ini memiliki potensi untuk menjadi pelanggan berulang (repeat customer).


**Cluster 2:**

Karakteristik:
*   Rata-rata pelanggan bekerja di bidang swasta/wiraswasta.
*   Rata-rata adalah lulusan universitas.
*   Memiliki pendapatan di atas rata-rata.
*   Sering bepergian domestik dan internasional.

Interpretasi: Pelanggan di cluster ini dapat dikategorikan sebagai pelanggan berpenghasilan tinggi dengan mobilitas tinggi. Cluster ini perlu dipertahankan dan ditingkatkan penjualannya maupun nilai pelanggannya.

**Cluster 3:**

Karakteristik:
*   Rata-rata pelanggan bekerja di pemerintah.
*   Rata-rata adalah lulusan universitas.
*   Memiliki pendapatan di bawah rata-rata.
*   Jarang bepergian domestik dan internasional.

Interpretasi: Sedikit berbeda dengan cluster 0, cluster 3 adalah Pegawai Negeri Sipil dengan mobilitas rendah. Umumnya, PNS sudah memiliki asuransi sendiri sehingga tidak membutuhkan asuransi dari luar lagi. Tujuan menyasar cluster ini adalah untuk mendorong PNS melengkapi paket asuransinya yang sudah ada.

# Business Recommendation
**Cluster 0: Pelanggan Berpenghasilan Rendah dengan Mobilitas Rendah**

* Tawarkan premi yang terjangkau.
* Tawarkan jenis asuransi single trip yang dapat menjamin untuk satu kali perjalanan dalam kurun waktu tertentu.
* Tawarkan jenis asuransi perjalanan domestik.
* Fokus pada manfaat dasar asuransi perjalanan, yaitu mengganti biaya pengobatan dan kecelakaan diri selama perjalanan.
* Jalin kerjasama dengan perusahaan tour & travel dan online booking platform.
* Edukasi pelanggan tentang manfaat asuransi perjalanan dengan Covid cover melalui email, sosial media, dan acara Travel Fair.

**Cluster 1: Pelanggan Berpenghasilan Sedang dengan Mobilitas Rendah**

* Tawarkan promo dan diskon menarik untuk mendorong pembelian.
* Tambahkan manfaat asuransi perjalanan, seperti penundaan/pembatalan perjalanan, keterlambatan/kehilangan bagasi, dan kerusakan/kehilangan barang berharga.
* Tawarkan jenis asuransi perjalanan domestik dan internasional.
* Jalin kerjasama dengan perusahaan tour & travel dan online booking platform.
* Edukasi pelanggan tentang manfaat asuransi perjalanan dengan Covid cover melalui email, sosial media, dan acara Travel Fair.

**Cluster 2: Pelanggan Berpenghasilan Tinggi dengan Mobilitas Tinggi**

* Tawarkan asuransi perjalanan dengan manfaat yang lebih luas, seperti perlindungan gadget, perlindungan terhadap rumah apabila meninggalkan rumah dalam jangka waktu yang cukup lama, dan bantuan hukum jika mengalami masalah hukum di lokasi tujuan.
* Tawarkan perlindungan premium tambahan seperti perlindungan visa, resiko olahraga musim dingin, dan perlindungan kapal pesiar.
* Tawarkan jenis asuransi tahunan, yaitu program asuransi yang dapat menjamin perjalanan sepanjang tahun dengan batasan durasi setiap perjalanannya.
* Iklankan penawaran khusus untuk perjalanan bisnis atau liburan eksklusif melalui email dan sosial media.
* Jalin kerjasama dengan maskapai penerbangan, hotel, dan perusahaan tour & travel untuk menawarkan paket wisata dan asuransi perjalanan yang menarik.
* Buat program loyalitas untuk pelanggan setia yang sering bepergian.

**Cluster 3: Pegawai Negeri Sipil dengan Mobilitas Rendah**

* Beri manfaat tambahan, peningkatan cakupan, atau proses klaim lebih mudah yang tidak tersedia dalam asuransi pemerintah.
* Tawarkan premi yang terjangkau.
* Jelaskan manfaat asuransi perjalanan yang relevan dengan kebutuhan mereka, seperti perlindungan perjalanan dinas dan wisata keluarga.
