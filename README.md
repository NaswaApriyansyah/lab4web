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
