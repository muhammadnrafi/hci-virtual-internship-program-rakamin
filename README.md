# Business Understanding

**Latar Belakang**  
Latar belakang case study Home Credit Default Risk dapat diawali dengan fenomena yang terjadi di pasar keuangan saat ini, yaitu semakin ketatnya persaingan dalam industri perbankan dan keuangan. Kondisi ini membuat lembaga keuangan semakin memperketat kriteria pemberian kredit. Oleh karena itu, perusahaan perlu menerapkan metode yang lebih cermat dalam menilai risiko kredit dan mengelola risiko tersebut.

Home Credit adalah sebuah perusahaan multinasional yang bergerak di bidang keuangan, yang menyediakan layanan kredit konsumen untuk pembelian barang-barang rumah tangga dan elektronik, seperti telepon seluler, televisi, dan sebagainya. Home Credit memiliki operasi di berbagai negara di seluruh dunia, termasuk di Indonesia.

Sebagai perusahaan keuangan, Home Credit memiliki risiko kredit yang tinggi karena memberikan kredit kepada konsumen yang memiliki kualifikasi yang berbeda-beda, termasuk yang memiliki catatan kredit buruk atau tidak memiliki catatan kredit sama sekali. Oleh karena itu, Home Credit perlu menerapkan metode yang lebih cermat dalam menilai risiko kredit dan mengelola risiko tersebut.

Salah satu metode yang dapat dilakukan oleh Home Credit adalah dengan menggunakan teknologi data mining dan machine learning untuk mengembangkan model prediksi default risk. Dalam hal ini, model prediksi dapat membantu perusahaan dalam menentukan kelayakan dan risiko pemberian kredit kepada calon nasabah.

Dalam case study Home Credit Default Risk, terdapat dataset yang berisi informasi tentang nasabah yang mengajukan kredit dari Home Credit. Dataset tersebut berisi informasi seperti usia, jenis kelamin, tingkat pendidikan, status pernikahan, dan informasi keuangan lainnya. Dengan menggunakan teknik data mining dan machine learning, Home Credit dapat membangun model prediksi default risk yang akurat dan dapat membantu perusahaan dalam mengambil keputusan kredit yang lebih tepat.

Target:  
`0` : Pembayaran Lancar  
`1` : Pembayaran Terkendala (Default)

Data: https://www.kaggle.com/c/home-credit-default-risk

**Goals / Tujuan**  
Pernyataan goals untuk case study Home Credit Default Risk yang bertujuan untuk dapat membedakan kelas positif dan negatif dengan baik dengan ROC AUC serta meminimalisir False Negative rate adalah sebagai berikut:

- Membangun model prediksi default risk yang akurat dengan nilai ROC AUC yang tinggi, yaitu di atas 0.70.
- Meminimalisir risiko kredit yang ditanggung oleh perusahaan dengan mengurangi jumlah nasabah yang default pada pinjaman mereka.
- Memperbaiki efisiensi proses kredit yang dihasilkan dengan model prediksi default risk yang akurat, sehingga perusahaan dapat menilai risiko kredit dengan lebih cepat dan efektif.  

Dengan mencapai goals tersebut, Home Credit dapat meningkatkan kinerja dan efisiensi operasi kredit mereka, serta meningkatkan kepercayaan dan loyalitas nasabah dalam menggunakan layanan mereka.

**Metrik Evaluasi**  
- `ROC AUC`: Dalam kasus Home Credit Default Risk, ROC AUC dapat digunakan untuk mengukur seberapa baik model prediksi dapat membedakan antara nasabah yang berisiko default dan yang tidak berisiko default. Semakin tinggi nilai ROC AUC, semakin baik kemampuan model dalam membedakan kelas positif dan negatif.
    Oleh karena itu, ROC AUC merupakan metrik evaluasi yang penting dalam kasus Home Credit Default Risk, karena dapat membantu perusahaan dalam memilih model prediksi default risk yang terbaik dan dapat meminimalkan risiko kredit yang ditanggung oleh perusahaan.
    
