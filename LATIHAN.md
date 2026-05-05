Berikut contoh **halaman portfolio sederhana** yang bisa kamu gunakan sebagai latihan. Contoh ini menggabungkan HTML + CSS + Flexbox + sedikit responsive, serta menggunakan gambar agar tampil lebih menarik.

---

# Latihan: Halaman Portfolio Sederhana

## Struktur File

```text
portfolio/
│── index.html
│── style.css
```

---

## File: `index.html`

```html
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
      <a href="#">Home</a>
      <a href="#">About</a>
      <a href="#">Project</a>
      <a href="#">Contact</a>
    </nav>
  </header>

  <!-- Hero Section -->
  <section class="hero">
    <img src="https://via.placeholder.com/150" alt="Foto Profil">
    <h1>Nama Kamu</h1>
    <p>Web Developer Pemula</p>
  </section>

  <!-- About -->
  <section class="about">
    <h2>Tentang Saya</h2>
    <p>
      Saya sedang belajar HTML, CSS, dan JavaScript untuk menjadi web developer.
      Saya tertarik membuat website yang menarik dan responsif.
    </p>
  </section>

  <!-- Project -->
  <section class="projects">
    <h2>Project Saya</h2>
    <div class="project-container">
      
      <div class="card">
        <img src="https://via.placeholder.com/300x150">
        <h3>Project 1</h3>
        <p>Website sederhana menggunakan HTML.</p>
      </div>

      <div class="card">
        <img src="https://via.placeholder.com/300x150">
        <h3>Project 2</h3>
        <p>Landing page dengan CSS.</p>
      </div>

      <div class="card">
        <img src="https://via.placeholder.com/300x150">
        <h3>Project 3</h3>
        <p>Portfolio pertama saya.</p>
      </div>

    </div>
  </section>

  <!-- Contact -->
  <section class="contact">
    <h2>Contact</h2>
    <form>
      <input type="text" placeholder="Nama"><br>
      <input type="email" placeholder="Email"><br>
      <textarea placeholder="Pesan"></textarea><br>
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

## File: `style.css`

```css
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background-color: #f4f4f4;
}

/* Navbar */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #333;
  color: white;
  padding: 15px;
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
  background-color: #fff;
}

.hero img {
  border-radius: 50%;
  width: 120px;
}

/* Section */
section {
  padding: 30px;
  text-align: center;
}

/* Projects */
.project-container {
  display: flex;
  gap: 15px;
  justify-content: center;
}

.card {
  background: white;
  padding: 15px;
  width: 250px;
  border-radius: 10px;
}

.card img {
  width: 100%;
  border-radius: 5px;
}

/* Contact */
.contact input,
.contact textarea {
  width: 60%;
  padding: 10px;
  margin: 5px;
}

.contact button {
  padding: 10px 20px;
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
    align-items: center;
  }

  .contact input,
  .contact textarea {
    width: 90%;
  }
}
```

---

## Tujuan Latihan

Dengan membuat halaman ini, kamu akan melatih:

* Menggabungkan HTML dan CSS dalam satu project
* Menggunakan Flexbox untuk layout
* Membuat card layout
* Menggunakan gambar dalam website
* Membuat tampilan responsive sederhana
* Membuat struktur website lengkap (navbar, section, footer)

---

## Tantangan Tambahan

Jika ingin meningkatkan skill, coba:

* Ganti gambar placeholder dengan gambar asli
* Tambahkan hover effect pada card
* Tambahkan icon (misalnya sosial media)
* Ubah warna agar lebih personal
* Tambahkan animasi sederhana dengan CSS

---

Kalau kamu mau, aku bisa bantu:

* upgrade jadi **portfolio yang lebih profesional (pakai Tailwind / animasi)**
* atau jadikan ini **template siap pakai untuk skripsi / CV online**
