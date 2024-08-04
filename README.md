# Capstone-Project-Modul-3-E-Commerce-Churn-Analysis
### Outline
* Business Understanding
* Data Understanding & Data Cleaning
* Exploratory Data Analysis
* Feature Engineering
* Hyperparameter Tuning
* Post Modelling
* Conclusion and Recommendation


## Business Understanding
### Latar Belakang

E-commerce adalah semua kegiatan perdagangan yang dilakukan melalui media elektronik. Untuk televisi dan telepon tersedia, tetapi lebih banyak e-commerce terjadi melalui internet. Perkembangan teknologi, khususnya internet, mempengaruhi banyak bidang kehidupan, termasuk ritel. Perdagangan telah berubah dalam hal proses jual beli dan pemasaran produk. Proses perdagangan ini umumnya dikenal sebagai electronic commerce atau e-commerce.

Pengertian e-commerce menurut Laudon & Laudon adalah proses penjualan dan pembelian barang secara elektronik oleh konsumen, yang merupakan transaksi business-to-business dengan perantara komputer, yakni menggunakan jaringan komputer.

David Baum (1999) kemudian juga mendefinisikan e-commerce sebagai seperangkat teknologi dinamis dengan bentuk aplikasi dan proses bisnis yang menghubungkan bisnis, konsumen dan masyarakat melalui e-commerce dalam pertukarang barang, jasa dan informasi secara elektronik

Pemahaman tentang e-commerce ini dapat menyebabkan kesalahpahaman tentang bagaimana sistem e-commerce dan pasar. Istilah e-comerce digunakan untuk menggabarkan semua transaksi yang menggunakan media elektronik.

### Pernyataan masalah

Pelanggan setia yang churn dapat menimbulkan kerugian bagi perusahaan jika tidak ditanggulangi. Oleh karena itu, penting bagi perusahaan untuk mempertahankan keterlibatan pelanggan setia di platform e-commerce. Salah satu cara untuk mencapai hal ini adalah dengan menawarkan promosi. Namun, biaya dan sumber daya yang dikeluarkan mungkin menjadi kurang efektif jika promosi dilakukan tanpa pendekatan strategis. Dalam industri e-commerce, sangat penting untuk memprediksi dan mengatasi churn pelanggan secara akurat untuk mempertahankan pelanggan dan meminimalkan dampak negatif terhadap bisnis pendapatan dan profitabilitas.

### Tujuan

Perusahaan dapat melakukan tindakan preventif dengan memprediksi churn pelanggan. Dengan mengidentifikasi pelanggan yang kemungkinan akan churn, strategi pemasaran dapat ditargetkan dengan lebih efektif. Hal ini dapat mengurangi biaya pemasaran dan meningkatkan keuntungan dengan mempertahankan pelanggan setia. Selain itu, memahami faktor-faktor yang mempengaruhi churn pelanggan dapat memberikan wawasan berharga untuk membuat keputusan strategi pemasaran.

### Pendekatan Analitik

Pendekatan analitik yang dilakukan berupa pembuatan, evaluasi dan implementasi model machine learning klasifikasi yang dapat memprediksi apabila pelanggan akan churn atau tidak berdasarkan riwayat data sebelumnya.

**Metrik Evaluasi**



|       | N-Pred| P-Pred |
| --- | --- | --- |
| **N-Act**     | TP | FP |
| **P-Act**      | FN | TP |

Target:   
0 : Pelanggan tidak churn  
1 : Pelanggan churn

Type 1 error : False Positive  
Konsekuensi: Mengeluarkan biaya untuk pelanggan yang tidak tepat sasaran atau pelanggan yang tidak akan churn. 

Type 2 error : False Negative  
Konsekuensi: Hilangnya pelanggan loyal

Berdasarkan konsekuensinya, langkah yang tepat untuk pemilihan model adalah model yang mengurangi hilangnya pelanggan loyal, tetapi tetap memperhatikan pengeluaran biaya pemasaran untuk pelanggan yang kurang tepat. Recall dan precision yang diseimbangkan akan dari kelas positif (Pelanggan *churn*). Metrik yang akan digunakan adalah Recall. 
