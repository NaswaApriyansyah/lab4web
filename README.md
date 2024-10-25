# lab4web
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

