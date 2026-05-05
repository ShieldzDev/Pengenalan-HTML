Berikut materi **Pertemuan 6: Layout CSS (Flexbox & Dasar Responsive)** dalam format Markdown dengan penjelasan naratif dan banyak contoh kode.

---

# Pertemuan 6: Layout CSS (Flexbox & Dasar Responsive)

## Kenapa Perlu Layout di CSS

Pada pertemuan sebelumnya, kita sudah bisa memberi warna, font, dan jarak. Namun, tampilan masih belum fleksibel untuk mengatur posisi elemen secara rapi, terutama jika ingin membuat layout seperti:

* Navbar horizontal
* Card berjajar
* Halaman yang responsif

Untuk itu, kita menggunakan **Flexbox**, salah satu teknik layout modern di CSS.

---

## Pengenalan Flexbox

Flexbox digunakan untuk mengatur posisi elemen dalam satu baris atau kolom secara fleksibel.

Untuk mengaktifkan Flexbox, kita gunakan:

```css
.container {
  display: flex;
}
```

Contoh:

```html id="f1a2b3"
<div class="container">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
</div>
```

```css id="f4d5e6"
.container {
  display: flex;
}
```

Secara default, item akan berjajar horizontal.

---

## Arah Flex (flex-direction)

Mengatur arah susunan item:

```css
.container {
  display: flex;
  flex-direction: row;
}
```

Pilihan:

* `row` (default) → horizontal
* `column` → vertikal

Contoh:

```css
.container {
  display: flex;
  flex-direction: column;
}
```

---

## Mengatur Jarak (justify-content)

Digunakan untuk mengatur posisi horizontal:

```css
.container {
  display: flex;
  justify-content: center;
}
```

Pilihan:

* `flex-start`
* `center`
* `flex-end`
* `space-between`
* `space-around`

Contoh:

```css
.container {
  display: flex;
  justify-content: space-between;
}
```

---

## Mengatur Posisi Vertikal (align-items)

```css
.container {
  display: flex;
  align-items: center;
}
```

Contoh lengkap:

```css
.container {
  display: flex;
  height: 200px;
  justify-content: center;
  align-items: center;
}
```

---

## Contoh Flexbox Sederhana

```html id="abc123"
<div class="container">
  <div class="box">1</div>
  <div class="box">2</div>
  <div class="box">3</div>
</div>
```

```css id="def456"
.container {
  display: flex;
  justify-content: space-around;
}

.box {
  width: 50px;
  height: 50px;
  background-color: blue;
  color: white;
  text-align: center;
}
```

---

## Membuat Navbar dengan Flexbox

```html id="nav123"
<div class="navbar">
  <h2>Logo</h2>
  <div class="menu">
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Contact</a>
  </div>
</div>
```

```css id="nav456"
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #333;
  color: white;
  padding: 10px;
}

.menu a {
  color: white;
  margin-left: 10px;
  text-decoration: none;
}
```

---

## Membuat Card Layout

```html id="card123"
<div class="container">
  <div class="card">Card 1</div>
  <div class="card">Card 2</div>
  <div class="card">Card 3</div>
</div>
```

```css id="card456"
.container {
  display: flex;
  gap: 10px;
}

.card {
  padding: 20px;
  background: lightgray;
  flex: 1;
}
```

---

## Dasar Responsive Design

Responsive berarti tampilan menyesuaikan ukuran layar.

### Menggunakan Flex Wrap

```css
.container {
  display: flex;
  flex-wrap: wrap;
}
```

Agar item turun ke bawah jika layar kecil.

---

### Menggunakan Media Query

Media query digunakan untuk mengatur tampilan berdasarkan ukuran layar.

```css
@media (max-width: 600px) {
  body {
    background-color: lightblue;
  }
}
```

Contoh:

```css
.container {
  display: flex;
}

@media (max-width: 600px) {
  .container {
    flex-direction: column;
  }
}
```

---

## Contoh Halaman Responsive Sederhana

```html id="resp123"
<!DOCTYPE html>
<html>
  <head>
    <title>Responsive</title>
    <style>
      body {
        font-family: Arial;
      }

      .container {
        display: flex;
        gap: 10px;
      }

      .card {
        flex: 1;
        padding: 20px;
        background: lightgray;
      }

      @media (max-width: 600px) {
        .container {
          flex-direction: column;
        }
      }
    </style>
  </head>
  <body>

    <h1>Responsive Layout</h1>

    <div class="container">
      <div class="card">Card 1</div>
      <div class="card">Card 2</div>
      <div class="card">Card 3</div>
    </div>

  </body>
</html>
```

---

## Latihan

Buat halaman dengan:

* Navbar (menggunakan flexbox)
* 3 card sejajar
* Saat layar kecil, card menjadi vertikal

Gunakan:

* `display: flex`
* `justify-content`
* `align-items`
* `@media`

---

## Ringkasan

Pada pertemuan ini, kamu telah mempelajari:

* Cara menggunakan Flexbox untuk layout
* Mengatur posisi horizontal dan vertikal
* Membuat navbar dan card layout
* Dasar responsive design dengan media query

Dengan ini, kamu sudah bisa membuat tampilan website yang lebih modern dan fleksibel.
