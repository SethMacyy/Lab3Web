# Pratikum 3
### NAMA : SURYA PUTRA DARMA JAYA
### NIM : 312410405
### KELAS : TI.24.A3

# 📁 Penjelasan Struktur Kode

## PENJELASAN lab3_list.html. ⬇️

### 1. Bagian Pembuka HTML

```html
<!DOCTYPE html>
<html lang="en">
```
### 2. Bagian `<head>`

```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
```

Penjelasan:

`<meta charset="UTF-8">` → Menentukan karakter encoding agar semua huruf dan simbol dapat ditampilkan dengan benar.

`<meta name="viewport" content="width=device-width, initial-scale=1.0">` → Membuat tampilan halaman responsif di perangkat mobile.

`<title>` → Menentukan judul tab browser: “HTML Lanjutan”.

### 3. Bagian `<style>` (CSS Internal)

```html
<style>
    form p > label {
        display: inline-block;
        width: 100px;
    }

    form input[type="text"], 
    form textarea {
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
Penjelasan CSS:

form p > label → Mengatur agar label sejajar dengan input (inline-block) dan lebarnya 100px.

form input[type="text"], form textarea → Memberi garis tepi hijau (#197a43) pada kotak input dan textarea.

form input[type="submit"] → Mengubah tampilan tombol:

Warna latar belakang hijau (#197a43)

Teks putih (#ffffff)

Huruf tebal (bold)

Padding 5px atas-bawah dan 15px kiri-kanan.

### 4. Bagian `<body>`

```html
<body>
    <header>
        <h1>Membuat Form</h1>
    </header>
```

`<header>` → Bagian kepala halaman yang berisi judul.

`<h1>` → Menampilkan teks besar “Membuat Form” sebagai judul utama.

### 5. Bagian Formulir `(<form>)`

```html
<form action="proses.php" method="post">
```

### ` 6.<fieldset>` dan `<legend>`
```html
<fieldset>
    <legend>Data Pelanggan</legend>
```
`<fieldset>` → Mengelompokkan elemen-elemen form menjadi satu bagian (kotak).

`<legend>` → Memberi judul pada grup field, yaitu “Data Pelanggan”.

### 7. Input Nama
```html
<p>
    <label for="nama">Nama</label>
    <input type="text" id="nama" name="nama">
</p>
```

`<label for="nama">` → Label yang terhubung dengan input melalui atribut for.

`<input type="text">` → Membuat kolom input teks.

id dan name digunakan untuk identifikasi data di backend (proses.php).

### 8. Input Alamat
```html
<p>
    <label for="alamat">Alamat</label>
    <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
</p>
```

`<textarea>` → Area teks yang bisa menampung banyak baris, cocok untuk menulis alamat.

cols="20" dan rows="3" → Mengatur ukuran tampilan kolom dan baris.

### 9. Input Jenis Kelamin

```html
<p>
    <label>Jenis Kelamin</label>
    <input id="jk_l" type="radio" name="kelamin" value="L">
    <label for="jk_l">Laki-laki</label>

    <input id="jk_p" type="radio" name="kelamin" value="P">
    <label for="jk_p">Perempuan</label>
</p>
```


`<input type="radio">` → Membuat tombol pilihan tunggal.

name="kelamin" → Menandakan kedua pilihan (Laki-laki & Perempuan) satu grup, sehingga hanya bisa memilih satu.

value="L" atau "P" → Nilai yang akan dikirim ke proses.php.

Label dengan for="jk_l" dan for="jk_p" → Mengaitkan teks label ke tombol radio.


### 10. Tombol Submit
```html
<p>
    <input type="submit" value="Login">
</p>
```

`<input type="submit">` → Tombol untuk mengirim data form.

value="Login" → Teks pada tombol.


### 11. Penutup
```html
</fieldset>
</form>
</body>
</html>
```

Menutup semua tag yang dibuka sebelumnya.

## PENJELASAN lab3_tabel.html. ⬇️

---

## 🧾 **Judul: Membuat Tabel (Table) di HTML**

Kode ini digunakan untuk menampilkan **tabel data Fakultas dan Program Studi** dengan tampilan sederhana menggunakan tag HTML dasar.

---

### 🧩 **1. Bagian Pembuka HTML**

```html
<!DOCTYPE html>
<html lang="en">
```

* `<!DOCTYPE html>` → Menandakan bahwa dokumen ini adalah **HTML5**.
* `lang="en"` → Menunjukkan bahasa utama halaman adalah **bahasa Inggris**.

---

### 🧠 **2. Bagian `<head>`**

```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
```

* `<meta charset="UTF-8">` → Agar teks ditampilkan dengan benar (mendukung karakter Latin, simbol, dan huruf Indonesia).
* `<meta name="viewport"...>` → Supaya tampilan tabel tetap rapi di layar HP maupun komputer.
* `<title>` → Menentukan judul tab di browser, yaitu **“HTML Lanjutan”**.

---

### 🧱 **3. Bagian Judul Halaman**

```html
<body>
    <header>
        <h1>Membuat Table</h1>
    </header>
