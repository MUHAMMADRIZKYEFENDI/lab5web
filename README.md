# lab5web
### Langkah-langkah Praktikum 
Persiapan membuat dokumen HTML dengan nama file lab5_javascript.html seperti berikut.
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>

<body>
    <h1>Pengenalan JavaScript</h1>
    <h3>Contoh document.write dan console.log</h3>
    <script>
        document.write("Hello World");
        console.log("Hello World"); 
    </script>
</body>

</html>
```

hasil browser nya sebagai berikut!!!
![Screenshot (255)](https://github.com/user-attachments/assets/5dbe3f4b-b042-412d-acf5-92a60eb72e28)

# Javascrip Dasar 
### 1.Pemakaian Alert sebagai property window.
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>alert box</title>
</head>

<body>
    <script language="javascript">
        <!--window.alert("ini merupakan pesan anda");//-->
    </script>
</body>

</html>
```
hasil browsernya!!!
![Screenshot (257)](https://github.com/user-attachments/assets/20e92478-8a6a-4f4a-99db-b313c69b4437)
### 2.Pemakaian method dalam objek 
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>skrip javascript</title>
</head>

<body>
    percobaan memakai javascript:<br>
    <script language="JavaScript">
        <!--document.write("selamat mecoba javascript<br>");
        document.write("semoga sukses!");
        //-->
    </script>

</body>

</html>
```
hasil browsernya!!
![Screenshot (256)](https://github.com/user-attachments/assets/957be0c5-5dff-4480-945a-b6c92b506564)

### 3.Pemakaian Prompt
```
<!DOCTYPE html>
<html>
<head>
    <title>pemasukan data</title>
</head>
<body>
    <script>
        var nama = prompt("Masukkan nama anda", "nama lengkap");
        document.write("Hai, " + nama);
    </script>
</body>
</html>
```
hasil browsernya!!
![Screenshot (259)](https://github.com/user-attachments/assets/de1aa8dd-ac5e-4df9-8b65-55502d913584)
### 4.Pembuatan fungsi dan cara pemanggilannya
```
<!DOCTYPE html>
<html>
<head>
    <title>Contoh Pembuatan Fungsi</title>
</head>
<body>
    <script>
        function pesan() {
            alert("Memanggil javascript lewat fungsi");
        }
    </script>

    <button onclick="pesan()">Klik Saya</button>
</body>
</html>
```
hasil browsernya!!!

![Screenshot (260)](https://github.com/user-attachments/assets/1f41af63-1ed7-4057-98f0-757a8c4bbaa6)

# Dasar Pemrograman Di Javascript 
### 1.Operasi dasar aritmatika
```
<!DOCTYPE html>
<html lang="id">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contoh Program JavaScript</title>
    <script>
        function test(val1, val2) {
            document.write("<br>Perkalian: " + (val1 * val2) + "<br>");
            document.write("Pembagian: " + (val1 / val2) + "<br>");
            document.write("<br>Penjumlahan: " + (val1 + val2) + "<br>");
            document.write("Pengurangan: " + (val1 - val2) + "<br>");
            document.write("Pangkat: " + (Math.pow(val1, val2)) + "<br>");
        }
    </script>
</head>

<body>
    <input type="button" name="button" value="Arithmetic" onclick="test(9.4, 2)">
</body>

</html>
```
hasil browser nya!!
![Screenshot (266)](https://github.com/user-attachments/assets/0d74800a-c1b4-4ddf-b156-23bb30b518eb)

### 2.Seleksi kondisi (if..else) 
```
<!DOCTYPE html>
<html lang="id">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contoh If-Else</title>
</head>

<body>
    <script>
        var nilai = prompt("Nilai (0-100):");
        var hasil;
        
        if (nilai >= 60) {
            hasil = "lulus";
        } else {
            hasil = "tidak lulus";
        }

        document.write("Hasil: " + hasil);
    </script>
</body>

</html>
```
hasil browsernya!!
![Screenshot (267)](https://github.com/user-attachments/assets/42ff86d7-6d0c-42a2-8fe1-57a3caf931d4)
### 3.Penggunaan operator switch untuk seleksi kondisi 
```
<!DOCTYPE html>
<html lang="id">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contoh Program JavaScript</title>
    <script>
        function test() {
            var val = window.prompt("Input nilai (1-5):");
            switch (val) {
                case "1":
                    document.write("Bilangan satu");
                    break;
                case "2":
                    document.write("Bilangan dua");
                    break;
                case "3":
                    document.write("Bilangan tiga");
                    break;
                case "4":
                    document.write("Bilangan empat");
                    break;
                case "5":
                    document.write("Bilangan lima");
                    break;
                default:
                    document.write("Bilangan lainnya");
                    break;
            }
        }
    </script>
</head>

<body>
    <input type="button" name="button" value="Switch" onclick="test()">
</body>

</html>
```
hasil browsernya!!
![Screenshot (268)](https://github.com/user-attachments/assets/d963d806-9f76-4966-a058-eaadd6e464c4)

# Pembuatan Form 
### 1.Form Input
```
<!DOCTYPE html>
<html lang="id">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form Input</title>
    <script language="javascript">
        function test() {
            var val = document.kirim.T1.value;
            if (val % 2 === 0) {
                document.kirim.T2.value = "Bilangan genap";
            } else {
                document.kirim.T2.value = "Bilangan ganjil";
            }
        }
    </script>
</head>

<body>
    <form method="POST" name="kirim">
        <p>Nilai: <input type="text" name="T1" size="20"></p>
        <p>MERUPAKAN BIL: <input type="text" name="T2" size="70" readonly></p>
        <p><input type="button" value="TEBAK" name="btnTebak" onclick="test()"></p>
    </form>
</body>

</html>
```
hasil browsernya!!

![Screenshot (272)](https://github.com/user-attachments/assets/bda703df-c72e-4220-8ed7-ab1518c89175)
### 2.Form Button. 
```
<!DOCTYPE html>
<html lang="id">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Objek Document</title>
    <script language="javascript">
        function ubahLatarBelakang(warna) {
            document.bgColor = warna;
        }

        function ubahWarnaTeks(warna) {
            document.fgcolor = warna;
        }
    </script>
</head>

<body>
    <h1>Tes</h1>
    <form>
        <input type="button" value="Latar Belakang Putih" onclick="ubahLatarBelakang('white')">
        <input type="button" value="Latar Belakang Kuning" onclick="ubahLatarBelakang('yellow')">
        <input type="button" value="Latar Belakang Biru" onclick="ubahLatarBelakang('blue')">
    </form>

    <script language="javascript">
        document.write("Disindifikasi terakhir pada: " + document.lastModified);
    </script>
</body>

</html>
```
hasil browsernya!!
![Screenshot (270)](https://github.com/user-attachments/assets/a4ef8e0d-c845-4c9c-80f5-59a4a3d2a877)

# HTML DOM 
### Pilihan menggunakan checkBox dengan perhitungan otomatis
```
<!DOCTYPE html>
<html lang="id">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Daftar Menu</title>
    <script>
        function hitung(ele) {
            var total = document.getElementById("total").value;
            total = (total ? parseInt(total) : 0);
            var harga = 0;

            if (ele.checked) {
                harga = parseInt(ele.value);
                total += harga; // Tambahkan harga ke total
            } else {
                harga = parseInt(ele.value);
                total -= harga; // Kurangi harga dari total
            }

            document.getElementById("total").value = total; // Update total
        }
    </script>
</head>

<body>
    <h1>Daftar Menu Makanan</h1>
    <label>
        <input type="checkbox" value="5000" id="menu1" onclick="hitung(this);" /> Ayam Goreng Rp. 5.000
    </label><br />
    <label>
        <input type="checkbox" value="500" id="menu2" onclick="hitung(this);" /> Tempe Goreng Rp. 500
    </label><br />
    <label>
        <input type="checkbox" value="2500" id="menu3" onclick="hitung(this);" /> Telur Dadar Rp. 2.500
    </label><hr />
    <strong>Total Bayar Rp. <input id="total" type="text" readonly /></strong>
</body>

</html>
```
hasil browsernya!!

![Screenshot (271)](https://github.com/user-attachments/assets/c21ce041-3a7e-422f-893a-4c50236628da)

# PERTANYAAN DAN TUGAS
# 1. Buat script untuk melakukan validasi pada isian form.
```
<!DOCTYPE html>
<html lang="id">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form dengan Validasi</title>
    <script>
        function validateForm() {
            // Mengambil nilai dari input
            var nama = document.forms["myForm"]["nama"].value;
            var email = document.forms["myForm"]["email"].value;
            var password = document.forms["myForm"]["password"].value;
            var errorMessages = "";

            // Validasi field nama
            if (nama == "") {
                errorMessages += "- Nama harus diisi.\n";
            }

            // Validasi format email
            var emailPattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            if (email == "") {
                errorMessages += "- Email harus diisi.\n";
            } else if (!emailPattern.test(email)) {
                errorMessages += "- Format email tidak valid.\n";
            }

            // Validasi password
            if (password == "") {
                errorMessages += "- Password harus diisi.\n";
            } else if (password.length < 8) {
                errorMessages += "- Password minimal 8 karakter.\n";
            }

            // Menampilkan pesan error jika ada
            if (errorMessages != "") {
                alert("Error:\n" + errorMessages);
                return false; // Mencegah form dikirim jika ada error
            }

            return true; // Form akan dikirim jika tidak ada error
        }
    </script>
</head>

<body>
    <h1>Form Registrasi</h1>
    <form name="myForm" onsubmit="return validateForm()">
        <label for="nama">Nama:</label>
        <input type="text" id="nama" name="nama"><br><br>

        <label for="email">Email:</label>
        <input type="text" id="email" name="email"><br><br>

        <label for="password">Password:</label>
        <input type="password" id="password" name="password"><br><br>

        <input type="submit" value="Daftar">
    </form>
</body>

</html>
```
HASIL BROWSERNYA
![Screenshot (273)](https://github.com/user-attachments/assets/816f42e2-c4a5-41c9-84f3-740dc610c7ea)
