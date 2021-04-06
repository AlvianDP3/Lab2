# Pratikum 2
# Pemrograman Web
``` 
Alvian Dwi Pramono
311910163
TI.19.C1
```
# Modul Praktikum Pemrograman Web
Penulisan Eksternal CSS menggunakan tag <link> menggunakan atribut href untuk merujuk
kepada file css yang diletakkan pada <head> dokumen.
Contoh Eksternal CSS.

# Inline CSS dengan menambahkan kode CSS pada tag HTML sebagai atribut dan value. Penempatan
CSS secara inline hanya akan mempengaruhi satu bagian baris kode.
Contoh Inline CSS.

# CSS Selector
CSS Selector dapat berupa elemen HTML, selector class atau selector id. Penggunaan CSS selector
disesuaikan dengan kebutuhannya. Elemen selector akan berlaku pada semua elemen tersebut.
Untuk class dan id selector, akan berlaku pada elemen yang menggunakan class atau id tersebut.
Elemen Selector dideklarasikan berdasarkan tag HTML.

# Class Selector dideklarasikan dengan menambahkan tanda titk (.) sebelum nama class yang akan
digunakan. Kemudian pada tag HTML ditambahkan atribut class dengan value nama class tanpa
menggunakan titik (.). Satu elemen HTML dapat diberikan lebih dari satu class.
<head>
<style>
body {background-color:blue;}
p {font-size:20px; color:mediumblue;}
</style>
</head>

<head>
<link href="style.css" rel="stylesheet" type="text/css">
</head>

<p style="color:blue; font-size:20px;">Pemrograman Web Semester Ganjil</p>

body {color:blue;}
p {font-family:"sans-serif"}
h1 {text-align:center;color:red';}
p {
text-aign:justify;
color:green;
font-size:12pt;
}

Deklarasi CSS
.merah {color:red;}
.serif {font-family:"sans-serif"}
.rata-tengah {text-align:center; font-size:12pt;}
# Penggunaan CSS
<h1 class="merah">Heading berwarna Merah</h1>
<p class="rata-tengah">Paragraf dengan rata tengah</>
<p class"merah serif">paragraf dengan warna merah dan font serif</>
Modul Praktikum Pemrograman Web

Agung Nugroho (agung@pelitabangsa.ac.id) 14
Universitas Pelita Bangsa, Bekasi
ID Selector dideklarasikan dengan menambahkan tanda # sebelum nama id yang akan digunakan.
Kemudian pada tag HTML ditambahkan atribut id dengan value nama id tanpa menggunakan #.
Satu elemen HTML hanya dapat diberikan satu id.

Instruksi Praktikum
1. Persiapkan text editor misalnya VSCode.
2. Buat file baru dengan nama lab2_css_dasar.html
3. Buat struktur dasar dari dokumen HTML.
4. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
5. Lakukan validasi dokumen css dengan mengakses https://jigsaw.w3.org/css-validator/
Langkah-langkah Praktikum
1. Membuat dokumen HTML
Buatlah dokumen HTML seperti berikut
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>CSS Dasar</title>
</head>
<body>
<header>
<h1>CSS Internal dan <i>Inline CSS</i></h1>
</header>
<nav>
<a href="lab2_css_dasar.html">CSS Dasar</a>
<a href="lab2_css_eksternal.html">CSS Eksternal</a>
<a href="lab1_tag_dasar.html">HTML Dasar</a>
</nav>
<!-- CSS ID Selector -->
<div id="intro">
<h1>Hello World</h1>
<p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman
Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat
adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML
dan CSS.</p>
<!-- CSS Class Selector -->
<a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
</div>
</body>
</html>
Deklarasi CSS
#merah {color:red;}
#serif {font-family:"sans-serif"}
#rata-tengah {text-align:center; font-size:12pt;}
Penggunaan CSS
<h1 id="merah">Heading berwarna Merah</h1>
<p id="rata-tengah">Paragraf dengan rata tengah</>
<p id"serif">paragraf dengan font serif</>
