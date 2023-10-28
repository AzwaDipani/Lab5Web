# Lab5web

Nama : Muhammad Azwa Dipani

NIM  : 312210417

Kelas : TI.22.A1

## Instruksi Praktikum
1. Persiapkan text editor misalnya VSCode.
2. Buat folder baru dengan nama Lab5Web
3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
4. Lakukan validasi dokumen html dengan mengakses http://validator.w3.org


## Langkah-langkah Praktikum
> - Persiapan membuat dokumen HTML dengan nama file `lab5_javascript.html` seperti berikut :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Mengenal JavaScript</title>
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

![img](pictures/Screenshot%20(173).png)


**1. Javascript Dasar**
> - Pemakaian `Alert` sebagai property window
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>alert box</title>
</head>
<body>
    <script language = "javascript" >
    <!-- 
    window.alert("ini merupakan pesan untuk anda");
    //-->
    </script>
</body>
</html>
```

![img](pictures/Screenshot%20(174).png)


> - Pemakaian `Method` dalam objek
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>skrip javascript</title>
</head>
<body>
percobaan memakai javascript:<br>
    <script language = "javascript" >
    <!-- 
    document.write("selamat mencoba javascript<br>");
    document.write("semoga sukses!");
    //-->
    </script>
</body>
</html>
```

![img](pictures/Screenshot%20(175).png)


> - Pemakaian `Prompt`
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>pemasukan data</title>
</head>
<body>
    <script language = "javascript" >
    <!-- 
    var nama = prompt("siapa nama anda?","masukkan nama anda");
    document.write("hai, " + nama);
    //-->
    </script>
</body>
</html>
```



![video](videos/Proyek%20tanpa%20judul.mp4)


> - Pembuatan `Fungsi` dan cara pemanggilannya
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>contoh program javascript</title>
    <script language="javascript">
    function pesan(){
        alert ("memanggil javascript lewat body onload")
    }
    </script>
</head>
<body onload=pesan()>
</body>
</html>
```

![img](pictures/Screenshot%20(176).png)


**2. Dasar Pemrograman di Javascript**
> - Operasi dasar `aritmatika`
```
<html>
<head>
    <title>contoh program javascript</title>

    <script language="javascript">
    function test (val1,val2)
    {
        document.write("<br>"+"perkalian : val1*val2 "+"<br>")
        document.write(val1*val2)
        document.write("<br>"+"pembagian : val1/val2 "+"<br>")
        document.write(val1/val2)
        document.write("<br>"+"penjumlahan : val1+val2 "+"<br>")
        document.write(val1+val2)
        document.write("<br>"+"pengurangan : val1-val2 "+"<br>")
        document.write(val1-val2)
        document.write("<br>"+"modulus : val1%val2 "+"<br>")
        document.write(val1%val2)
    }
    </script>
</head>
<body>
    <input type="button" name="button1" value="arithmetic" onclick=test(9,4)>
    </body>
    </html>
```




> - Seleksi kondisi `(if..else)`
```
<html>
<head>
    <title>contoh if-else</title>
</head>
<body>
    <script language = "javascript">
    <!--
      var nilai = prompt("nilai (0-100): ", 0);
      var hasil = "";
      if (nilai >= 60)
      hasil = "lulus";
      else 
      hasil = "tidak lulus";
      document.write("hasil:" + hasil);   
    //-->
    </script>
</body>
</html>
```


https://github.com/syifaaurellia/Lab5web/assets/115867244/f9918a4c-8a33-48ba-86d4-6dda773e2ba2


> - Penggunaan operator `switch` untuk seleksi kondisi
```
<html>
<head>
    <title>contoh program javascript</title>

<script language="javascript">
function test ()
{
    val1=window.prompt("input nilai (1-5):")
    switch (val1)
    {
        case "1" :
            document.write("bilangan satu")
            break
        case "2" :
            document.write("bilangan dua")
            break
        case "3" :
            document.write("bilangan tiga")
            break
        case "4" :
            document.write("bilangan empat")
            break
        case "5" :
            document.write("bilangan lima")
            break
        default :
            document.write("bilangan lainnya")
    }
}
</script>
</head>
<body>
    <input type="button" name="button1" value="switch" onclick=test()>
</body>
</html>
```


https://github.com/syifaaurellia/Lab5web/assets/115867244/e5991430-6d1f-4663-8584-72b688e0f253



