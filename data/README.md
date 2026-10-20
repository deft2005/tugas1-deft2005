
# Data Tugas 1

## Dataset yang Dipilih

Item

Isi

Nama dataset

SFinDSet — Financial Transaction Records

Sumber

[Kaggle — SFinDSet for Systematic Detection of Financial Crimes](https://www.kaggle.com/datasets/muhammadnuraddeenado/sfindset-for-systematic-detection-of-fincrimes)

Lisensi/ketentuan pakai

GNU Lesser General Public License

Ukuran

Dilaporkan memiliki 1.048.575 baris dan berukuran sekitar 112,8 MB. Memenuhi ketentuan lebih dari 1.000.000 baris, dengan catatan jumlah baris aktual perlu diverifikasi setelah mengunduh file.

Periode data

Data transaksi sintetis. Rentang tanggal transaksi belum diverifikasi dan akan ditentukan dari kolom tanggal pada dataset setelah proses profiling.

Unit analisis

Satu record transaksi finansial sintetis.

## Tempat Mencari Dataset

Pilih dataset Indonesia yang legal digunakan, dapat didokumentasikan sumbernya, dan memenuhi batas ukuran tugas.

Situs

Kegunaan

[Satu Data Indonesia](https://data.go.id/)

Portal data terbuka lintas instansi pemerintah Indonesia.

[Badan Pusat Statistik](https://www.bps.go.id/)

Statistik sosial, ekonomi, kependudukan, dan data wilayah.

[BMKG Data Online](https://dataonline.bmkg.go.id/)

Data cuaca, iklim, gempa bumi, dan observasi meteorologi.

[Hugging Face Datasets](https://huggingface.co/datasets)

Dataset publik yang dapat dicari berdasarkan topik, bahasa, atau ukuran.

[Kaggle Datasets](https://www.kaggle.com/datasets)

Katalog dataset publik; periksa lisensi dan dokumentasi pembuatnya.

[Google Dataset Search](https://datasetsearch.research.google.com/)

Mesin pencari untuk menemukan dataset dari berbagai portal.

## Cara Memperoleh Data

1.  Buka [halaman dataset SFinDSet di Kaggle](https://www.kaggle.com/datasets/muhammadnuraddeenado/sfindset-for-systematic-detection-of-fincrimes).
    
2.  Baca deskripsi dataset dan periksa lisensi serta ketentuan penggunaannya.
    
3.  Unduh file dataset ke folder `data/raw/` tanpa mengubah data mentah.
    
4.  Catat nama file, ukuran aktual, jumlah baris, dan checksum SHA-256 bila diperlukan.
    
5.  Identifikasi kolom tanggal dan tentukan rentang periode data melalui profiling.
    
6.  Ubah variabel `DATA_PATH` pada `notebooks/01_data_profiling.ipynb` agar menunjuk ke file dataset yang telah diunduh.
    
7.  Gunakan Polars untuk profiling dan cleaning, serta DuckDB untuk analisis SQL dan `SUMMARIZE`.
    

## Aturan Penyimpanan

-   Jangan commit dataset mentah atau hasil olahan berukuran besar ke Git.
    
-   File pada `data/raw/` adalah data asli dan tidak boleh diubah.
    
-   Simpan hasil transformasi yang dapat direproduksi pada `data/processed/`.
    
-   Dokumentasikan sumber data, lisensi, ukuran file, jumlah baris, serta langkah pengunduhan agar analisis dapat direproduksi.
    
-   Gunakan notebook dan script untuk melakukan transformasi sehingga proses cleaning dapat dijalankan ulang.
    
-   Jangan menyimpulkan adanya transaksi kriminal nyata karena dataset ini bersifat sintetis.