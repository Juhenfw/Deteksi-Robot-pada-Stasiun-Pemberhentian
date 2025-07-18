# Pelacakan Robot Berbasis Stasiun

## Deskripsi
**Pelacakan Robot Berbasis Stasiun** adalah sistem yang dirancang untuk mendeteksi dan melacak lokasi **robot Pudu** di berbagai **stasiun** dan merekam data tersebut ke dalam **database** untuk pemantauan lebih lanjut. Sistem ini menggunakan **YOLO** untuk deteksi objek secara real-time dan memanfaatkan **database MySQL** untuk menyimpan data dan log pergerakan robot.

Sistem ini mendeteksi robot yang bergerak melalui berbagai checkpoint stasiun, memverifikasi apakah robot berada di area yang ditentukan, dan merekam status **masuk/keluar** robot di setiap checkpoint. Semua data disimpan dalam **database MySQL**, memungkinkan pemantauan dan analisis pergerakan robot secara terus-menerus.

## Fitur
- **Pelacakan Real-Time**: Mendeteksi robot **Pudu** di beberapa **stasiun** secara real-time menggunakan YOLO.
- **Penyimpanan Data**: Merekam informasi pergerakan robot ke dalam **database MySQL** untuk pemantauan lebih lanjut.
- **Multithreading**: Memproses frame video, deteksi objek, dan penyimpanan data secara bersamaan.
- **Pembersihan Data**: Secara otomatis menghapus data yang sudah kadaluarsa untuk mencegah kebocoran memori.
- **Manajemen Koneksi Database**: Memanfaatkan pooling koneksi MySQL untuk operasi database yang efisien.

## Teknologi yang Digunakan
- **YOLOv11**: Digunakan untuk deteksi objek robot secara real-time dalam aliran video.
- **OpenCV**: Digunakan untuk pemrosesan citra dan tampilan frame video.
- **MySQL**: Digunakan untuk penyimpanan data dan pencatatan pergerakan robot.
- **Python**: Bahasa pemrograman utama yang digunakan untuk mengembangkan sistem ini.
- **Threading**: Memungkinkan pemrosesan paralel untuk frame video dan interaksi dengan database.

## Instalasi
Clone repository ini ke mesin lokal Anda dengan perintah berikut:
```bash
git clone https://github.com/Juhenfw/Deteksi-Robot-pada-Stasiun-Pemberhentian.git
cd Deteksi-Robot-pada-Stasiun-Pemberhentian
```
