# Lab3Web - HTML Lanjutan: List, Table, dan Form

Repository ini berisi hasil praktikum pemrograman web tentang pembuatan List, Table, dan Form menggunakan HTML dan CSS.

## Informasi Mahasiswa
- **Nama**: Abdi Putra Perdana
- **NIM**: 312410426
- **Kelas**: TI 24 A3
- **Mata Kuliah**: Pemrograman Web
- **Dosen Pengampu**: Agung Nugroho

---

## Daftar Isi
1. [Membuat List](#1-membuat-list)
2. [Membuat Table](#2-membuat-table)
3. [Membuat Form](#3-membuat-form)
4. [Pertanyaan dan Tugas](#4-pertanyaan-dan-tugas)

---

## 1. Membuat List

### File: `lab3_list.html`

### Langkah 1: Persiapan Dokumen HTML

Buat file `lab3_list.html` dengan struktur dasar:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat List</h1>
    </header>
</body>
</html>
```

---

### Langkah 2: Membuat Ordered List

Tambahkan kode untuk membuat Ordered List:

```html
<section id="order-list">
    <h2>Ordered List</h2>
    <ol>
        <li>Pemrograman Web</li>
        <li>Sistem Informasi</li>
        <li>Basis Data 2</li>
    </ol>
</section>
```

**Screenshot:**

<img width="1919" height="1078" alt="image" src="https://github.com/user-attachments/assets/91c8aeac-e79b-4c66-93f4-35b0b5221e35" />


**Penjelasan:**
- Tag `<ol>` digunakan untuk membuat ordered list (list terurut)
- Tag `<li>` untuk membuat item dalam list
- Secara default ordered list akan menggunakan penomoran 1, 2, 3, dst

---

### Langkah 3: Membuat Unordered List

Tambahkan kode untuk membuat Unordered List:

```html
<section id="unorder-list">
    <h2>Unordered List</h2>
    <ul type="square">
        <li>Jaringan Komputer</li>
        <li>Struktur Data</li>
        <li>Algoritma &amp; Pemrograman</li>
    </ul>
</section>
```

**Screenshot:**

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/e177ef90-f449-4837-b7f1-80e861e81782" />


**Penjelasan:**
- Tag `<ul>` untuk membuat unordered list (list tidak terurut)
- Atribut `type="square"` mengubah bullet point menjadi kotak
- `&amp;` adalah entity HTML untuk karakter `&`

---

### Langkah 4: Membuat Description List

Tambahkan kode untuk membuat Description List:

```html
<section id="unorder-list">
    <h2>Description List</h2>
    <dl>
        <dt>Fakultas Teknik</dt>
        <dd>Teknik Industri</dd>
        <dd>Teknik Informatika</dd>
        <dd>Teknik Lingkungan</dd>
        <dt>Fakultas Ekonomi dan Bisnis</dt>
        <dd>Akuntansi</dd>
        <dd>Manajemen</dd>
        <dd>Bisnis Digital</dd>
    </dl>
</section>
```

**Screenshot:**

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/55373dc3-7cc0-4bc3-a47c-7a5c25abf456" />


**Penjelasan:**
- `<dl>` (description list) tag untuk memulai description list
- `<dt>` (description term) tag untuk membuat kata yang akan dideskripsikan
- `<dd>` (description description) tag untuk membuat penjelasan dari kata

---

## 2. Membuat Table

### File: `lab3_tabel.html`

### Langkah 1: Persiapan Dokumen HTML

Buat file `lab3_tabel.html`:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat Table</h1>
    </header>
</body>
</html>
```

---

### Langkah 2: Membuat Tabel Sederhana

Tambahkan kode untuk membuat tabel:

```html
<table border="1" cellpadding="4" cellspacing="0">
    <thead>
        <tr>
            <th>No.</th>
            <th>Fakultas</th>
            <th>Program Studi</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1.</td>
            <td>Teknik</td>
            <td>Teknik Informatika</td>
        </tr>
        <tr>
            <td>2.</td>
            <td>Teknik</td>
            <td>Teknik Industri</td>
        </tr>
        <tr>
            <td>3.</td>
            <td>Teknik</td>
            <td>Teknik Lingkungan</td>
        </tr>
    </tbody>
</table>
```

**Screenshot:**

<img width="1919" height="1076" alt="Screenshot 2025-10-07 200834" src="https://github.com/user-attachments/assets/4c7937de-348f-469c-9bbd-80336c1f5acc" />


**Penjelasan:**
- `<table>` untuk membuat tabel
- `<thead>` untuk membungkus bagian kepala tabel
- `<tbody>` untuk membungkus bagian body tabel
- `<tr>` untuk membuat baris tabel
- `<th>` untuk membuat judul kolom (table header)
- `<td>` untuk membuat kolom data (table data)
- `border="1"` membuat border tabel
- `cellpadding="4"` mengatur jarak antara isi sel dengan border
- `cellspacing="0"` mengatur jarak antar sel

---

### Langkah 3: Menggabungkan Sel Data

Untuk menggabungkan sel data, gunakan atribut `rowspan` dan `colspan`:

```html
<table border="1" cellpadding="6" cellspacing="0">
    <thead>
        <tr>
            <th>No.</th>
            <th>Fakultas</th>
            <th>Program Studi</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>1.</td>
            <td rowspan="3">Teknik</td>
            <td>Teknik Informatika</td>
        </tr>
        <tr>
            <td>2.</td>
            <td>Teknik Industri</td>
        </tr>
        <tr>
            <td>3.</td>
            <td>Teknik Lingkungan</td>
        </tr>
    </tbody>
</table>
```

**Screenshot:**

<img width="1917" height="1079" alt="image" src="https://github.com/user-attachments/assets/1bd1ac73-0231-4aba-aae1-497add82877f" />


**Penjelasan:**
- `rowspan="3"` menggabungkan sel secara vertikal (3 baris)
- `colspan` digunakan untuk menggabungkan sel secara horizontal
- Penggabungan sel berguna untuk menghindari pengulangan data

---

## 3. Membuat Form

### File: `lab3_form.html`

### Langkah 1: Persiapan Dokumen HTML

Buat file `lab3_form.html`:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat Form</h1>
    </header>
</body>
</html>
```

---

### Langkah 2: Membuat Form

Tambahkan kode untuk membuat form:

```html
<form action="proses.php" method="post">
    <fieldset>
        <legend>Data Pelanggan</legend>
        <p>
            <label for="nama">Nama</label>
            <input type="text" id="nama" name="nama">
        </p>
        <p>
            <label for="alamat">Alamat</label>
            <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
        </p>
        <p>
            <label>Jenis Kelamin</label>
            <input id="jk_l" type="radio" name="kelamin" value="L" /><label
for="jk_l">Laki-laki</label>
            <input id="jk_p" type="radio" name="kelamin" value="P" /><label
for="jk_p">Perempuan</label>
        </p>
        <p><input type="submit" value="Login"></p>
    </fieldset>
</form>
```

**Screenshot:**

<img width="1919" height="1078" alt="image" src="https://github.com/user-attachments/assets/0f3d7cf9-d1c0-4053-846b-e667b4dc62ae" />


**Penjelasan:**
- `<form>` untuk membuat form
- `action="proses.php"` menentukan file yang akan memproses data form
- `method="post"` menentukan metode pengiriman data (POST/GET)
- `<fieldset>` untuk mengelompokkan elemen form
- `<legend>` untuk membuat judul fieldset
- `<label>` untuk membuat label input
- `<input type="text">` untuk input text satu baris
- `<textarea>` untuk input text multi-baris
- `<input type="radio">` untuk pilihan radio button
- `<input type="submit">` untuk tombol submit

---

### Langkah 3: Menambahkan Style pada Form

Tambahkan CSS untuk mempercantik form:

```html
<style>
form p > label {
    display: inline-block;
    width: 100px;
}
form input[type="text"], form textarea {
    border: 1px solid #197a43;
}
form input[type="submit"] {
    border: 1px solid #197a43;
    background-color: #197a43;
    color: #ffffff;
    font-weight: bold;
    padding: 5px 15px;
}
</style>
```

**Screenshot:**

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/b76251e4-5b70-439e-9c78-a8d008699f1f" />

**Penjelasan:**
- CSS digunakan untuk styling form agar lebih menarik
- `display: inline-block` untuk mengatur layout label
- `width: 100px` untuk membuat lebar label konsisten
- Border, background, dan padding diatur untuk mempercantik tampilan

---

## 4. Pertanyaan dan Tugas

### Pertanyaan
**Buatlah form yang menampilkan dropdown menu dan listbox dengan multiple selection.**

### Jawaban

### File: `lab3_form_tugas.html`

Membuat form pendaftaran mahasiswa dengan dropdown menu dan multiple selection:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form dengan Dropdown dan Multiple Selection</title>
    <style>
        form p > label {
            display: inline-block;
            width: 150px;
            font-weight: bold;
        }
        form input[type="text"], 
        form input[type="email"],
        form select {
            border: 1px solid #197a43;
            padding: 5px;
            width: 300px;
        }
        form select[multiple] {
            height: 120px;
        }
        form input[type="submit"] {
            border: 1px solid #197a43;
            background-color: #197a43;
            color: #ffffff;
            font-weight: bold;
            padding: 8px 20px;
            cursor: pointer;
        }
        fieldset {
            border: 2px solid #197a43;
            border-radius: 5px;
            padding: 20px;
        }
        legend {
            color: #197a43;
            font-weight: bold;
            font-size: 18px;
            padding: 0 10px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Form Pendaftaran Mahasiswa</h1>
    </header>

    <form action="proses.php" method="post">
        <fieldset>
            <legend>Data Mahasiswa</legend>
            
            <p>
                <label for="nama">Nama</label>
                <input type="text" id="nama" name="nama">
            </p>
            
            <p>
                <label for="nim">NIM</label>
                <input type="text" id="nim" name="nim">
            </p>
            
            <p>
                <label>Jenis Kelamin</label>
                <input id="jk_l" type="radio" name="kelamin" value="L">
                <label for="jk_l" style="width: auto;">Laki-laki</label>
                <input id="jk_p" type="radio" name="kelamin" value="P">
                <label for="jk_p" style="width: auto;">Perempuan</label>
            </p>
            
            <!-- Dropdown Menu -->
            <p>
                <label for="fakultas">Fakultas</label>
                <select id="fakultas" name="fakultas">
                    <option value="">-- Pilih Fakultas --</option>
                    <option value="teknik">Fakultas Teknik</option>
                    <option value="ekonomi">Fakultas Ekonomi dan Bisnis</option>
                    <option value="pertanian">Fakultas Pertanian</option>
                    <option value="kedokteran">Fakultas Kedokteran</option>
                </select>
            </p>
            
            <!-- Multiple Selection Listbox -->
            <p>
                <label for="matkul">Mata Kuliah</label>
                <select id="matkul" name="matkul[]" multiple>
                    <option value="pweb">Pemrograman Web</option>
                    <option value="si">Sistem Informasi</option>
                    <option value="bd">Basis Data</option>
                    <option value="rpl">Rekayasa Perangkat Lunak</option>
                    <option value="jarkom">Jaringan Komputer</option>
                </select>
            </p>
            
            <p>
                <label></label>
                <input type="submit" value="Submit">
            </p>
        </fieldset>
    </form>
</body>
</html>
```

**Screenshot:**

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/8d69ff5f-9177-465e-8d83-5a5d710dede7" />

**Penjelasan:**

**1. Dropdown Menu (Select):**
- Tag `<select>` digunakan untuk membuat dropdown
- Tag `<option>` untuk setiap pilihan dalam dropdown
- Atribut `value` berisi nilai yang akan dikirim ke server
- User hanya bisa memilih satu pilihan

**2. Multiple Selection Listbox:**
- Tag `<select>` dengan atribut `multiple` untuk multiple selection
- Atribut `name="matkul[]"` menggunakan array untuk menampung multiple values
- User bisa memilih lebih dari satu pilihan dengan menekan **Ctrl** (Windows) atau **Cmd** (Mac)
- Atribut `size` bisa ditambahkan untuk menentukan jumlah item yang terlihat

---

## Kesimpulan

Dari praktikum ini, saya telah mempelajari:

1. ✅ Cara membuat berbagai jenis List (Ordered, Unordered, Description)
2. ✅ Cara membuat Table dengan penggabungan sel (rowspan & colspan)
3. ✅ Cara membuat Form dengan berbagai input type
4. ✅ Cara implementasi Dropdown Menu (select)
5. ✅ Cara implementasi Multiple Selection Listbox
6. ✅ Cara styling menggunakan CSS untuk tampilan yang lebih menarik

---

**© 2025 - Praktikum Pemrograman Web - Universitas Pelita Bangsa**
