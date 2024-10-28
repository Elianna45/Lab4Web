# web4lab
<h2>1. Membuatlab4_box.htm</h2>

         <!DOCTYPE html>
             <html lang="en">
             <head>
              <meta charset="UTF-8">
              <meta name="viewport" content="width=device-width, initial-scale=1.0">
              <title>Box Element</title>
             </head>
             <body>
              <header>
              <h1>Box Element</h1>
              </header>
             </body>
             </html>
   
![image](https://github.com/user-attachments/assets/27a78d8f-46c4-4ffb-a8a9-14e6fb1a0195)

<br>

<h2>2. Membuat Box Element</h2>

    <section>
     <div class="div1">Div 1</div>
     <div class="div2">Div 2</div>
     <div class="div3">Div 3</div>
    </section>

<h2>Menambahkan CSS Float Property</h2>

    <style>
     div {
     float:left;
     padding: 10px;
     }
     .div1 {
     background: red;
     }
     .div2 {
     background: yellow;
     }
     .div3 {
     background: green;
     }
    </style>

![image](https://github.com/user-attachments/assets/0cf8960b-fdda-4d42-8d90-1ea48564b4b3)


  Tiga kotak (div1, div2, div3) yang berwarna merah, kuning, dan hijau diatur agar 
  sejajar secara horizontal dengan menggunakan properti float.
<br>

<h2>3. Mengatur Clearfix Element</h2>

    <section>
     <div class="div1">Div 1</div>
     <div class="div2">Div 2</div>
     <div class="div3">Div 3</div>
     <div class="div4">Div 4</div>
    </section>

  ![image](https://github.com/user-attachments/assets/c9d82f56-b393-4cb8-adeb-df13a63396e6)

<br>

<h2>Membuat Layout Sederhana</h2>

    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Layout Sederhana</title>
        <link rel="stylesheet" href="style.css">
    </head>
    <body>
        <div id="container">
    
        
    </body>
    </html>
    
 Menambahkan kotak keempat (div4) dengan warna biru yang diatur menggunakan properti clear untuk menghentikan efek float dari elemen sebelumnya, sehingga kotak tersebut muncul di bawahnya alih-alih di samping. Ini berfungsi untuk mengatur aliran tata letak dalam desain halaman.

<br>

<h2>Kemudian buat kerangka layout dengan semantics element seperti berikut</h2>

    <header>
     <h1>Layout Sederhana</h1>
    </header>
    <nav>
     <a href="home.html" class="active">Home</a>
     <a href="artikel.html">Artikel</a>
     <a href="about.html">About</a>
     <a href="kontak.html">Kontak</a>
    </nav>
    <section id="hero"></section>
    <section id="wrapper">
     <section id="main"></section>
     <aside id="sidebar"></aside>
    </section>
    <footer>
     <p>&copy; 2021 - Universitas Pelita Bangsa</p>
    </footer>

![image](https://github.com/user-attachments/assets/1553bbc1-8114-4142-be88-f1207fe17d13)

dalam file HTML, elemen-elemen semantik seperti <header>, <nav>, dan <footer> digunakan untuk membuat kerangka dasar tata letak halaman. Elemen <nav> berfungsi untuk navigasi, sementara <section> digunakan untuk menempatkan konten utama (#main) dan sidebar (#sidebar). Elemen ini membantu menjaga struktur halaman tetap bersih dan terorganisir.
<br>

<h2>Kemudian tambahkan kode CSS untuk membuat layoutnya</h2>

    /* import google font */
    @import
    url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
    @import
    url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap');
    /* Reset CSS */
    * {
        margin: 0;
        padding: 0;
    }
    body {
        line-height:1;
        font-size:100%;
        font-family:'Open Sans', sans-serif;
        color:#5a5a5a;
    }
    #container {
        width: 980px;
        margin: 0 auto;
        box-shadow: 0 0 1em #cccccc;
    }
    /* header */
    header {
        padding: 20px;
    }
    header h1 {
        margin: 20px 10px;
        color: #b5b5b5;
    }

![image](https://github.com/user-attachments/assets/bcc5ba18-25dc-40b4-bf93-2c4325563f28)

Mengimpor font Google Open Sans untuk diterapkan di seluruh halaman. Selanjutnya, menggunakan "Reset CSS" untuk menghapus margin dan padding default dari semua elemen, sehingga memberikan kontrol penuh atas tata letak. Properti body menetapkan font dasar, ukuran teks, dan warna teks default. Bagian #container mengatur lebar halaman menjadi 980px, dipusatkan dengan margin otomatis, serta ditambahkan efek bayangan halus. Pada header, padding ditambahkan, dan warna teks judul (h1) diatur menjadi abu-abu terang (#b5b5b5), sehingga memberikan tampilan yang bersih dan rapi.

<br>

<h2>Membuat Navigasi</h2>

    /* navigasi */
    nav {
     display: block;
     background-color: #1f5faa;
    }
    nav a {
     padding: 15px 30px;
     display: inline-block;
     color: #ffffff;
     font-size: 14px;
     text-decoration: none;
     font-weight: bold;
    }
    nav a.active,
    nav a:hover {
     background-color: #2b83ea;
    }

![image](https://github.com/user-attachments/assets/e928646a-8163-4147-8558-f9ef398e82cf)

Kode ini mengatur gaya untuk elemen navigasi. Navigasi memiliki latar belakang berwarna biru gelap (#1f5faa), dan tautan (link) ditampilkan sebagai blok inline dengan padding, serta teks berwarna putih. Saat tautan aktif atau ketika di-hover, latar belakangnya berubah menjadi biru yang lebih terang (#2b83ea) untuk memberikan efek interaktif.

<br>

<h2>Membuat Hero Panel</h2>

    <section id="hero">
     <h1>Hello World!</h1>
     <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
    elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
    vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
    pretium ac.</p>
     <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
    </section>

CSS

    /* Hero Panel */
    #hero {
     background-color: #e4e4e5;
     padding: 50px 20px;
     margin-bottom: 20px;
    }
    #hero h1 {
     margin-bottom: 20px;
     font-size: 35px;
    }
    #hero p {
     margin-bottom: 20px;
     font-size: 18px;
     line-height: 25px;
    }


![image](https://github.com/user-attachments/assets/edb2206e-5932-43fe-849e-112f6987d16d)

Kode ini membuat Hero Panel, sebuah elemen yang mencolok di halaman web. Bagian HTML menggunakan elemen <section> dengan ID hero, yang berisi judul besar, paragraf, dan tombol "Learn more". Dalam CSS, panel ini memiliki latar belakang berwarna abu-abu terang (#e4e4e5), dengan padding yang luas untuk memberikan ruang, serta margin bawah untuk memisahkannya dari elemen lainnya.

<br>

<h2>Mengatur Layout Main dan Sidebar</h2>

    /* main content */
    #wrapper {
     margin: 0;
    }
    #main {
     float: left;
     width: 640px;
     padding: 20px;
    }
    /* sidebar area */
    #sidebar {
     float: left;
     width: 260px;
     padding: 20px;
    }


<h2>Membuat Sidebar Widget</h2>

    <aside id="sidebar">
      <div class="widget-box">
        <h3 class="title">Widget Header</h3>
        <ul>
          <li><a href="#">Widget Link</a></li>
          <li><a href="#">Widget Link</a></li>
          <li><a href="#">Widget Link</a></li>
          <li><a href="#">Widget Link</a></li>
          <li><a href="#">Widget Link</a></li>
        </ul>
      </div>
      <div class="widget-box">
        <h3 class="title">Widget Text</h3>
        <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt
        arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer
        pharetra est nunc, nec pretium nunc pretium ac.</p>
      </div>
    </aside>
    
<h2>Menambahkan CSS</h2>


    /* widget */
    .widget-box {
     border:1px solid #eee;
     margin-bottom:20px;
    }
    .widget-box .title {
     padding:10px 16px;
     background-color:#428bca;
     color:#fff;
    }
    .widget-box ul {
     list-style-type:none;
    }
    .widget-box li {
     border-bottom:1px solid #eee;
    
    
![image](https://github.com/user-attachments/assets/3478c99d-952f-4dbc-b8a3-62aeead93806)

Kode ini membuat sebuah Sidebar Widget yang terdiri dari dua bagian. Bagian pertama adalah daftar tautan dengan judul Widget Header, sementara bagian kedua menyajikan teks deskriptif dengan judul Widget Text. Dalam CSS, setiap widget memiliki batas tipis (1px solid #eee) dan margin bawah untuk memberikan pemisahan visual antar widget. Judul widget (.title) memiliki latar belakang berwarna biru (#428bca) dan teks berwarna putih, sedangkan tautan diatur dengan padding dan warna abu-abu. Saat tautan di-hover, latar belakangnya berubah menjadi abu-abu muda untuk memberikan efek interaktif.

<br>

<h2>Mengatur Footer</h2>


    /* footer */
    footer {
     clear:both;
     background-color:#1d1d1d;
     padding:20px;
     color:#eee;
    }

 ![image](https://github.com/user-attachments/assets/870006e8-71a3-4f33-8e66-279a47d72061)

  <h2>Menambahkan Elemen lainnya pada Main Content</h2>

      <section id="main">
     <div class="row">
     <div class="box">
     <img src="https://dummyimage.com/120/db7d25/fff.png" alt=""
    class="image-circle">
     <h3>Heading</h3>
     <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
    euismod.</p>
     <a href="#" class="btn btn-default">View detail</a>
     </div>
     <div class="box">
     <img src="https://dummyimage.com/120/3e73e6/fff.png" alt=""
    class="image-circle">
     <h3>Heading</h3>
     <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
    euismod.</p>
     <a href="#" class="btn btn-default">View detail</a>
     </div>
     <div class="box">
     <img src="https://dummyimage.com/120/71e6d4/fff.png" alt=""
    class="image-circle">
     <h3>Heading</h3>
     <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
    euismod.</p>
     <a href="#" class="btn btn-default">View detail</a>
     </div>
     </div>
    </section>

CSS

    /* box */
    .box {
      display:block;
      float:left;
      width:33.333333%;
      box-sizing:border-box;
      -moz-box-sizing:border-box;
      -webkit-box-sizing:border-box;
      padding:0 10px;
      text-align:center;
    }
    .box h3 {
      margin: 15px 0;
    }
    .box p {
      line-height: 20px;
      font-size: 14px;
      margin-bottom: 15px;
    }
    box img {
      border: 0;
      vertical-align: middle;
    }
    .image-circle {
      border-radius: 50%;
    }
    .row {
      margin: 0 -10px;
      box-sizing: border-box;
      -moz-box-sizing: border-box;
      -webkit-box-sizing: border-box;
    }
    .row:after, .row:before,
    .entry:after, .entry:before {
      content:'';
      display:table;
    }
    .row:after,
    .entry:after {
      clear:both;
    }
    
  ![image](https://github.com/user-attachments/assets/2da06e21-f0b9-4036-a6f4-1f6c8d934676)
Kode ini menambahkan elemen tambahan pada Konten Utama berupa tiga kotak yang berisi gambar, judul, paragraf, dan tombol tautan. Setiap kotak diatur dalam satu baris, dengan gambar berbentuk lingkaran (.image-circle) dan konten yang tersusun rapi dalam proporsi sepertiga dari lebar kontainer. CSS memastikan tata letak yang responsif dengan menggunakan properti float, box-sizing, dan pengaturan margin untuk menjaga jarak antar elemen. Setiap kotak memiliki teks yang rata tengah dan tombol yang disesuaikan untuk navigasi.

<br>

<h2>Menambahkan Content Artikel</h2>

         <hr class="divider" />
         <article class="entry">
          <h2>First featurette heading.</h2>
          <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
         elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
         vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
         pretium ac.</p>
         </article>
         <hr class="divider" />
         <article class="entry">
          <h2>First featurette heading.</h2>
          <img src="https://dummyimage.com/150/7b8a70/fff.png" alt=""
         class="right-img">
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
         elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
         vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
         pretium ac.</p>
         </article>

CSS

         .divider {
             border:0;
             border-top:1px solid #eeeeee;
             margin:40px 0;
             }
             /* entry */
             .entry {
             margin: 15px 0;
             }
             .entry h2 {
             margin-bottom: 20px;
         }
         .entry p {
             line-height: 25px;
         }
         .entry img {
             float: left;
             border-radius: 5px;
             margin-right: 15px;
         }
         .entry .right-img {
             float: right;
         }

![image](https://github.com/user-attachments/assets/62434a1c-2ae5-4bad-95cb-75a60538976f)


Kode ini menambahkan konten artikel ke dalam tata letak dengan tiga elemen artikel (<article>) yang masing-masing mencakup judul, gambar, dan paragraf. Setiap artikel dipisahkan oleh garis horizontal (<hr>) yang menggunakan kelas divider untuk menciptakan tampilan yang bersih. Gambar dalam artikel diatur untuk mengalir ke kiri atau kanan teks, dengan CSS yang mengatur margin dan border-radius, sehingga menciptakan tampilan yang rapi dan terorganisir. Desain ini memastikan bahwa teks mudah dibaca berkat pengaturan line-height dan margin yang sesuai pada elemen teks.

<br>

<h1>Jawaban dan Tugas</h1>

<h2>1. Tambahkan Layout untuk menu About</h2>

    <!DOCTYPE html>
    <html lang="id">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>About Us & Portfolio</title>
        <link rel="stylesheet" href="lab1-web-main.css">
    </head>
    <body>
    
      <header>
        <h1>About Us</h1>
      </header>
            <div class="container">
                <p>Kami adalah tim profesional yang berdedikasi dalam memberikan solusi kreatif dan inovatif untuk memenuhi kebutuhan klien kami. Kami memiliki berbagai pengalaman dalam mengerjakan proyek-proyek di berbagai bidang.</p>
            </div>
        </section>
    
    
        <section id="portofolio">
            <div class="container">
                <h2>Our Portofolio</h2>
                <div class="portofolio-grid">
                    <div class="portofolio-item">
                        <img src="project1.jpg" alt="Proyek 1">
                        <h3>Proyek 1</h3>
                        <p>Deskripsi singkat tentang proyek 1.</p>
                    </div>
                    <div class="portofolio-item">
                        <img src="project2.jpg" alt="Proyek 2">
                        <h3>Proyek 2</h3>
                        <p>Deskripsi singkat tentang proyek 2.</p>
                    </div>
                    <div class="portofolio-item">
                        <img src="project3.jpg" alt="Proyek 3">
                        <h3>Proyek 3</h3>
                        <p>Deskripsi singkat tentang proyek 3.</p>
                    </div>
                </div>
            </div>
        </section>
    
    </body>
    </html>


CSS

    * {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
    }
    
    body {
        font-family: Arial, sans-serif;
        line-height: 1.6;
    }
    
    .container {
        width: 80%;
        margin: auto;
    }
    
    h1, h2 {
        text-align: center;
        margin-bottom: 1rem;
    }
    #about {
        padding: 20px;
    }
    
    #about p {
        max-width: 300px;
        margin: auto;
        font-size: 1.1rem;
        color: #333;
    }
    
    #portofolio {
        padding: 2rem 0;
    }
    
    .portofolio-grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
        gap: 1rem;
    }
    
    .portofolio-item {
        background: #fff;
        border: 1px solid #ddd;
        padding: 1rem;
        text-align: center;
    }
    
    .portofolio-item img {
        width: 100%;
        height: auto;
    }
    
    .portofolio-item h3 {
        margin-top: 1rem;
        font-size: 1.2rem;
        color: #333;
    }
    
    .portofolio-item p {
        font-size: 0.9rem;
        color: #666;
    }

![image](https://github.com/user-attachments/assets/bf7d7089-15cb-4ed2-8798-89df51985818)

Kode ini menciptakan halaman "About" yang informatif dan terstruktur dengan baik, menampilkan deskripsi perusahaan dan portofolio proyek yang mudah diakses. Desain responsif berkat penggunaan CSS Flexbox memastikan bahwa konten akan terlihat baik di berbagai ukuran layar.

<br>

<h2>2. 2. Menambahkan Layout untuk Menu Contact</h2>

    <!DOCTYPE html>
    <html lang="id">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Contact Us</title>
        <link rel="stylesheet" href="lab1-web-main.css">
    </head>
    <body>
    
        <section id="contact">
            <div class="container">
                <h2>Contact Us</h2>
                <p>Jika Anda memiliki pertanyaan atau ingin bekerja sama dengan kami, jangan ragu untuk menghubungi kami melalui formulir di bawah ini.</p>
                
                <form action="#" method="post">
                    <label for="name">Nama</label>
                    <input type="text" id="name" name="name" required>
    
                    <label for="email">Email</label>
                    <input type="email" id="email" name="email" required>
    
                    <label for="message">Pesan</label>
                    <textarea id="message" name="message" rows="5" required></textarea>
    
                    <button type="submit">Kirim Pesan</button>
                </form>
            </div>
        </section>
    
    </body>
    </html>


CSS

    * {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
    }
    
    body {
        font-family: Arial, sans-serif;
        line-height: 1.6;
    }
    
    .container {
        width: 80%;
        margin: auto;
    }
    
    h2 {
        text-align: center;
        margin-bottom: 1rem;
        font-size: 2rem;
        color: #333;
    }
    
    #contact {
        padding: 2rem 0;
        background-color: #f9f9f9;
    }
    
    #contact p {
        text-align: center;
        max-width: 600px;
        margin: 0 auto 2rem;
        color: #555;
        font-size: 1.1rem;
    }
    
    form {
        max-width: 600px;
        margin: 0 auto;
        background: #fff;
        padding: 2rem;
        border: 1px solid #ddd;
        border-radius: 8px;
    }
    
    label {
        display: block;
        margin-top: 1rem;
        font-weight: bold;
        color: #333;
    }
    
    input[type="text"],
    input[type="email"],
    textarea {
        width: 100%;
        padding: 0.8rem;
        margin-top: 0.5rem;
        border: 1px solid #ccc;
        border-radius: 4px;
        font-size: 1rem;
    }
    
    textarea {
        resize: vertical;
    }
    
    button[type="submit"] {
        display: inline-block;
        width: 100%;
        padding: 1rem;
        margin-top: 1.5rem;
        background-color: #333;
        color: #fff;
        font-size: 1.1rem;
        border: none;
        border-radius: 4px;
        cursor: pointer;
        transition: background-color 0.3s ease;
    }
    
    button[type="submit"]:hover {
        background-color: #555;
    }
    

![image](https://github.com/user-attachments/assets/35aa5532-2891-4ab2-8e8f-3d6ec6cc5230)

Form kontak dengan field untuk nama, email, dan pesan.
Tombol "Send Message" yang berfungsi untuk mengirim form.
