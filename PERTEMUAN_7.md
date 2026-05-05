Berikut materi **Pertemuan 7: Pengenalan JavaScript (Dasar Interaksi Web)** dalam format Markdown dengan penjelasan naratif dan banyak contoh kode.

---

# Pertemuan 7: Pengenalan JavaScript (Dasar Interaksi Web)

## Apa itu JavaScript

Jika HTML digunakan untuk struktur dan CSS untuk tampilan, maka JavaScript digunakan untuk membuat halaman web menjadi interaktif.

Dengan JavaScript, kita bisa:

* Menangani klik tombol
* Mengubah isi halaman tanpa reload
* Mengolah input dari pengguna
* Membuat logika sederhana

Contoh sederhana:

```html
<button onclick="alert('Hello World')">Klik Saya</button>
```

Saat tombol diklik, akan muncul popup.

---

## Cara Menggunakan JavaScript

### Inline JavaScript

```html
<button onclick="alert('Halo')">Klik</button>
```

---

### Internal JavaScript

```html
<!DOCTYPE html>
<html>
<head>
  <script>
    function sapa() {
      alert("Halo dari JavaScript");
    }
  </script>
</head>
<body>

<button onclick="sapa()">Klik</button>

</body>
</html>
```

---

### External JavaScript

**script.js**

```javascript
function sapa() {
  alert("Halo dari file JS");
}
```

**index.html**

```html
<script src="script.js"></script>
<button onclick="sapa()">Klik</button>
```

---

## Variabel

Variabel digunakan untuk menyimpan data.

```javascript
let nama = "Budi";
let umur = 20;

console.log(nama);
console.log(umur);
```

---

## Tipe Data

```javascript
let teks = "Hello";      // string
let angka = 10;          // number
let benar = true;        // boolean
```

---

## Operator

```javascript
let a = 10;
let b = 5;

console.log(a + b); // 15
console.log(a - b); // 5
console.log(a * b); // 50
```

---

## Fungsi

Fungsi digunakan untuk mengelompokkan kode.

```javascript
function salam() {
  console.log("Halo!");
}

salam();
```

Dengan parameter:

```javascript
function sapa(nama) {
  console.log("Halo " + nama);
}

sapa("Budi");
```

---

## DOM (Document Object Model)

DOM adalah cara JavaScript berinteraksi dengan HTML.

### Mengambil Elemen

```html
<p id="teks">Hello</p>
```

```javascript
let elemen = document.getElementById("teks");
console.log(elemen);
```

---

### Mengubah Isi

```javascript
document.getElementById("teks").innerHTML = "Teks baru";
```

---

### Mengubah Style

```javascript
document.getElementById("teks").style.color = "red";
```

---

## Event (Interaksi)

### Klik Tombol

```html
<button onclick="ubahTeks()">Klik</button>
<p id="hasil">Hello</p>
```

```javascript
function ubahTeks() {
  document.getElementById("hasil").innerHTML = "Berubah!";
}
```

---

## Contoh Interaktif Sederhana

```html
<!DOCTYPE html>
<html>
<head>
  <title>JavaScript Dasar</title>
</head>
<body>

  <h1 id="judul">Hello</h1>
  <button onclick="ganti()">Ganti Teks</button>

  <script>
    function ganti() {
      document.getElementById("judul").innerHTML = "Hello JavaScript";
    }
  </script>

</body>
</html>
```

---

## Mengambil Input User

```html
<input type="text" id="nama">
<button onclick="tampil()">Kirim</button>

<p id="output"></p>
```

```javascript
function tampil() {
  let nama = document.getElementById("nama").value;
  document.getElementById("output").innerHTML = "Halo " + nama;
}
```

---

## Contoh Mini Project

Form sederhana:

```html
<!DOCTYPE html>
<html>
<body>

<h2>Form Sederhana</h2>

<input type="text" id="nama" placeholder="Nama">
<button onclick="proses()">Submit</button>

<p id="hasil"></p>

<script>
function proses() {
  let nama = document.getElementById("nama").value;
  document.getElementById("hasil").innerHTML = "Halo, " + nama;
}
</script>

</body>
</html>
```

---

## Latihan

Buat halaman dengan:

* Input nama
* Tombol
* Output teks

Ketika tombol diklik:

* Tampilkan "Halo [nama]"

Tambahan:

* Ubah warna teks hasil
* Tambahkan validasi jika input kosong

---

## Ringkasan

Pada pertemuan ini, kamu telah mempelajari:

* Apa itu JavaScript dan fungsinya
* Cara menambahkan JavaScript ke HTML
* Variabel dan fungsi
* DOM untuk mengakses HTML
* Event untuk interaksi pengguna

Dengan JavaScript, website kamu tidak hanya statis, tetapi sudah bisa merespon interaksi pengguna.
