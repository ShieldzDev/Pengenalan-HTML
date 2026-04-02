Berikut materi **Pertemuan 1: Pengenalan HTML & Struktur Dasar** dalam format Markdown, dengan penjelasan lebih naratif dan banyak contoh kode.

---

# Pertemuan 1: Pengenalan HTML & Struktur Dasar

## Apa itu HTML

HTML (HyperText Markup Language) adalah bahasa dasar untuk membuat halaman web. HTML tidak bersifat seperti bahasa pemrograman (tidak ada logika seperti if/loop), tetapi digunakan untuk menyusun struktur dan konten sebuah halaman.

Browser seperti Chrome atau Firefox akan membaca file HTML dan menampilkannya menjadi halaman yang bisa dilihat oleh pengguna.

Sebagai contoh sederhana, berikut adalah isi file HTML paling dasar:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Halaman Pertama</title>
  </head>
  <body>
    <h1>Hello World</h1>
    <p>Ini adalah halaman HTML pertama saya</p>
  </body>
</html>
```

Jika file ini disimpan dengan nama `index.html` dan dibuka di browser, maka akan muncul teks “Hello World” dan sebuah paragraf.

---

## Cara Kerja HTML di Browser

Ketika kita membuka file HTML:

1. Browser membaca file dari atas ke bawah
2. Setiap tag HTML diterjemahkan menjadi tampilan visual
3. Struktur HTML menentukan bagaimana konten ditampilkan

Contoh:

```html
<h1>Judul Besar</h1>
<p>Paragraf pertama</p>
<p>Paragraf kedua</p>
```

Browser akan menampilkan:

* Judul besar (teks besar dan tebal)
* Dua paragraf di bawahnya

---

## Struktur Dasar HTML

Setiap dokumen HTML memiliki struktur standar seperti berikut:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Judul Halaman</title>
  </head>
  <body>
    Konten ditulis di sini
  </body>
</html>
```

Penjelasan:

* `<!DOCTYPE html>` memberitahu browser bahwa ini adalah HTML5
* `<html>` adalah root dari seluruh dokumen
* `<head>` berisi informasi tentang halaman (tidak terlihat langsung)
* `<body>` berisi konten yang akan ditampilkan ke pengguna

Contoh lain dengan konten lebih jelas:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Website Saya</title>
  </head>
  <body>
    <h1>Selamat Datang</h1>
    <p>Ini adalah website pertama saya.</p>
  </body>
</html>
```

---

## Tag, Element, dan Atribut

HTML terdiri dari tag, element, dan atribut.

### Tag

Tag adalah penanda yang ditulis dengan tanda `< >`.

```html
<p>Ini paragraf</p>
```

Tag pembuka: `<p>`
Tag penutup: `</p>`

### Element

Element adalah keseluruhan dari tag pembuka, isi, dan tag penutup.

```html
<p>Ini paragraf</p>
```

### Atribut

Atribut memberikan informasi tambahan pada tag.

```html
<p class="text">Ini paragraf dengan atribut</p>
```

Contoh lain:

```html
<a href="https://google.com">Buka Google</a>
```

`href` adalah atribut yang menentukan tujuan link.

---

## Heading (Judul)

HTML menyediakan 6 level heading, dari yang terbesar (`h1`) sampai terkecil (`h6`).

```html
<h1>Judul 1</h1>
<h2>Judul 2</h2>
<h3>Judul 3</h3>
<h4>Judul 4</h4>
<h5>Judul 5</h5>
<h6>Judul 6</h6>
```

Contoh penggunaan:

```html
<h1>Blog Saya</h1>
<h2>Artikel Terbaru</h2>
<h3>Cara Belajar HTML</h3>
```

---

## Paragraf

Paragraf digunakan untuk menampilkan teks dalam bentuk blok.

```html
<p>Ini adalah paragraf pertama.</p>
<p>Ini adalah paragraf kedua.</p>
```

Jika kita menulis teks tanpa tag `<p>`, browser tetap akan menampilkan, tetapi tidak terstruktur dengan baik.

---

## Line Break dan Horizontal Line

Untuk membuat baris baru:

```html
<p>Baris pertama<br>Baris kedua</p>
```

Untuk membuat garis horizontal:

```html
<hr>
```

Contoh:

```html
<h1>Judul</h1>
<hr>
<p>Ini adalah isi konten</p>
```

---

## Contoh Halaman Lengkap Sederhana

Berikut contoh halaman HTML sederhana yang menggabungkan semua materi:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Profil Saya</title>
  </head>
  <body>
    <h1>Halo, Saya Budi</h1>
    <h2>Tentang Saya</h2>
    <p>Saya sedang belajar HTML.</p>

    <hr>

    <h2>Hobi</h2>
    <p>Saya suka membaca dan coding.</p>
  </body>
</html>
```

---

## Latihan

Buat file HTML dengan ketentuan:

* Memiliki minimal:

  * 1 heading utama
  * 2 subheading
  * 3 paragraf
* Gunakan `<hr>` untuk memisahkan bagian
* Gunakan `<br>` di salah satu paragraf

Contoh struktur yang diharapkan:

```html
<h1>Nama Kamu</h1>
<h2>Tentang Saya</h2>
<p>...</p>

<hr>

<h2>Pengalaman</h2>
<p>...</p>
```

---

## Ringkasan

Pada pertemuan ini, kamu sudah belajar:

* Apa itu HTML dan fungsinya
* Struktur dasar HTML
* Cara kerja browser membaca HTML
* Penggunaan tag dasar seperti heading dan paragraf
* Konsep tag, element, dan atribut

Langkah selanjutnya adalah memperkaya tampilan dengan elemen lain seperti list, link, dan gambar.
