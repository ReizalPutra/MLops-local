# Submission 1: Machine Learning Pipeline - Emotion CLassification
Nama: Muhamad Reizal Putra Hidayat

Username dicoding: reizalputra

| | Deskripsi |
| ----------- | ----------- |
| Dataset | [Emotion](https://www.kaggle.com/datasets/nelgiriyewithana/emotions) |
| Masalah | Dalam sebuah platform media sosial terutama twitter(X), sebuah postingan(twit) biasanya berisi sebuah emosi yang menggambarkan suasana hati. emosi ini bisa kita idenfikasi secara manual dengan cara membaca. akan tetapi, cara manual mengahabiskan banyak waktu dan rawan terjadi human error. dengan memahami emosi yang terdapat dalam postingan atau ketikan, kita bisa menggunakannya untuk analisa sentimen untuk keperluan apa saja |
| Solusi machine learning | Dengan menggunakan machine learning, dapat membantu dalam mengidenfikasi atau mengklasifikasikan postingan atau ketikan berdasarkan emosi secara otomatis. hal ini memudahkan dan efisien dibandingkan cara manual|
| Metode pengolahan | Data postingan(twit) twitter akan dipisah menjadi data train dan data evaluasi dengan rasio 80:20, kemudian data akan melalui tahapan validasi untuk analisa dan menemukan anomali pada data.disini terdapat 6 macam emosi yang diwakili oleh angka yaitu 0: 'sadness', 1: 'joy', 2: 'love', 3: 'anger', 4: 'fear', 5: 'surprise'. Tahap selanjutnya data akan diproses agar siap untuk masuk kedalam pelatihan mengunakan model yang telah dibuat. Setelah pelatihan selesai model akan di test dengan cara dikirim pada endpoint dimana model siap dipakai. |
| Arsitektur model | Arsitektur yang digunakan terdiri dari layer Embedding dan 2 layer Dense(64 dan 32) sebagai hidden layer, kemudian fungsi aktivasi pada output layer menggunakan softmax karena dalam kasus ini adalah multi classification dan dengan shape 6, karena terdapat 6 class. |
| Metrik evaluasi | Metrik evaluasi yang digunakan yaitu metrik klasifikasi seperti ExampleCount, AUC, FalsePositives, TruePositives, FalseNegatives, TrueNegatives, dan sparseCategoricalAccuracy. |
| Performa model | Evaluasi model diperoleh yaitu AUC sebesar 99,5%, kemudian example_count 83365, dengan SparseCategoricalAccuracy 89.6%, dan loss sebesar 0.215. Untuk False Negatives 9142, False Positive 7987, True Negative 408838 dan True Positive 74223. |