# CSS DASAR

## 1.Membuat Dokumen HTML
```HTML
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
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
```
### Hasilnya
![Gambar 1](https://github.com/RizjkyDitoRidwansyah/Lab2Web/assets/116090827/d46ece9c-36e6-41a8-94fb-811c2a62b878)

## 2.Mendeklarasikan CSS Internal
```HTML
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
```
### Hasilnya
![Gambar 2](https://github.com/RizjkyDitoRidwansyah/Lab2Web/assets/116090827/5c5bf7f1-036b-424f-b915-30438f943578)


## 3.Menambahkan Inline CSS
```HTML
<p style="text-align: center; color: #ccd8e4;">
```
### Hasilnya
![Gambar 3](https://github.com/RizjkyDitoRidwansyah/Lab2Web/assets/116090827/a0ccb22b-e1f5-49c7-a721-1e785dfecd75)

## 4.Membuat CSS Eksternal

#### Membuat File CSS Terlebih Dahulu
![Gambar 4](https://github.com/RizjkyDitoRidwansyah/Lab2Web/assets/116090827/1802d16a-e96f-46ff-ba85-ca0c6a07c587)

#### Masukkan sourcecode
```CSS
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
#### Selanjutnya tambahkan tag `<link>` untuk merujuk file css yang sudah dibuat pada bagian `<head>`
```HTML
<head>
<!-- menyisipkan css eksternal -->
<link rel="stylesheet" href="style_eksternal.css" type="text/css">
</head>
```
### Hasilnya
![Gambar 4 1](https://github.com/RizjkyDitoRidwansyah/Lab2Web/assets/116090827/5e262730-2049-47e9-a838-113e0c92fe71)

### 5.Menambahkan CSS Selector
#### Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file style_eksternal.css,
```CSS
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
### Hasilnya
![Gambar 5](https://github.com/RizjkyDitoRidwansyah/Lab2Web/assets/116090827/28ab133c-30ae-4335-9312-57af2eb06d87)
