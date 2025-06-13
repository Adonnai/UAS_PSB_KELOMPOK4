# 🔬 Klasifikasi Sel Sumsum Tulang Menggunakan Deep Learning

Proyek ini bertujuan untuk mengklasifikasikan sel-sel sumsum tulang menjadi tujuh tipe morfologi menggunakan jaringan saraf konvolusional (CNN) berbasis ReXNet-150. Model yang telah dilatih kemudian diintegrasikan ke dalam antarmuka web interaktif menggunakan Gradio dan di-deploy melalui Hugging Face Spaces.


## 🧠 Ringkasan

- **Model**: ReXNet-150 (via `timm`)
- **Dataset**: Dataset klasifikasi sel sumsum tulang (Kaggle)
- **Kelas**: BLA, EOS, LYT, MON, NGS, NIF, PMO
- **Deploy**: Gradio + Hugging Face Spaces

## 🚀 Fitur

- Klasifikasi gambar mikroskopis sel sumsum tulang
- Antarmuka berbasis web yang mudah digunakan
- Prediksi 3 kelas teratas dengan nilai probabilitas
- Visualisasi performa model: Loss, Akurasi, dan F1-Score
- Analisis distribusi data kelas dalam bentuk bar chart dan pie chart

## 🖼️ GUI

👉 Coba aplikasi secara langsung: [🔗 Hugging Face Space](https://huggingface.co/spaces/Finpropsmkel3/bone-marrow-classifier-gui/tree/main)

🧠 Untuk Melatih Model Sendiri (Opsional)
Gunakan file bonemarrow.py di Google Colab untuk melatih model menggunakan DataLoader dan kelas visualisasi yang efisien.

📊 Hasil Pelatihan
Akurasi Training: ~96%

Akurasi Validasi: ~79%

F1 Score (Validasi): ~0.79

📚 Referensi
Matek, C., Schwarz, S., Spiekermann, K., & Marr, C. (2021). Human-level recognition of blast cells in acute myeloid leukaemia with convolutional neural networks. Nature Machine Intelligence, 3(3), 251–258. DOI: 10.1038/s42256-021-00336-0
