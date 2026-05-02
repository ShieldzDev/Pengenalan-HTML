Berikut materi **Pertemuan 5: Pengenalan CSS (Cascading Style Sheets)** dalam format Markdown dengan penjelasan naratif dan banyak contoh kode.

---

# Pertemuan 5: Pengenalan CSS (Cascading Style Sheets)

## Apa itu CSS

CSS (Cascading Style Sheets) digunakan untuk mengatur tampilan HTML, seperti warna, ukuran teks, jarak, dan layout.

Jika HTML berfungsi sebagai struktur, maka CSS berfungsi sebagai tampilan (design).

Contoh HTML tanpa CSS:

```html
<h1>Halo Dunia</h1>
<p>Ini adalah paragraf</p>
```

Dengan CSS:

```html
<h1 style="color: blue;">Halo Dunia</h1>
<p style="color: gray;">Ini adalah paragraf</p>
```

---

## Cara Menggunakan CSS

Ada 3 cara menggunakan CSS dalam HTML.

### Inline CSS

CSS langsung ditulis di dalam tag HTML menggunakan atribut `style`.

```html
<p style="color: red;">Teks berwarna merah</p>
```

Kelemahan: sulit dikelola jika banyak elemen.

---

### Internal CSS

CSS ditulis di dalam tag `<style>` di bagian `<head>`.

```html
<!DOCTYPE html>
<html>
  <head>
    <style>
      p {
        color: blue;
      }
    </style>
  </head>
  <body>
    <p>Ini paragraf berwarna biru</p>
  </body>
</html>
```

---

### External CSS

CSS ditulis di file terpisah.

**style.css**

```css
p {
  color: green;
}
```

**index.html**

```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <p>Ini paragraf berwarna hijau</p>
  </body>
</html>
```

Ini adalah cara yang paling direkomendasikan.

---

## Selector CSS

Selector digunakan untuk memilih elemen HTML yang akan diberi style.

### Selector Tag

```css
p {
  color: red;
}
```

Semua `<p>` akan berwarna merah.

---

### Selector Class

```html
<p class="teks">Hello</p>
```

```css
.teks {
  color: blue;
}
```

---

### Selector ID

```html
<p id="judul">Judul</p>
```

```css
#judul {
  color: green;
}
```

---

### Kombinasi Selector

```css
div p {
  color: purple;
}
```

Artinya: semua `<p>` di dalam `<div>`.

---

## Properti Dasar CSS

### Warna

```css
p {
  color: red;
}
```

```css
body {
  background-color: lightgray;
}
```

---

### Ukuran Teks

```css
h1 {
  font-size: 32px;
}
```

---

### Font

```css
p {
  font-family: Arial;
}
```

---

### Text Alignment

```css
h1 {
  text-align: center;
}
```

---

## Box Model (Dasar)

Setiap elemen HTML memiliki box yang terdiri dari:

* content
* padding
* border
* margin

Contoh:

```css
div {
  border: 1px solid black;
  padding: 10px;
  margin: 20px;
}
```

---

## Contoh Penggunaan CSS

```html
<!DOCTYPE html>
<html>
  <head>
    <style>
      body {
        background-color: #f0f0f0;
        font-family: Arial;
      }

      h1 {
        color: blue;
        text-align: center;
      }

      p {
        color: #333;
        font-size: 16px;
      }

      .box {
        border: 1px solid black;
        padding: 10px;
        margin: 20px;
        background-color: white;
      }
    </style>
  </head>
  <body>

    <h1>Belajar CSS</h1>

    <div class="box">
      <p>Ini adalah paragraf di dalam box.</p>
    </div>

  </body>
</html>
```

---

## Menghubungkan HTML dan CSS (Best Practice)

Struktur folder:

```
project/
│── index.html
│── style.css
```

**style.css**

```css
body {
  font-family: Arial;
  background-color: #fafafa;
}

h1 {
  color: darkblue;
}
```

**index.html**

```html
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>
    <h1>Hello CSS</h1>
  </body>
</html>
```

---

## Mini Project: Halaman Profil dengan CSS

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Profil</title>
    <style>
      body {
        font-family: Arial;
        background-color: #f4f4f4;
        text-align: center;
      }

      .card {
        background: white;
        padding: 20px;
        margin: 50px auto;
        width: 300px;
        border-radius: 10px;
      }

      img {
        width: 100px;
        border-radius: 50%;
      }

      h1 {
        color: #333;
      }

      p {
        color: #777;
      }
    </style>
  </head>
  <body>

    <div class="card">
      <img src="https://via.placeholder.com/100">
      <h1>Nama Kamu</h1>
      <p>Web Developer Pemula</p>
    </div>

  </body>
</html>
```

---

## Latihan

Buat halaman HTML dengan:

* Judul
* Paragraf
* Gambar
* 1 div sebagai card

Gunakan CSS untuk:

* Mengubah warna background
* Mengatur font
* Memberi padding dan margin
* Membuat tampilan lebih rapi

---
