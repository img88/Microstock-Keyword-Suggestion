# Microstock Keyword Helper
Author: Irfan Muhammad Ghani
Updated: 13 Apr 2021


Pada dasarnya urutan keyword yang digunakan pada metadata gambar sangat menentukan posisi hasil pencarian, dan ini mempengaruhi banyaknya download dan penghasilan.

Tools ini dibuat untuk memudahkan microstocker dalam menganalisa title dan keywords yang akan digunakan di dalam metadata gambar.

Yang dibutuhkan:

- Pandas
- Selenium
- BeautifulSoup
- Driver browser:
    - Edge: https://developer.microsoft.com/en-us/microsoft-edge/tools/webdriver/
    - Chrome: https://chromedriver.chromium.org/downloads
    - Apabila browser yang digunakan bukan di atas, cari dengan kata kunci "nama_browsernya driver"

Cara kerjanya:

- Pastikan telah menginstall library yang diperlukan dan memasukkan driver browser ke variable "driver"
- Masukkan kata kunci pencarian gambar di variable "search_for", dan masukkan jumlah data yg ingin diambil di variable "how_many"
- Sistem akan melakukan scapping data pada halaman pertama pencarian, diantaranya:
    - Title
    - Keywords
    - Jumlah keywords
    - Category
    - Author
    - Jumlah stok Author
    - Link author
    - Link gambar
- Semua data akan disimpan pada dataframe "metadata", dari sini temen-temen bisa menganalisa beberapa hal, semisal keyword apa saja yg paling relevan untuk pencarian tersebut, atau menentukan judul yang cocok untuk gambar yang akan diupload.
- Selain itu, data tersebut akan disimpan dalam format .csv<br/><br/>

Tools ini baru bisa mengambil data dari Shutterstock saja, mungkin jika ada waktu luang akan saya update agar bisa mengambil data dari agensi lainnya, dan menambahkan beberapa fitur otomatis.
