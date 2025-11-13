# Pyramid Web Framework - Learning Journey

Dokumentasi ini berisi kumpulan kode program tugas tambahan mata kuliah Pemrograman Web. Proyek ini difokuskan pada eksplorasi mendalam kerangka kerja (framework) **Pyramid** menggunakan bahasa pemrograman Python, dimulai dari konfigurasi dasar hingga pembuatan aplikasi web berbasis database dan form validasi.

* **Nama:** Choirunnisa Syawaldina
* **NIM:** 123140018
* **Kelas:** RA
* **Program Studi:** Teknik Informatika, Institut Teknologi Sumatera

---

## Struktur Pembelajaran

Repositori ini dibagi menjadi 18 modul terpisah yang merepresentasikan progresi materi pembelajaran:

### Dasar & Konfigurasi
* 📂 **01_single_file**: Implementasi server WSGI minimal dalam satu berkas.
* 📂 **02_package**: Transformasi skrip tunggal menjadi Python Package terstruktur.
* 📂 **03_configuration**: Eksternalisasi konfigurasi menggunakan `development.ini`.
* 📂 **04_debugtoolbar**: Integrasi alat bantu debugging dan inspeksi request.

### Pengujian (Testing)
* 📂 **05_unit_testing**: Pengujian unit terisolasi menggunakan `pytest`.
* 📂 **06_functional_testing**: Simulasi interaksi pengguna (end-to-end) dengan `WebTest`.

### Routing & Views
* 📂 **07_basic_views**: Penerapan konfigurasi view secara deklaratif (`@view_config`).
* 📂 **09_view_classes**: Penggunaan Class-Based Views untuk logika yang lebih terorganisir.
* 📂 **10_request_response**: Manipulasi objek HTTP Request dan Response serta Redirect.
* 📂 **11_routing**: Pemanfaatan URL Dispatching dengan pola rute dinamis.
* 📂 **15_more_view_classes**: Logika view lanjut untuk menangani banyak aksi dalam satu rute.

### Templating & Static Assets
* 📂 **08_templating**: Pengenalan template engine Chameleon (`.pt`).
* 📂 **12_jinja2**: Migrasi template engine menggunakan Jinja2.
* 📂 **13_static_assets**: Manajemen aset statis (CSS, JS, Gambar).
* 📂 **14_json**: Pembuatan endpoint API dengan output JSON.

### Fitur Lanjut
* 📂 **16_logging**: Implementasi pencatatan log aplikasi untuk monitoring.
* 📂 **17_sessions**: Penyimpanan data sementara (transient) menggunakan Session Factory.
* 📂 **18_forms**: Pembuatan dan validasi formulir HTML menggunakan library `Deform` dan `Colander`.

---

## Panduan Instalasi

Setiap folder merupakan paket Python independen. Untuk menjalankannya, ikuti langkah berikut:

1.  **Persiapan Lingkungan:**
    Pastikan Python 3.x sudah terinstall dan *virtual environment* sudah aktif.

2.  **Instalasi Paket (Editable Mode):**
    Masuk ke direktori modul yang ingin dijalankan, lalu install dependensinya:
    ```bash
    cd [NAMA_FOLDER_TUJUAN]
    pip install -e .
    ```
    *(Gunakan `pip install -e ".[dev]"` jika ingin menjalankan modul testing)*

3.  **Menjalankan Server:**
    Gunakan perintah `pserve` untuk memuat konfigurasi:
    ```bash
    pserve development.ini --reload
    ```

4.  **Akses Aplikasi:**
    Buka browser dan kunjungi: `http://localhost:6543`

---

**Catatan:**
Setiap modul dilengkapi dengan file `README` internal yang menjelaskan detail teknis spesifik dari percobaan tersebut.
