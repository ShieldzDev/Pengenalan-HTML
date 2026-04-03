Berikut materi **Pertemuan 2: Formatting & Elemen Dasar HTML** dalam format Markdown, dengan penjelasan naratif dan banyak contoh kode.

---

# Pertemuan 2: Formatting & Elemen Dasar HTML

## Formatting Teks

HTML menyediakan beberapa tag untuk memformat teks agar memiliki makna atau tampilan tertentu.

Perhatikan contoh berikut:

```html
<p>Ini adalah teks <b>tebal</b></p>
<p>Ini adalah teks <strong>penting</strong></p>
<p>Ini adalah teks <i>miring</i></p>
<p>Ini adalah teks <em>penekanan</em></p>
<p>Ini adalah teks <u>garis bawah</u></p>
```

Penjelasan:

* `<b>` hanya membuat teks menjadi tebal
* `<strong>` menunjukkan bahwa teks tersebut penting (secara semantik)
* `<i>` membuat teks miring
* `<em>` memberi penekanan (biasanya juga tampil miring)
* `<u>` memberi garis bawah

Contoh penggunaan dalam satu paragraf:

```html
<p>
  Saya sedang belajar <strong>HTML</strong> dan ini sangat <em>menarik</em>.
  Saya ingin menjadi <b>web developer</b>.
</p>
```

---

## List (Daftar)

HTML menyediakan dua jenis list utama: ordered list dan unordered list.

### Unordered List (Bullet)

```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>
```

Hasilnya akan berupa daftar dengan tanda bullet.

### Ordered List (Nomor)

```html
<ol>
  <li>Bangun pagi</li>
  <li>Belajar HTML</li>
  <li>Istirahat</li>
</ol>
```

Hasilnya berupa daftar bernomor.

### Kombinasi List

List bisa digabung:

```html
<ul>
  <li>Frontend
    <ol>
      <li>HTML</li>
      <li>CSS</li>
    </ol>
  </li>
  <li>Backend</li>
</ul>
```

---

## Link (Hyperlink)

Link digunakan untuk berpindah ke halaman lain.

Struktur dasar:

```html
<a href="https://google.com">Buka Google</a>
```

Atribut `href` menentukan tujuan link.

Contoh lain:

```html
<a href="https://github.com">Kunjungi GitHub</a>
```

### Membuka Link di Tab Baru

```html
<a href="https://google.com" target="_blank">Buka di tab baru</a>
```

### Link ke Halaman Lokal

Jika punya file lain:

```html
<a href="about.html">Halaman Tentang</a>
```

---

## Gambar (Image)

Untuk menampilkan gambar digunakan tag `<img>`.

```html
<img src="gambar.jpg" alt="Deskripsi gambar">
```

Penjelasan:

* `src` adalah lokasi gambar
* `alt` adalah deskripsi jika gambar tidak tampil

Contoh:

```html
<img src="https://via.placeholder.com/150" alt="Contoh gambar">
```

### Mengatur Ukuran Gambar

```html
<img src="https://via.placeholder.com/150" width="100" height="100">
```

---

## Menggabungkan Link dan Gambar

Gambar bisa dijadikan link:

```html
<a href="https://google.com">
  <img src="https://via.placeholder.com/100" alt="Klik gambar">
</a>
```

---

## Contoh Halaman Lengkap

Berikut contoh halaman yang menggunakan formatting, list, link, dan gambar:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Belajar HTML</title>
  </head>
  <body>
    <h1>Belajar HTML Dasar</h1>

    <p>
      Saya sedang belajar <strong>HTML</strong>. Ini adalah langkah awal
      menjadi <em>web developer</em>.
    </p>

    <h2>Materi yang Dipelajari</h2>
    <ul>
      <li>HTML Dasar</li>
      <li>Formatting</li>
      <li>Link</li>
    </ul>

    <h2>Langkah Belajar</h2>
    <ol>
      <li>Pahami teori</li>
      <li>Praktik coding</li>
      <li>Buat project</li>
    </ol>

    <h2>Contoh Gambar</h2>
    <img src="https://via.placeholder.com/150" alt="Gambar contoh">

    <h2>Referensi</h2>
    <p>
      Kunjungi 
      <a href="https://developer.mozilla.org" target="_blank">
        MDN Web Docs
      </a>
      untuk belajar lebih lanjut.
    </p>
  </body>
</html>
```

---

## Latihan

Buat halaman HTML dengan ketentuan:

* Gunakan minimal:

  * 2 jenis formatting teks
  * 1 unordered list
  * 1 ordered list
  * 1 link
  * 1 gambar
* Buat halaman bertema:

  * “Hobi Saya” atau “Belajar Web Development”

Contoh struktur:

```html
<h1>Hobi Saya</h1>

<p>Saya suka <b>bermain game</b> dan <i>membaca</i>.</p>

<h2>Daftar Hobi</h2>
<ul>
  <li>Game</li>
  <li>Membaca</li>
</ul>

<h2>Website Favorit</h2>
<a href="https://google.com">Google</a>
```

---
