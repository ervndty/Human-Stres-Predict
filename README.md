# Submission 1: Machine Learning Pipeline - Human Stres Prediction
Nama: Ervin Aditya

Username dicoding: ervin_aditya24

![human resources problems](https://user-images.githubusercontent.com/58927608/232183728-df31ce54-b58c-4163-a563-5df9d3daf167.jpg)

[Sumber Gambar](https://blog.peoplespheres.com/en-us/what-problems-do-human-resources-managers-face-every-day)

| | Deskripsi |
| ----------- | ----------- |
| Dataset | [Human Stres Prediction](https://www.kaggle.com/datasets/kreeshrajani/human-stress-prediction) |
| Masalah | Stres merupakan reaksi fisik dan emosional seseorang terhadap perubahan lingkungan yang menuntut penyesuaian diri. Meskipun stres adalah hal yang wajar dalam kehidupan, jika terlalu berat dan berlangsung lama, dapat berdampak buruk pada kesehatan. |
| Solusi machine learning | Karena stres sulit dikenali hanya dari aktivitas sehari-hari, machine learning dapat dimanfaatkan untuk mendeteksi tanda-tanda stres melalui pola ketikan seseorang di media sosial. |
| Metode pengolahan | Dataset Human Stress Prediction memiliki tujuh fitur, namun dalam proyek ini hanya digunakan fitur text dan label. Fitur lainnya dihapus. Data kemudian dibagi menjadi 80% untuk pelatihan dan 20% untuk evaluasi. Teks diubah menjadi huruf kecil (lowercase), dan label dikonversi ke bentuk angka (integer). |
| Arsitektur model | Model yang digunakan berbasis embedding yang terdiri dari: vectorize_layer, embedding layer dengan dimensi 16, dilanjutkan dengan AveragePooling1D karena data berbentuk teks, lalu dua dense layer berukuran 64 dan 32 dengan aktivasi ReLU, serta sigmoid untuk klasifikasi dua label. Digunakan loss function binary_crossentropy, optimizer Adam, dan metrik BinaryAccuracy. |
| Metrik evaluasi | Metrik evaluasi yang digunakan meliputi: ExampleCount, AUC, FalsePositives, TruePositives, FalseNegatives, TrueNegatives, dan BinaryAccuracy. |
| Performa model | Hasil evaluasi menunjukkan AUC sebesar 82%, example_count sebanyak 575, BinaryAccuracy sebesar 75%, dan loss sebesar 1.364. Nilai False Negative sebanyak 68, False Positive 75, True Negative 201, dan True Positive 231. Performa model masih bisa ditingkatkan karena akurasi belum mencapai 80%. |
