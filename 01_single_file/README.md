# 01: Single-File Web Applications

## Analisis
Percobaan ini mendemonstrasikan struktur paling minimal dari framework Pyramid. Kami menggunakan `pyramid.config.Configurator` untuk memetakan URL root ('/') ke fungsi view `hello_world` secara imperatif. Server dijalankan menggunakan `wsgiref.simple_server` yang merupakan server WSGI standar bawaan Python. Ini membuktikan bahwa Pyramid dapat berjalan tanpa struktur folder yang kompleks (scaffolding) untuk aplikasi mikro.