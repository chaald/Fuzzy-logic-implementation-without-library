# Fuzzy-logic-implementation-without-library
Implementasi logika fuzzy tanpa library untuk memilih 5 bengkel terbaik dari 100 bengkel.

## Deskripsi Proyek

Proyek ini adalah tugas akhir untuk mata kuliah Kecerdasan Buatan. Tujuannya adalah mengembangkan sistem Inferensi Logika Fuzzy untuk memilih 5 bengkel terbaik dari dataset yang berisi 100 bengkel tanpa menggunakan library logika fuzzy eksternal. Program membaca input dari file bernama bengkel.xlsx dan mengeluarkan 5 bengkel terbaik dengan informasi tentang kualitas layanan, harga, dan skor kelayakan yang diperoleh dari proses defuzzifikasi.

## Fitur
- Membaca data bengkel dari bengkel.xlsx.
- Mengevaluasi setiap bengkel berdasarkan kualitas layanan dan harga menggunakan implementasi Logika Fuzzy khusus.
- Memilih dan menampilkan 5 bengkel terbaik dengan ID mereka, kualitas layanan, informasi harga, dan skor kelayakan.

## Daftar Isi
- Instalasi
- Penggunaan
- Format Data Input
- Sistem Logika Fuzzy
  - Fuzzifikasi
  - Inferensi
  - Defuzzifikasi
- Output

## Instalasi
- Clone repository:
git clone https://github.com/chaald/fuzzy-logic-implementation-without-library.git
- Masuk ke direktori proyek:
cd fuzzy-logic-implementation-without-library
- Install dependencies yang diperlukan:
pip install -r requirements.txt

## Penggunaan
- Letakkan file bengkel.xlsx di direktori proyek.
- Jalankan program utama:
python main.py
- Program akan menampilkan 5 bengkel terbaik dengan ID mereka, kualitas layanan, harga, dan skor kelayakan.

## Format Data Input

File bengkel.xlsx harus memiliki kolom-kolom berikut:
- id: Identifikasi unik untuk setiap bengkel.
- servis: Kualitas layanan yang diberikan oleh bengkel.
- harga: Biaya layanan yang ditawarkan oleh bengkel.

## Sistem Logika Fuzzy
1. Fuzzifikasi: Fuzzifikasi adalah proses mengubah nilai input crisp menjadi himpunan fuzzy. Proyek ini mendefinisikan fungsi keanggotaan fuzzy untuk kualitas layanan dan harga.
2. Inferensi: Inferensi menggunakan aturan fuzzy yang telah ditentukan untuk mengevaluasi nilai input. Aturan fuzzy disimpan dalam sebuah dictionary dan proses inferensi menghitung derajat keanggotaan untuk setiap aturan.
3. Defuzzifikasi: Defuzzifikasi mengubah output fuzzy menjadi skor kelayakan crisp. Proyek ini menggunakan metode centroid untuk menghitung skor kelayakan akhir.

## Output

Program menampilkan 5 bengkel terbaik dengan informasi berikut:
- id: ID bengkel.
- servis: Kualitas layanan yang diberikan.
- harga: Biaya layanan yang ditawarkan.
- skor kelayakan: Skor defuzzifikasi yang mewakili kelayakan bengkel.
Daftar peringkat akhir bengkel disimpan dalam peringkat.xls.
