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
# Dasar Pemrograman Di Javascript 
### 1.Operasi dasar aritmatika
```
