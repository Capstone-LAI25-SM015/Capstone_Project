# Laporan Proyek - LAI25-SM015

## Domain Proyek

Pertanian merupakan sektor vital bagi ketahanan pangan, tetapi petani sering menghadapi kesulitan dalam mendeteksi penyakit pada tanaman mereka sejak dini. Salah satu tantangan terbesar adalah penyakit daun yang dapat merusak hasil pertanian. Sistem deteksi otomatis yang akurat dapat membantu petani mengidentifikasi penyakit dengan lebih cepat dan lebih akurat, serta meningkatkan produktivitas pertanian.

Proyek ini bertujuan untuk mengembangkan model Jaringan Syaraf Tiruan Konvolusional (CNN) untuk mendeteksi penyakit daun pada 10 jenis tanaman pertanian, termasuk tomat, cabai, kentang, dan lainnya. Model ini dikembangkan menggunakan kumpulan data gambar daun tanaman berlabel, dan dapat memberikan informasi tentang jenis penyakit yang terdeteksi. Dengan sistem ini, petani dapat mengambil tindakan yang lebih cepat dan lebih efektif, sehingga mengurangi kerugian panen.


## Business Understanding

Pada bagian ini, kamu perlu menjelaskan proses klarifikasi masalah.

Bagian laporan ini mencakup:

### Problem Statements

Pernyataan masalah latar belakang:
- Proyek ini dimulai dari pengamatan langsung di lingkungan sekitar yang menunjukkan rendahnya pemahaman petani terhadap penyakit tanaman dan teknologi digital. 


### Goals

Tujuan dari pernyataan masalah:
- Mengembangkan sebuah sistem deteksi penyakit daun tanaman menggunakan Streamlit, yang memanfaatkan teknologi deep learning (Convolutional Neural Networks / CNN). Sistem ini akan mampu mendeteksi jenis penyakit dari gambar daun tanaman secara otomatis.

## Data Understanding
Dataset terdiri dari tanaman Cabai, Jagung, Kembang Kol, Kentang, Labu, Singkong, Terong, Timun, Tomat, dan Padi. Masing-masing berisi 50 data pada setiap penyakit tanaman.

Cabai
[Link Dataset Cabai](https://www.kaggle.com/datasets/ratnasarii/penyakitdauncabai)
1. DaunSehat
2. LeafCurl
3. Yellowwiss

Jagung
[Link Dataset Jagung](https://www.kaggle.com/datasets/ndisan/corn-leaf-disease)
1. Bercak Daun 
2. Daun Sehat 
3. Hawar Daun 
4. Karat Daun 

Kembang Kol
[Link Dataset Kembang Kol](https://www.kaggle.com/datasets/jocelyndumlao/cauliflower-leaf-diseases-datase)
1. Black Rot 
2. Healthy 
3. Insect Hole

Kentang 
[Link Dataset Kentang](https://www.kaggle.com/datasets/nirmalsankalana/potato-leaf-disease-dataset\)
1. Bacteria 
2. Fungi 
3. Healthy 
4. Nematode 
5. Pest 
6. Phytopthora 
7. Virus 

Labu 
[Link Datase Labu](https://www.kaggle.com/datasets/rifat963/pumpkin)
1. Bacterial Leaf Spot
2. Downy Mildew
3. Healthy Leaf
4. Mosaic Disease
5. Powdery Mildew

Singkong
[Link Dataset Singkong](https://www.kaggle.com/datasets/nirmalsankalana/cassava-leaf-disease-classification)
1. Bacterial Blight 
2. Brown Streak Disease 
3. Green Mottle 
4. Healthy
5. Mosaic Disease 

Terong 
[Link Dataset Terong](https://www.kaggle.com/datasets/researchforus/eggplant-leaf-disease-dataset)
1. Healthy Leaf 
2. Insect Pest Disease
3. Leaf Spot Disease
4. Mosaic Virus Disease 
5. Small Leaf Disease 
6. White Mold Disease 
7. Wilt Disease 

Timun
[Link Dataset Timun](https://www.kaggle.com/datasets/sujaykapadnis/cucumber-disease-recognition-dataset)
1. Anthracnose 
2. Bacterial Wilt 
3. Belly Rot 
4. Downy Mildew 
5. Fresh Cucumber 
6. Fresh Leaf 
7. Gummy Stem Blight 
8. Pythium Fruit Rot 

Tomat
[Link Dataset Tomat](https://www.kaggle.com/datasets/charuchaudhry/plantvillage-tomato-leaf-dataset)
Variabel atau fitur pada data :
1. Bacterial Spot 
2. Early Blight
3. Late Blight 
4. Leaf Mold 
5. Septoria Leaf Spot 
6. Spider Mites 
7. Target Spot
8. Yellow Leaf Curl Virus 
9. Mosaic Virus 
10. Healthy 

Padi 
[Link Dataset Padi](https://www.kaggle.com/datasets/nirmalsankalana/rice-leaf-disease-image?)
1. Bacterial Blight 
2. Blast 
3. Brown Spot 
4. Tungro 


## Data Preparation

**Langkah-langkah yang dilakukan :**

* Menyatukan semua case penyakit dalam satu folder.
* Membagi dataset menjadi train, val, dan test untuk tahap pengujian model.

## Modeling

**Model yg diujikan :**

1. MobileNet 
2. VGG16
3. ResNet50
4. InceptionV5

## Evaluation

**Hasil Evaluasi pada masing-masing model :**

1. MobileNet 

| Model             | precision |  recall | f1-score |
| ----------------- | --------- | ------- | -------- |
| accuracy          |           |         |   0.75   |
| macro avg         |   0.79    |  0.75   |   0.74   |
| weughted avg      |   0.79    |  0.75   |   0.75   |

2. VGG16
| Model             | precision |  recall | f1-score |
| ----------------- | --------- | ------- | -------- |
| accuracy          |           |         |   0.53   |
| macro avg         |   0.55    |  0.53   |   0.51   |
| weughted avg      |   0.53    |  0.53   |   0.50   |


3. ResNet50

| Model             | precision |  recall | f1-score |
| ----------------- | --------- | ------- | -------- |
| accuracy          |           |         |   0.74   |
| macro avg         |   0.81    |  0.74   |   0.73  |
| weughted avg      |   0.80    |  0.74   |   0.73   |

4. InceptionV5

| Model             | precision |  recall | f1-score |
| ----------------- | --------- | ------- | -------- |
| accuracy          |           |         |   0.72   |
| macro avg         |   0.77    |  0.72   |   0.70   |
| weughted avg      |   0.77    |  0.72   |   0.70   |


