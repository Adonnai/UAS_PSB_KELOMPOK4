#  Klasifikasi Sel Sumsum Tulang Menggunakan Deep Learning

Proyek ini bertujuan untuk mengklasifikasikan sel-sel sumsum tulang menjadi tujuh tipe morfologi menggunakan jaringan saraf konvolusional (CNN) berbasis ReXNet-150. Model yang telah dilatih kemudian diintegrasikan ke dalam antarmuka web interaktif menggunakan Gradio dan di-deploy melalui Hugging Face Spaces.

# Tentang Dataset 
Dataset yang digunakan merupakan data gambar dari sel darah putih yang sudah dipisahkan ke dalam 7 kelompok berdasarkan kelompok jenis sel (6) dan satu mewakili kelompok sel tidak terdeteksi. Pembagian kelompok dataset sebagai berikut:

- BLA - Blast
- EOS - Eosinophil
- LYT - Lymphocyte
- MON - Monocyte
- NGS - Segmented Neutrophil
- NIF - Not Identifiable
- PMO - Promyelocyte
Jumlah dataset setiap kelompok adalah 500, jadi total dataset yang digunakan untuk proses training model adalah adalah 3500 gambar.

Sumber asli dari dataset ini adalah TCIA (The Cancer Imaging Archive. Dilakukan pengambilan data di Munich Leukemia Laboratory (MLL), dipindai menggunakan peralatan yang dikembangkan di Fraunhofer IIS, dan diproses lebih lanjut menggunakan perangkat lunak yang dikembangkan di Helmholtz Munich[]. Diperoleh lebih dari 170.000 sel yang telah dianonimkan dan dianotasi oleh ahli dari apusan sumsum tulang 945 pasien. Sel-sel ini diwarnai menggunakan pewarnaan May-Grünwald-Giemsa/Pappen- heim. Diagnosis dalam kelompok pasien ini mencakup berbagai penyakit hematologi.


  Ringkasan

- **Model**: ReXNet-150 (via `timm`)
- **Dataset**: Dataset klasifikasi sel sumsum tulang (Kaggle)
- **Kelas**: BLA, EOS, LYT, MON, NGS, NIF, PMO
- **Deploy**: Gradio + Hugging Face Spaces

Fitur

- Klasifikasi gambar mikroskopis sel sumsum tulang
- Antarmuka berbasis web yang mudah digunakan
- Prediksi 3 kelas teratas dengan nilai probabilitas
- Visualisasi performa model: Loss, Akurasi, dan F1-Score
- Analisis distribusi data kelas dalam bentuk bar chart dan pie chart

 Hasil Pelatihan

- Akurasi Training: ~96%
- Akurasi Validasi: ~79%
- F1 Score (Validasi): ~0.79

## GUI

 Coba aplikasi secara langsung: 
[🔗 Hugging Face Space](https://huggingface.co/spaces/Finpropsmkel3/bone-marrow-classifier-gui/tree/main)

## Lampiran Tautan

### Kode Program Kami: 
[🔗 Google Colab](https://colab.research.google.com/drive/1hjX2By_O8tePe4ajHOs55wlN7ha3fdku?usp=sharing)

### Dataset: 
[🔗 For Training](https://drive.google.com/drive/folders/1ID8L4sfX80BjmAtt9jvzUAiP5NjFhVB0?usp=sharing) 
[🔗 For GUI](https://drive.google.com/drive/folders/15yEDcphooLdY2yXLDGBgi0s6OFrI1iil?usp=sharing)



### Referensi:

- Matek, C., Schwarz, S., Spiekermann, K., & Marr, C. (2021). Human-level recognition of blast cells in acute myeloid leukaemia with convolutional neural networks. Nature Machine Intelligence, 3(3), 251–258. DOI: 10.1038/s42256-021-00336-0
- Matek, C., Krappe, S., Münzenmayer, C., Haferlach, T., & Marr, C. (2021). An Expert-Annotated Dataset of Bone Marrow Cytology in Hematologic Malignancies [Data set]. The Cancer Imaging Archive. https://doi.org/10.7937/TCIA.AXH3-T579
- Matek, C., Krappe, S., Münzenmayer, C., Haferlach, T., and Marr, C. (2021). Highly accurate differentiation of bone marrow cell morphologies using deep neural networks on a large image dataset. https://doi.org/10.1182/blood.2020010568
- D. Roy, “bone-marrow-cell-classification,” Kaggle.com, 2021, doi: https://doi.org/10.7937/TCIA.AXH3-T579.



