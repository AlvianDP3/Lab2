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
# Modul Praktikum Pemrograman Web
ID Selector dideklarasikan dengan menambahkan tanda # sebelum nama id yang akan digunakan.
Kemudian pada tag HTML ditambahkan atribut id dengan value nama id tanpa menggunakan #.
Satu elemen HTML hanya dapat diberikan satu id.

### 1. Membuat dokumen HTML
Buatlah dokumen HTML seperti berikut

```
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
```

Modul Praktikum Pemrograman Web

Selanjutnya buka pada brwoser untuk melihat hasilnya.

![Contoh1](https://user-images.githubusercontent.com/56244029/113761133-4cace600-9741-11eb-8fc9-7af8eb5a59a4.png)


### 2. Mendeklarasikan CSS Internal
Kemudian tambahkan deklarasi CSS internal seperti berikut pada bagian head dokumen.

```
<head>
<title>CSS Dasar</title>
<style>
body {
font-family:'Open Sans', sans-serif;
}
header {
min-height: 80px;
border-bottom:1px solid #77CCEF;
}
h1 {
font-size: 24px;
color: #0F189F;
text-align: center;
padding: 20px 10px;
}
h1 i {
color:#6d6a6b;
}
</style>
</head>
```

Selanjutnya simpan perubahan yang ada, dan lakukan refresh pada browser untuk melihat hasilnya.

![Contoh2](https://user-images.githubusercontent.com/56244029/113763698-2e94b500-9744-11eb-98a1-51d44d762a93.jpg)

### 3. Menambahkan Inline CSS

```
<p style="text-align: center; color: #ccd8e4;">
```

Simpan kembali dan refresh kembali browser untuk melihat perubahannya.

![Contoh3](https://user-images.githubusercontent.com/56244029/113765023-f1312700-9745-11eb-9081-ab31f01026b3.jpg)

# 4. Membuat CSS Eksternal
Buatlah file baru dengan nama style_eksternal.css kemudian buatlah deklarasi CSS seperti berikut.

```
nav {
background: #20A759;
color:#fff;
padding: 10px;
}
nav a {
color: #fff;
text-decoration: none;
padding:10px 20px;
}
nav .active,
nav a:hover {
background: #0B6B3A;
}
```

Kemudian tambahkan tag <link> untuk merujuk file css yang sudah dibuat pada bagian <head>

```
<head>
<!-- menyisipkan css eksternal -->
<link rel="stylesheet" href="style_eksternal.css" type="text/css">
</head>
```

Selanjutnya refresh kembali browser untuk melihat perubahannya.

![contoh4](https://user-images.githubusercontent.com/56244029/113767920-6f42fd00-9749-11eb-902a-b5f748c8048a.jpg)

# 5. Menambahkan CSS Selector
Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file
style_eksternal.css, tambahkan kode berikut.

```
/* ID Selector */
#intro {
background: #418fb1;
border: 1px solid #099249;
min-height: 100px;
padding: 10px;
}
#intro h1 {
text-align: left;
border: 0;
color: #fff;
}
/* Class Selector */
.button {
padding: 15px 20px;
background: #bebcbd;
color: #fff;
display: inline-block;
margin: 10px;
text-decoration: none;
}
.btn-primary {
background: #E42A42;
}
```

Kemudian simpan kembali dan refresh browser untuk melihat perubahannya.

![contoh5](https://user-images.githubusercontent.com/56244029/113768567-30617700-974a-11eb-86f4-c2eaaee406fe.jpg)

# Pertanyaan dan Tugas
1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS
dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan
penjelasannya!
3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada
elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan
penjelasan dan contohnya!
4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut
terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser?
Berikan penjelasan dan contohnya! ( <p id="paragraf-1" class="text-paragraf"> )

# jawaban

1. Kita bisa memformat tampilan halaman web menggunakan HTML, namun cara ini sudah tidak digunakan lagi. Kita bisa memformat tampilan halaman web mengguankan CSS. karena kita memisahkan fungsional dari HTML, CSS, dan JavaScript sesuai tujuan masing-masing.
HTML digunakan untuk membuat kerangka website, CSS digunakan untuk membuat tampilan website, JavaScript digunakan untuk membuat website menjadi interaktif.

2. <h1>rancangan website dasar<h1> Penjelasan Satu elemen H1
<h2>HTML</h2> Penjelasan Elemen H2 sebanyak yang dibutuhkan untuk menunjukkan bagian pada halaman (Anda hanya membutuhkan satu, dua, atau tiga bila halaman ringkas.

3. Opsi 1 – Internal CSS
Kode CSS internal diletakkan di dalam bagian <head> pada halaman. Class dan ID bisa digunakan untuk merujuk pada kode CSS, namun hanya akan aktif pada halaman tersebut. Style CSS yang dipasang dengan metode ini akan di-download setiap kali halaman dipanggil, jadi ini akan meningkatkan kecepatan akses. Namun, ada beberapa case dimana penggunaan internal stylesheet justru berguna. Salah satu contohnya adalah untuk mengirimkan template halaman ke seseorang – karena semuanya bisa terlihat dalam 1 halaman, maka akan lebih mudah untuk melihat previewnya. CSS internal diletakkan di dalam tag <style></style>. Contohnya:

<head>
  <style type="text/css">
    p {color:white; font-size: 10px;}
    .center {display: block; margin: 0 auto;}
    #button-go, #button-back {border: solid 1px black;}
  </style>
</head>
Manfaat internal CSS:

Perubahan hanya terjadi pada 1 halaman
Class dan ID bisa digunakan oleh internal stylesheet
Tidak perlu meng-upload beberapa file karena HTML dan CSS bisa digunakan di file yang sama.
Kekurangan menggunakan Internal CSS:

Meningkatkan waktu akses website
Perubahan hanya terjadi pada 1 halaman – tidak efisien bila Anda ingin menggunakan CSS yang sama pada beberapa file.
Cara menambahkan internal CSS ke halaman HTML
1. Buka file HTML Anda dengan menggunakan text editor. Jika halaman sudah di-upload ke hosting, Anda bisa menggunakan text editor yang telah disediakan oleh hosting Anda. Jika Anda memiliki file HTML di komputer Anda, Anda bisa menggunakan text editor apapun untuk meng-edit dan kemudian meng-upload file ke akun hosting Anda menggunakan aplikasi FTP.

2. Temukan bagian awal kode <head> dan tambahkan kode berikut ini di bawahnya:

<style type="text/css">
3. Pada baris baru, tambahkan rule CSS:

body {
    background-color: blue;
}
h1 {
    color: red;
    padding: 60px;
}
4. Setelah Anda menambahkan rule CSS, tambahkan tag penutup:

</style>
Nantinya file HTML yang sudah ditambahkan style CSS akan terlihat seperti ini:

<!DOCTYPE html>
<html>
<head>
<style>
body {
    background-color: blue;
}
h1 {
    color: red;
    padding: 60px;
} 
</style>
</head>
<body>
 
<h1>Hostinger Tutorials</h1>
<p>This is our paragraph.</p>
 
</body>
</html>
Opsi 2 – External CSS
Salah satu cara yang paling nyaman untuk menambahkan CSS ke website Anda adalah dengan menghubungkannya ke file .CSS eksternal. Dengan cara tersebut, perubahan apapun yang Anda buat pada file CSS akan tampil pada website Anda secara keseluruhan. File CSS eksternal biasanya diletakkan setelah bagian <head> pada halaman:

<head>
  <link rel="stylesheet" type="text/css" href="style.css" />
</head>
Dalam contoh diatas, file style.css berisikan semua rule. Contohnya:

.xleftcol {
   float: left;
   width: 33%;
   background:#809900;
}
.xmiddlecol {
   float: left;
   width: 34%;
   background:#eff2df;
}
Manfaat CSS eksternal:

Ukuran file HTML menjadi lebih kecil dan strukturnya lebih rapi
Kecepatan loading menjadi lebih cepat
File CSS yang sama bisa digunakan di banyak halaman.
Kekurangan CSS eksternal:

Halaman belum tampil secara sempurna hingga file CSS selesai dipanggil.
Opsi 3 – Inline CSS
Inline CSS digunakan untuk tag HTML tertentu. Atribut <style> digunakan untuk memberikan style ke tag HTML tertentu. Cara ini kurang direkomendasikan, karena setiap tag HTML malah harus diberikan style masing-masing. Anda akan lebih sulit dalam mengatur website jika hanya menggunakan inline CSS. Namun, di beberapa situasi justru inline CSS menjadi berguna. Contohnya, pada saat Anda tidak memiliki akses ke file CSS atau harus mengubah style untuk 1 elemen saja.
Contoh halaman HTML dengan inline CSS adalah seperti berikut:

<!DOCTYPE html>
<html>
<body style="background-color:black;">
 
<h1 style="color:white;padding:30px;">Hostinger Tutorials</h1>
<p style="color:white;">Something usefull here.</p>
 
</body>
</html>
Manfaat Inline CSS:

Berguna jika Anda ingin menguji dan melihat perubahan
Berguna untuk perbaikan cepat
Permintaan HTTP yang lebih kecil
Kekurangan inline CSS:

Inline CSS harus diterapkan pada setiap elemen
