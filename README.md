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

## Usage

This starter project is ready to be used as a foundation for building web applications. The app.py file contains all the Flask routes and logic, making it simple to expand and customize. You can add more templates, routes, or static files as needed.

## Customization
You can easily modify:

 - The HTML structure in `templates/index.html`
 - The styling in `static/style.css`
 - The interactivity in `static/script.js`

Feel free to update the app.py file to add your routes or any additional logic to fit your needs.

## License
This project is licensed under the MIT License.

## Contributing
Feel free to fork this repository and create pull requests if you have improvements or bug fixes. If you have any suggestions, open an issue, and we’ll discuss it!

This project is built with simplicity and efficiency in mind, perfect for quickly starting small web apps or prototypes with minimal overhead.
