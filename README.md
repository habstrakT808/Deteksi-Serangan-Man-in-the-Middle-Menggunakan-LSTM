# Deteksi Serangan Man-in-the-Middle (MitM) pada Jaringan Menggunakan LSTM

## Deskripsi Proyek

Proyek ini bertujuan untuk mendeteksi serangan **Man-in-the-Middle (MitM)** pada jaringan menggunakan pendekatan deep learning dengan algoritma **Long Short-Term Memory (LSTM)**. Model dilatih untuk mempelajari pola dari dataset **CIC-IDS-2017** yang mencakup berbagai serangan jaringan dan lalu lintas jaringan normal.

## Fitur Utama
- **Preprocessing Data**: Data difilter, dibersihkan, dan dinormalisasi untuk memastikan hasil pelatihan yang optimal.
- **Arsitektur LSTM**: Model memanfaatkan LSTM untuk menangkap dependensi jangka panjang dalam data jaringan.
- **Evaluasi Model**: Menggunakan metrik seperti akurasi, precision, recall, dan F1-score untuk menilai performa model.
- **Visualisasi**: Menyediakan berbagai visualisasi seperti loss curve, confusion matrix, dan precision-recall curve untuk analisis hasil.

## Dataset
Dataset yang digunakan adalah **CIC-IDS-2017**, yang terdiri dari berbagai jenis serangan jaringan termasuk MitM. Dataset ini tersedia di [Canadian Institute for Cybersecurity](https://www.unb.ca/cic/datasets/ids-2017.html).

### Proses Data
1. **Pembersihan Data**: Menghapus kolom yang tidak relevan atau memiliki nilai null.
2. **Encoding**: Label diubah menjadi nilai numerik.
3. **Normalisasi**: Fitur dinormalisasi ke rentang [0,1].

## Instalasi dan Persiapan
1. **Kloning Repository**
```bash
$ git clone https://github.com/username/repo-name.git
$ cd repo-name
```

2. **Instalasi Dependencies**
Gunakan file `requirements.txt` untuk menginstal dependensi.
```bash
$ pip install -r requirements.txt
```

3. **Struktur Folder**
```
repo-name/
├── data/
├── models/
├── notebooks/
├── src/
├── requirements.txt
└── README.md
```

4. **Menyiapkan Dataset**
Unduh dataset CIC-IDS-2017 dan letakkan dalam folder `data/`.

## Cara Menjalankan
1. **Pra-Pemrosesan Data**
Jalankan script untuk memproses data.
```bash
$ python src/preprocess_data.py
```

2. **Pelatihan Model**
Latih model menggunakan LSTM.
```bash
$ python src/train_model.py
```

3. **Evaluasi Model**
Evaluasi hasil model menggunakan script evaluasi.
```bash
$ python src/evaluate_model.py
```

## Hasil Visualisasi
- **Loss Curve**: Menunjukkan perubahan loss selama pelatihan.
- **Confusion Matrix**: Menampilkan performa model pada data uji.
- **Precision-Recall Curve**: Analisis lebih lanjut untuk kelas serangan.

## Metrik Evaluasi
| Metric       | Value         |
|--------------|---------------|
| Accuracy     | 99.99%        |
| Precision    | 100.00%       |
| Recall       | 99.33%        |
| F1-Score     | 99.65%        |

## Lisensi
Proyek ini dilisensikan di bawah [MIT License](LICENSE).

## Kontribusi
Kontribusi sangat dihargai! Silakan buat **Pull Request** atau laporkan masalah di **Issues**.

## Kontak
Untuk pertanyaan lebih lanjut, hubungi:
- **Nama**: Hafiyan Al Muqaffi Umary
- **Email**: jhodywiraputra@gmail.com
- **LinkedIn**: [linkedin.com/in/username](https://linkedin.com/in/username)
