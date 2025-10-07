# Pratikum 1 - HTML Dasar
### NAMA : SURYA PUTRA DARMA JAYA
### NIM : 312410405
### KELAS : TI.24.A3

## 📁 Penjelasan Struktur Kode

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

<textarea> → Area teks yang bisa menampung banyak baris, cocok untuk menulis alamat.

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

