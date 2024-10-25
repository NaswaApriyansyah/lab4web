![image](https://github.com/user-attachments/assets/d5e0dac4-3271-49b9-b3bc-5cb1b6b06636)# lab4web
# 1Langkah-langkah Praktikum
Persiapan membuat dokumen HTML dengan nama file lab4_box.html seperti berikut.
```<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Box Element</title>
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
</head>
<body>
<header>
<h1>Box Element</h1>
<section>
    <div class="div1">Div 1</div>
    <div class="div2">Div 2</div>
    <div class="div3">Div 3</div>
    </section>
</header>
</body>
</html>
```
Kemudian buka browser untuk melihat hasilnya.
![Screenshot (3)](https://github.com/user-attachments/assets/35ca4b45-d557-4802-884f-e70859af3534)

# 2.Mengatur Clearfix Element
Clearfix digunakan untuk mengatur element setelah float element. Property clear digunakan untuk
mengaturnya.
```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Box Element</title>
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
    .div4 {
        background-color: blue;
        clear: left;
        float: none;
        }
    </style>
</head>
<body>
<header>
<h1>Box Element</h1>
<section>
    <div class="div1">Div 1</div>
    <div class="div2">Div 2</div>
    <div class="div3">Div 3</div>
    <div class="div4">div 4</div>
    </section>
</header>
</body>
</html>
```
hasil browsernya
![Screenshot (4)](https://github.com/user-attachments/assets/70ac3c83-91c5-4295-a519-7f47c3256fda)

# 3. Membuat Layout Sederhana
```<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Layout Sederhana</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
<div id="container">
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
</div>
</body>
</html>
```
hasil browser sebagai berikut
![Cuplikan layar 2024-10-25 075718](https://github.com/user-attachments/assets/92dffcd5-9c5c-4be3-9232-720e53272f9d)

kemudian tambahkan kode berikut!
```/* import google font */
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
@importurl('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap');
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
```
hasil browser sebagai berikut!
![Screenshot (5)](https://github.com/user-attachments/assets/22995be0-a9dc-4adf-a77b-9ff432b5387f)
# Membuat Navigasi
```/* navigasi */
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
```
hasil browser sebagai berikut!
![Screenshot (6)](https://github.com/user-attachments/assets/7153f863-3d9b-4cb1-b62b-f2e78fcd4512)

# Membuat Hero Panel.
tambahkan html
```<section id="hero">
<h1>Hello World!</h1>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
pretium ac.</p>
<a href="home.html" class="btn btn-large">Learn more &raquo;</a>
</section>
```
tambahkan css
```/* Hero Panel */
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
```
hasil brower sebagai berikut!
![Screenshot (7)](https://github.com/user-attachments/assets/ce2160fc-eb61-432c-ae94-4c9a85c3a08b)
# Mengatur Layout Main dan Sidebar
tambahkan css
```/* main content */
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
```
# Membuat Sidebar Widget
Kemudian selanjutnya menambahkan element lain dalam sidebar.
```<aside id="sidebar">
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
</aside
```
Kemudian tambahkan CSS.
```/* widget */
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
}
.widget-box li a {
padding:10px 16px;
color:#333;
display:block;
text-decoration:none;
}
.widget-box li:hover a {
background-color:#eee;
}
.widget-box p {
padding:15px;
line-height:25px;
}
```
hasil browser sebagai berikut!

![Cuplikan layar 2024-10-25 082037](https://github.com/user-attachments/assets/84e431a7-c3f9-4585-a9f1-ac7aacb2cbca)

# Mengatur Footer
Selanjutnya mengatur tampilan footer. Tambahkan CSS untuk footer.
```/* footer */
footer {
clear:both;
background-color:#1d1d1d;
padding:20px;
color:#eee;
}
```

hasil browsernya sebagai berikut!

![Cuplikan layar 2024-10-25 082920](https://github.com/user-attachments/assets/695d888a-8bc8-4231-b857-c6716b65c0bc)
# Menambahkan Elemen lainnya pada Main Content
```<section id="main">
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
```
# Kemudian tambahkan CSS.
```/* box */
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
```

Lihat hasilnya dibrowser.

![Cuplikan layar 2024-10-25 082957](https://github.com/user-attachments/assets/e8334a2d-f033-4c31-8eac-82eb7d72b1b2)

# Menambahkan Content Artikel
Selanjutnya membuat content artikel. Tambahkan HTML berikut pada main content.
```<hr class="divider" />
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
```
Kemudian tambahkan CSS.
```.divider {
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
```
 hasil gambar sebagai berikut!
 
![Cuplikan layar 2024-10-25 083032](https://github.com/user-attachments/assets/8854493f-9e07-4b6b-a52b-10f779b23786)
