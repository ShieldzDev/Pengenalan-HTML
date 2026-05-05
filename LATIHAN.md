Berikut contoh **halaman portfolio sederhana** sebagai latihan yang menggabungkan HTML + CSS + Flexbox + sedikit responsive. Struktur dibuat cukup realistis tapi tetap mudah dipahami.

---

# Latihan: Halaman Portfolio Sederhana

## Struktur Folder

```
portfolio/
│── index.html
│── style.css
```

---

## File: index.html

```html id="pf1html"
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Portfolio Saya</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <!-- Navbar -->
  <header class="navbar">
    <h2>MyPortfolio</h2>
    <nav>
      <a href="#about">Tentang</a>
      <a href="#project">Project</a>
      <a href="#contact">Kontak</a>
    </nav>
  </header>

  <!-- Hero -->
  <section class="hero">
    <img src="https://via.placeholder.com/120" alt="Foto Profil">
    <h1>Nama Kamu</h1>
    <p>Web Developer Pemula</p>
  </section>

  <!-- Tentang -->
  <section id="about" class="about">
    <h2>Tentang Saya</h2>
    <p>
      Saya sedang belajar HTML, CSS, dan JavaScript.
      Saya tertarik menjadi seorang web developer.
    </p>
  </section>

  <!-- Project -->
  <section id="project" class="project">
    <h2>Project Saya</h2>

    <div class="project-container">
      <div class="card">
        <h3>Project 1</h3>
        <p>Website sederhana menggunakan HTML</p>
      </div>

      <div class="card">
        <h3>Project 2</h3>
        <p>Form pendaftaran sederhana</p>
      </div>

      <div class="card">
        <h3>Project 3</h3>
        <p>Landing page sederhana</p>
      </div>
    </div>
  </section>

  <!-- Kontak -->
  <section id="contact" class="contact">
    <h2>Kontak</h2>

    <form>
      <input type="text" placeholder="Nama">
      <input type="email" placeholder="Email">
      <textarea placeholder="Pesan"></textarea>
      <button type="submit">Kirim</button>
    </form>
  </section>

  <!-- Footer -->
  <footer>
    <p>© 2026 Portfolio Saya</p>
  </footer>

</body>
</html>
```

---

## File: style.css

```css id="pf1css"
body {
  font-family: Arial;
  margin: 0;
  background-color: #f4f4f4;
}

/* Navbar */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #333;
  color: white;
  padding: 10px 20px;
}

.navbar a {
  color: white;
  margin-left: 15px;
  text-decoration: none;
}

/* Hero */
.hero {
  text-align: center;
  padding: 40px;
  background: white;
}

.hero img {
  border-radius: 50%;
}

/* Section umum */
section {
  padding: 30px;
  margin: 20px;
  background: white;
  border-radius: 8px;
}

/* Project */
.project-container {
  display: flex;
  gap: 10px;
}

.card {
  flex: 1;
  background: #eee;
  padding: 20px;
  border-radius: 8px;
}

/* Form */
form {
  display: flex;
  flex-direction: column;
}

input, textarea {
  margin-bottom: 10px;
  padding: 10px;
}

button {
  padding: 10px;
  background: #333;
  color: white;
  border: none;
}

/* Footer */
footer {
  text-align: center;
  padding: 15px;
  background: #333;
  color: white;
}

/* Responsive */
@media (max-width: 600px) {
  .project-container {
    flex-direction: column;
  }
}
```

---

## Penjelasan Singkat

Halaman ini terdiri dari beberapa bagian utama:

* Navbar → navigasi antar section
* Hero → identitas utama (nama & foto)
* About → deskripsi diri
* Project → menampilkan karya
* Contact → form sederhana
* Footer → informasi penutup

Flexbox digunakan pada:

```css
.project-container {
  display: flex;
}
```

Responsive dilakukan dengan:

```css
@media (max-width: 600px) {
  .project-container {
    flex-direction: column;
  }
}
```

---

## Tantangan Pengembangan

Coba modifikasi sendiri:

1. Tambahkan gambar di setiap project
2. Tambahkan hover effect pada card:

   ```css
   .card:hover {
     background: #ddd;
   }
   ```
3. Tambahkan link ke project (pakai `<a>`)
4. Ubah warna tema sesuai selera
5. Tambahkan social media (GitHub / Instagram)

---

## Hasil yang Diharapkan

Setelah latihan ini, kamu sudah bisa:

* Membuat halaman portfolio sederhana
* Menggunakan Flexbox untuk layout
* Menggunakan form dalam website
* Membuat tampilan responsive dasar

---

Kalau kamu mau, aku bisa lanjutkan ke:

* versi **portfolio yang lebih profesional (dengan animasi + Tailwind)**
* atau **langsung ke JavaScript (biar websitenya interaktif)**
