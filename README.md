# flask-minimal

Flask-minimal merupakan proyek awal berbasis Flask yang dirancang untuk memudahkan dalam membangun aplikasi web secara cepat dan efisien. Proyek ini dibuat dengan ringan dan struktur yang sederhana sehingga semua kode utama disimpan didalam satu file (`app.py`) dan juga sudah dilengkapi dengan template dasar dan file statis untuk memulai pengembangan lebih praktis.


## Fitur
- Aplikasi Flask dalam satu file (`app.py`) untuk memudahkan pengembangan dan meningkatkan produktivitas.
- Struktur templat HTML dasar dengan gaya minimalis dan JavaScript sederhana.
- Pengaturan proyek yang sederhana dan mudah dipahami.
- Mudah disesuaikan untuk mempercepat proses pembuatan aplikasi web.

## Persiapan
```bash
sudo apt update
sudo apt install python3 python3-venv python3-pip -y
```

## Instalasi

1. Klon repositori proyeknya dulu:
   ```bash
   git clone https://github.com/yourusername/flask-minimal.git
   cd flask-minimal
   ```

2. Buat virtual environment (agar lebih rapi dan terpisah):
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```

3. Instal dependensi yang diperlukan:
   ```bash
   pip install -r requirements.txt
   ```

4. Jalankan aplikasinya:
   ```bash
   python app.py
   ```

Aplikasi Flask kamu sudah aktif dan bisa diakses lewat browser dengan membuka alamat:
`http://(ip publik kamu):5000`


## 🔁 Menjalankan Otomatis Setelah Reboot

1. Buat Script Startup
   ```bash
   nano ~/flask-minimal/start-flask.sh
   ```

   Isi:
   ```bash
   #!/bin/bash
   cd ~/flask-minimal
   source venv/bin/activate
   python app.py
   ```

   Simpan dan Beri Izin Eksekusi
   ```bash
   chmod +x ~/flask-minimal/start-flask.sh
   ```

2. Tambahkan ke Crontab
   ```bash
   crontab -e
   ```

   Tambahkan baris ini dibagian bawah
   ```bash
   @reboot /home/ubuntu/flask-minimal/start-flask.sh
   ```
   ganti home dan Ubuntu dengan path sesuai sistem kamu


3. Reboot dan Tes
   ```bash
   sudo reboot
   ```

   Setelah server hidup kembali, akses aplikasi Flask melalui browser:
   ```cpp
   http://<IP-server>:5000
   ```


## 🛡️ Catatan Tambahan (Untuk Server EC2)

Jika menggunakan AWS EC2:
1. Pastikan Port 5000 dibuka di security group
2. Tambahkan rule:
   `Custom TCP → Port 5000 → Source: Anywhere (0.0.0.0/0)`
   

## Penggunaan 

Proyek ini sudah siap digunakan sebagai dasar untuk membangun aplikasi web. File app.py berisi semua rute dan logika dasar Flask, sehingga mudah untuk dikembangkan dan disesuaikan. Anda dapat menambahkan lebih banyak template, rute, atau file statis sesuai kebutuhan.

## Kostumisasi 
Anda dapat dengan mudah mengubah:

 - Struktur HTML di dalam `templates/index.html`
 - Gaya Tampilan (CSS) di dalam `static/style.css`
 - Interaktivitas (JavaScript) di dalam `static/script.js`

Silakan ubah file app.py untuk menambahkan rute baru atau logika tambahan sesuai kebutuhan proyek Anda.

## Lisensi
Proyek ini menggunakan lisensi MIT.

## Kontribusi 
Jangan ragu untuk melakukan forking repositori ini dan membuat permintaan tarik jika Anda memiliki perbaikan atau perbaikan bug. Jika Anda memiliki saran, sampaikan masalah Anda, dan kami akan membahasnya!

Proyek ini dibangun dengan mempertimbangkan kesederhanaan dan efisiensi, cocok untuk memulai aplikasi web kecil atau prototipe dengan cepat dengan overhead minimal.
