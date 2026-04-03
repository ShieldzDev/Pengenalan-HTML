Berikut materi **Pertemuan 4: Form HTML & Mini Project** dalam format Markdown dengan penjelasan naratif dan banyak contoh kode.

---

# Pertemuan 4: Form HTML & Mini Project

## Pengenalan Form

Form digunakan untuk mengambil input dari pengguna, seperti nama, email, password, dan lain-lain. Data dari form biasanya akan dikirim ke server untuk diproses.

Struktur dasar form:

```html
<form>
  <input type="text">
  <button type="submit">Kirim</button>
</form>
```

Namun, form yang baik membutuhkan label, struktur, dan tipe input yang sesuai.

---

## Elemen Input

Tag `<input>` memiliki banyak tipe yang bisa digunakan tergantung kebutuhan.

### Input Text

```html
<form>
  <input type="text" placeholder="Masukkan nama">
</form>
```

### Input Email

```html
<form>
  <input type="email" placeholder="Masukkan email">
</form>
```

### Input Password

```html
<form>
  <input type="password" placeholder="Masukkan password">
</form>
```

### Input Number

```html
<form>
  <input type="number" placeholder="Masukkan umur">
</form>
```

---

## Label pada Form

Label digunakan untuk memberi keterangan pada input.

```html
<form>
  <label>Nama:</label>
  <input type="text">
</form>
```

Cara yang lebih baik adalah menghubungkan label dengan input menggunakan `for` dan `id`:

```html
<form>
  <label for="nama">Nama:</label>
  <input type="text" id="nama">
</form>
```

---

## Input Pilihan

### Checkbox

Digunakan untuk memilih lebih dari satu opsi.

```html
<form>
  <label>
    <input type="checkbox"> HTML
  </label>
  <label>
    <input type="checkbox"> CSS
  </label>
</form>
```

### Radio Button

Digunakan untuk memilih satu opsi saja.

```html
<form>
  <label>
    <input type="radio" name="gender"> Laki-laki
  </label>
  <label>
    <input type="radio" name="gender"> Perempuan
  </label>
</form>
```

Perhatikan bahwa `name` harus sama agar hanya satu yang bisa dipilih.

---

## Textarea

Digunakan untuk input teks panjang.

```html
<form>
  <textarea placeholder="Masukkan pesan"></textarea>
</form>
```

---

## Select (Dropdown)

```html
<form>
  <label>Pilih Kota:</label>
  <select>
    <option>Jakarta</option>
    <option>Bandung</option>
    <option>Surabaya</option>
  </select>
</form>
```

---

## Button

```html
<form>
  <button type="submit">Kirim</button>
  <button type="reset">Reset</button>
</form>
```

---

## Contoh Form Lengkap

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Form Pendaftaran</title>
  </head>
  <body>

    <h1>Form Pendaftaran</h1>

    <form>
      <label for="nama">Nama:</label><br>
      <input type="text" id="nama" placeholder="Masukkan nama"><br><br>

      <label for="email">Email:</label><br>
      <input type="email" id="email" placeholder="Masukkan email"><br><br>

      <label>Password:</label><br>
      <input type="password"><br><br>

      <label>Jenis Kelamin:</label><br>
      <input type="radio" name="gender"> Laki-laki
      <input type="radio" name="gender"> Perempuan<br><br>

      <label>Hobi:</label><br>
      <input type="checkbox"> Membaca
      <input type="checkbox"> Coding
      <input type="checkbox"> Gaming<br><br>

      <label>Kota:</label><br>
      <select>
        <option>Jakarta</option>
        <option>Bandung</option>
      </select><br><br>

      <label>Pesan:</label><br>
      <textarea></textarea><br><br>

      <button type="submit">Kirim</button>
      <button type="reset">Reset</button>
    </form>

  </body>
</html>
```

---

## Atribut Penting pada Form

### action dan method

```html
<form action="/submit" method="POST">
```

* `action` menentukan ke mana data dikirim
* `method` menentukan cara pengiriman (GET atau POST)

### required

```html
<input type="text" required>
```

Field wajib diisi.

### value

```html
<input type="text" value="Default">
```

---

## Mini Project: Halaman Profil dengan Form

Buat halaman HTML sederhana yang berisi:

* Judul profil
* Deskripsi singkat
* Gambar
* Form kontak

Contoh:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Profil Saya</title>
  </head>
  <body>

    <h1>Profil Saya</h1>

    <img src="https://via.placeholder.com/150" alt="Foto Profil">

    <p>Halo, saya sedang belajar HTML.</p>

    <h2>Hubungi Saya</h2>

    <form>
      <input type="text" placeholder="Nama"><br><br>
      <input type="email" placeholder="Email"><br><br>
      <textarea placeholder="Pesan"></textarea><br><br>
      <button type="submit">Kirim</button>
    </form>

  </body>
</html>
```

---

## Latihan

Buat form dengan ketentuan:

* Input:

  * Nama
  * Email
  * Password
* Pilihan:

  * Radio (jenis kelamin)
  * Checkbox (minimal 2 hobi)
* Dropdown kota
* Textarea pesan
* Tombol submit dan reset

Tambahkan juga:

* Judul halaman
* Gambar
* Paragraf deskripsi

---

## Ringkasan

Pada pertemuan ini, kamu telah mempelajari:

* Cara membuat form di HTML
* Berbagai tipe input
* Cara menggunakan label
* Cara membuat dropdown, checkbox, dan radio button
* Membuat halaman HTML lengkap dengan form

Dengan ini, kamu sudah mampu membuat halaman web statis yang interaktif dan siap dikembangkan ke tahap berikutnya seperti CSS dan JavaScript.