**3. Pembuatan Form**
> - Form `Input`
```
<html>
<head>
    <script language="javascript">
    function test () {
        var val1=document.kirim.T1.value
        if (val1%2==0)
            document.kirim.T2.value="bilangan genap"
        else
            document.kirim.T2.value="bilangan ganjil"
    }
    </script>
</head>
<body>
    <form method="POST" name="kirim">
        <p>BIL <input type="text" name="T1" size="20">
        MERUPAKAN BIL <input type="text" name="T2" size="20"></p>
        <p><input type="button" value="TEBAK" name="B1" onclick=test()></p>
    </form>
</body>
</html>
```


https://github.com/syifaaurellia/Lab5web/assets/115867244/94dd2d32-cb81-4de0-a5ab-9aac2632d634


> - Form `Button`
```
<html>
<head>
    <title>objek document</title>
</head>
<body>
    <script language = "javascript">
    <!--
    function ubahWarnaLB(warna) {
        document.bgColor = warna;
    }    
    function ubahWarnaLD(warna) {
        document.fgColor = warna;
    }
    //-->
    </script>

    <h1>tes</h1>
    <form>
        <input type="button" value="Latar Belakang Hijau" onclick="ubahWarnaLB('GREEN')">
        <input type="button" value="Latar Belakang Putih" onclick="ubahWarnaLB('WHITE')">
        <input type="button" value="Teks Kuning" onclick="ubahWarnaLD('YELLLOW')">
        <input type="button" value="Teks Biru" onclick="ubahWarnaLD('BLUE')">
    </form>
    <script language = "javascript">
    <!--
    document.write("Dimodifikasi terakhir pada " +
    document.lastModified);
    //-->
    </script>
</body>
</html>
```


https://github.com/syifaaurellia/Lab5web/assets/115867244/1b7438de-a501-47fe-a513-aa92d3ac862a


**4. HTML DOM**
> - Pilihan menggunakan `checkbox` dengan perhitungan otomatis
```
<!--
File: daftar_menu.html
-->
<html>
<head>
    <title>Daftar Menu</title>
    <script>
        function hitung(ele) {
            var total = document.getElementById('total').value;
                total = (total ? parseInt(total) : 0);
            var harga = 0;

            if (ele.checked) {
                harga = ele.value
                total += parseInt(harga);
            } else {
                harga = ele.value;
                if (total > 0)
                    total -= parseInt(harga);
            }
            document.getElementById('total').value = total;
        }
    </script>
</head>
<body>
    <h1>Daftar Menu Makanan</h1>
    <label><input type="checkbox" value="5000" id="menu1" onclick="hitung(this);" /> Ayam Goreng Rp. 5.000</label><br />
    <label><input type="checkbox" value="500" id="menu2" onclick="hitung(this);" /> Tempe Goreng Rp. 5.00</label><br />
    <label><input type="checkbox" value="2500" id="menu3" onclick="hitung(this);" /> Telur Dadar Rp. 2.500</label><br />
    <strong>Total Bayar: Rp. <input id="total" type="text" /></strong>
</body>
</html>
```


https://github.com/syifaaurellia/Lab5web/assets/115867244/6838d230-b904-4095-a151-ae2af4bd5b81



## Pertanyaan dan Tugas
**1. Buat script untuk melakukan `validasi` pada isian form**
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulir Validasi</title>

    <!-- my styles css -->
    <link rel="stylesheet" href="style.css">
    <script>
        function validateForm() {
            // Dapatkan referensi ke elemen-elemen formulir
            var nama = document.forms["myForm"]["nama"].value;
            var email = document.forms["myForm"]["email"].value;

            // Lakukan validasi
            if (nama == "") {
                alert("Nama anda belum diisi");
                return false;
            }

            if (email == "") {
                alert("Email anda belum diisi");
                return false;
            }

            // Validasi apakah email sesuai dengan format yang benar
            var emailPattern = /^[a-zA-Z0-9._-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,4}$/;

            if (!emailPattern.test(email)) {
                alert("Email Anda tidak valid.");
                return false;
            }
        }
    </script>
</head>
<body>
    <h1>Formulir Validasi</h1>
    <div class="container">
        <form name="myForm" onsubmit="return validateForm()" method="post">
            <div class="input-group">
                <input type="text" id="nama" name="nama" placeholder="Nama" class="input">
            </div>
            
            <div class="input-group">
                <input type="text" id="email" name="email" placeholder="Email" class="input">
            </div>
            
    
            <input type="submit" value="Submit" class="btn">
        </form>
    </div>
    
</body>
</html>
```


https://github.com/syifaaurellia/Lab5web/assets/115867244/9c34b9f1-6e00-4b0d-b16b-2d7398947f17



## Selesai, Terima Kasih