</body>
```

* `<header>` → Bagian atas halaman yang berisi judul.
* `<h1>` → Menampilkan teks besar “**Membuat Table**” di atas halaman.

---

### 📊 **4. Bagian Tabel**

```html
<table border="1" cellpadding="6" cellspacing="0">
```

* `<table>` → Menandakan awal tabel.
* `border="1"` → Memberi **garis tepi (border)** pada tabel.
* `cellpadding="6"` → Menambah **jarak dalam sel (isi tabel)** agar teks tidak terlalu rapat.
* `cellspacing="0"` → Menghilangkan jarak antar sel supaya tabel tampak menyatu.

---

### 🧭 **5. Bagian Kepala Tabel (`<thead>`)**

```html
<thead>
    <tr>
        <th>No.</th>
        <th>Fakultas</th>
        <th>Program Studi</th>
    </tr>
</thead>
```

* `<thead>` → Bagian atas tabel (judul kolom).
* `<tr>` → Baris tabel.
* `<th>` → Kolom **judul tabel** (hurufnya otomatis tebal dan rata tengah).

🟢 **Hasil tampilan baris header:**

| No. | Fakultas | Program Studi |
| --- | -------- | ------------- |

---

### 🧩 **6. Bagian Isi Tabel (`<tbody>`)**

```html
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
```

#### Penjelasan:

* `<tbody>` → Tempat untuk **data isi tabel**.
* `<tr>` → Menandakan **baris** baru.
* `<td>` → Menandakan **isi kolom (cell)** pada tabel.

🔹 `rowspan="3"` pada kolom “Teknik” berarti kolom itu **menggabungkan 3 baris ke bawah**, jadi tulisan *Teknik* tampil di tengah tiga baris jurusan.

🟢 **Hasil tampilan:**

| No. | Fakultas | Program Studi      |
| --- | -------- | ------------------ |
| 1.  | Teknik   | Teknik Informatika |
| 2.  |          | Teknik Industri    |
| 3.  |          | Teknik Lingkungan  |

---

### 🔚 **7. Penutup**

```html
</table>
</html>
```

* `</table>` → Menutup tabel.
* `</html>` → Menutup seluruh dokumen HTML.

---


---

## 🧾 **Judul: Membuat Formulir (Form) Data Pelanggan di HTML**

Kode ini digunakan untuk membuat **form input data pelanggan** menggunakan HTML dan CSS agar tampilannya lebih rapi dan menarik.
Form ini berisi kolom **Nama**, **Alamat**, **Jenis Kelamin**, dan **tombol kirim (Login)**.

---

### 🧩 **1. Bagian Pembuka HTML**

```html
<!DOCTYPE html>
<html lang="en">
```

* `<!DOCTYPE html>` → Menandakan dokumen ini memakai **HTML5**.
* `lang="en"` → Menunjukkan bahwa bahasa utama dokumen adalah **Inggris**.

---

### 🧠 **2. Bagian `<head>`**

```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
```

* `<meta charset="UTF-8">` → Agar karakter seperti huruf dan simbol tampil dengan benar.
* `<meta name="viewport"...>` → Membuat halaman **responsif** (pas di layar HP dan laptop).
* `<title>` → Judul halaman yang muncul di tab browser: **"HTML Lanjutan"**.

---

### 🎨 **3. Bagian CSS (Gaya Tampilan)**

```html
<style>
    form p > label {
        display: inline-block;
        width: 100px;
    }

    form input[type="text"], 
    form textarea {
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

#### Penjelasan gaya CSS:

* `form p > label` → Label dibuat sejajar (inline-block) dengan lebar 100px supaya rata kiri.
* `form input[type="text"], form textarea` → Kolom teks dan area tulisan diberi **garis hijau (#197a43)**.
* `form input[type="submit"]` → Tombol kirim diberi:

  * Warna latar hijau
  * Tulisan putih tebal
  * Sedikit jarak dalam tombol (padding)

🟢 **Tujuan:** agar form terlihat rapi, berwarna, dan mudah dibaca.

---

### 🧱 **4. Bagian Judul Halaman**

```html
<header>
    <h1>Membuat Form</h1>
</header>
```

* `<header>` → Bagian kepala halaman.
* `<h1>` → Menampilkan judul besar **"Membuat Form"** di atas halaman.

---

### 🧾 **5. Bagian Formulir (`<form>`)**

```html
<form action="proses.php" method="post">
```

* `action="proses.php"` → Menentukan file tujuan untuk **memproses data** (biasanya file PHP).
* `method="post"` → Mengirim data **secara tersembunyi** (tidak tampil di URL, lebih aman).

---

### 📦 **6. Fieldset dan Legend**

```html
<fieldset>
    <legend>Data Pelanggan</legend>
```

* `<fieldset>` → Membuat kotak pembatas untuk kelompok form.
* `<legend>` → Judul kotak, yaitu **“Data Pelanggan”**.

---

### 🧍 **7. Input Nama**

```html
<p>
    <label for="nama">Nama</label>
    <input type="text" id="nama" name="nama">
</p>
```

* `<label for="nama">` → Label teks “Nama” yang terhubung dengan kolom input.
* `<input type="text">` → Kolom teks untuk menulis nama pelanggan.
* `name="nama"` → Nama variabel yang akan dikirim ke server.

🟢 **Tampilannya:** kolom untuk mengetik nama.

---

### 🏠 **8. Input Alamat**

```html
<p>
    <label for="alamat">Alamat</label>
    <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
</p>
```

* `<textarea>` → Area teks besar untuk menulis alamat lengkap.
* `cols="20"` dan `rows="3"` → Menentukan ukuran kotak teks.

🟢 **Tampilannya:** kotak teks lebih besar, bisa untuk beberapa baris.

---

### 🚻 **9. Input Jenis Kelamin**

```html
<p>
    <label>Jenis Kelamin</label>
    <input id="jk_l" type="radio" name="kelamin" value="L">
    <label for="jk_l">Laki-laki</label>

    <input id="jk_p" type="radio" name="kelamin" value="P">
    <label for="jk_p">Perempuan</label>
</p>
```

**Penjelasan:**

* `<input type="radio">` → Membuat tombol bulat untuk memilih salah satu opsi.
* `name="kelamin"` → Mengelompokkan kedua tombol supaya hanya **satu yang bisa dipilih**.
* `value="L"` dan `value="P"` → Nilai yang dikirim ke server (L = Laki-laki, P = Perempuan).
* `<label for="jk_l">` dan `<label for="jk_p">` → Menampilkan teks di samping tombol radio.

🟢 **Tampilannya:**

```
Jenis Kelamin: ○ Laki-laki   ○ Perempuan
```

---

### 🖱️ **10. Tombol Submit**

```html
<p>
    <input type="submit" value="Login">
</p>
```

* `<input type="submit">` → Tombol untuk mengirim semua data di form.
* `value="Login"` → Tulisan pada tombolnya adalah **“Login”**.

🟢 **Tampilannya:** tombol berwarna hijau bertuliskan “Login”.

---

### 🔚 **11. Penutup**

```html
</fieldset>
</form>
</body>
</html>
```

* `</fieldset>` → Menutup kotak form.
* `</form>` → Menutup form.
* `</body>` dan `</html>` → Menutup seluruh halaman HTML.

---

## ✅ **Kesimpulan Singkat**

---

### 🧾 **1. Membuat Formulir (Form)**

➡️ Kode ini digunakan untuk membuat **form input data pelanggan** seperti *Nama*, *Alamat*, dan *Jenis Kelamin*, dengan tambahan tombol **“Login”** untuk mengirim data.
Form ini sudah diberi **gaya (CSS)** agar tampilannya rapi, berwarna hijau, dan mudah dibaca.
🔹 **Fungsinya:** Mengumpulkan data dari pengguna dan mengirimkannya ke file `proses.php` untuk diproses lebih lanjut.

---

### 📊 **2. Membuat Tabel (Table)**

➡️ Kode ini digunakan untuk menampilkan **data Fakultas dan Program Studi** dalam bentuk tabel.
Menggunakan atribut seperti `border`, `cellpadding`, `cellspacing`, dan `rowspan` agar tabel tampak rapi dan kolom Fakultas bisa menyatu dalam beberapa baris.
🔹 **Fungsinya:** Menyajikan data secara **terstruktur dan mudah dibaca**.

---

### 💻 **3. Form HTML Lanjutan dengan CSS**

➡️ Kode ini merupakan versi lebih lengkap dari form sebelumnya, yang memanfaatkan **CSS internal** untuk mempercantik tampilan.
Terdapat bagian header, fieldset, label, input teks, textarea, radio button, dan tombol kirim.
🔹 **Fungsinya:** Membuat tampilan form **lebih interaktif, teratur, dan menarik secara visual**.

---

### 🧩 **Kesimpulan Umum**

Ketiga kode tersebut menunjukkan **dasar HTML lanjutan**, yaitu cara membuat **formulir** dan **tabel** dengan tampilan yang rapi menggunakan **CSS**.
Semua digunakan untuk **menginput dan menampilkan data** secara terstruktur di halaman web.