- `False Negative Rate`: Metrik evaluasi yang dapat digunakan untuk mengukur kinerja model dalam memprediksi nasabah yang sebenarnya berisiko default namun diprediksi tidak berisiko default oleh model. False Negative Rate menghitung persentase dari jumlah nasabah yang sebenarnya berisiko default namun diprediksi tidak berisiko default oleh model dibandingkan dengan total jumlah nasabah yang berisiko default. Hal ini perlu diminimalisir untuk mengurangi kerugian pada pihak perusahaan akibat default yang tidak terdeteksi oleh model prediksi. Dalam kasus Home Credit Default Risk, False Negative Rate menjadi metrik evaluasi yang penting untuk diperhatikan, karena dapat membantu perusahaan untuk mengurangi risiko kredit yang diambil dan meningkatkan kepercayaan nasabah.

## Kesimpulan

**Bisnis**  
Berikut adalah beberapa solusi yang dapat dilakukan perusahaan untuk meminimalisir potensi default risk berdasarkan variabel yang telah disebutkan:

1. Pendidikan: Perusahaan dapat mempertimbangkan untuk memberikan diskon bunga atau pinjaman dengan syarat yang lebih baik kepada nasabah yang memiliki pendidikan yang lebih tinggi.

2. Skor kredit: Perusahaan dapat menentukan syarat pinjaman yang lebih ketat untuk nasabah dengan skor kredit rendah. Selain itu, perusahaan juga dapat memberikan penghargaan kepada nasabah dengan skor kredit yang tinggi dengan memberikan diskon bunga atau syarat yang lebih baik.

3. Jenis kredit: Perusahaan dapat mempertimbangkan untuk membatasi jenis kredit tertentu yang memiliki risiko default yang lebih tinggi. Misalnya, perusahaan dapat membatasi pemberian kredit konsumsi dan hanya fokus pada kredit modal kerja.

4. Pekerjaan: Perusahaan dapat mempertimbangkan jenis pekerjaan nasabah sebagai faktor penilaian dalam memberikan kredit. Misalnya, perusahaan dapat memperketat syarat pemberian kredit untuk nasabah yang memiliki jenis pekerjaan dengan risiko default yang lebih tinggi.

5. Saldo yang belum dibayar: Perusahaan dapat mempertimbangkan untuk menawarkan pembayaran cicilan yang lebih fleksibel untuk nasabah yang memiliki saldo yang belum dibayar yang besar.

6. Lama waktu kredit: Perusahaan dapat mempertimbangkan untuk memperpendek jangka waktu kredit agar risiko default dapat diminimalisir.

7. Jenis penghasilan: Perusahaan dapat mempertimbangkan jenis penghasilan nasabah sebagai faktor penilaian dalam memberikan kredit. Misalnya, perusahaan dapat memberikan syarat kredit yang lebih baik kepada nasabah dengan penghasilan yang stabil dan cukup tinggi.

8. Masa kerja: Perusahaan dapat mempertimbangkan masa kerja nasabah sebagai faktor penilaian dalam memberikan kredit. Misalnya, perusahaan dapat memberikan syarat kredit yang lebih baik kepada nasabah dengan masa kerja yang lebih lama karena memiliki penghasilan yang lebih stabil.

**Model**  
Nilai ROC AUC dan recall menunjukkan seberapa baik model dapat membedakan antara kelas default dan non-default. Nilai ROC AUC sebesar 0.755 menunjukkan bahwa model memiliki kemampuan yang cukup baik dalam membedakan antara kelas default dan non-default, dengan 0.5 sebagai nilai ROC AUC yang biasa digunakan sebagai baseline. Namun, nilai ini tidak menjelaskan seberapa akurat model dalam memprediksi kelas default.

Sementara itu, nilai recall sebesar 0.71 menunjukkan bahwa model mampu mengidentifikasi 71% dari total kasus default yang ada di dataset. Namun, nilai precision sebesar 0.15 menunjukkan bahwa dari seluruh prediksi default yang dilakukan oleh model, hanya 15% yang benar-benar merupakan kasus default. Artinya, sebagian besar prediksi default yang dilakukan oleh model adalah false positive, yang dapat menyebabkan kerugian finansial bagi perusahaan.

Dalam konteks risiko default, model yang memiliki nilai recall yang tinggi penting untuk mengidentifikasi sebanyak mungkin kasus default yang ada. Namun, model juga harus memiliki nilai precision yang tinggi untuk meminimalkan false positive dan mencegah perusahaan memberikan kredit kepada peminjam yang berisiko tinggi. Oleh karena itu, perlu dilakukan peningkatan terhadap precision agar model dapat memberikan prediksi yang lebih akurat dan mengurangi risiko default pada perusahaan.



