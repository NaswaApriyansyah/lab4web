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
