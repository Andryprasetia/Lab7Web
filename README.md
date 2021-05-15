# Pemograman Web
~~~
Nama  : Andry Prasetia Perdana
NIM:  : 311910284
Kelas : TI19C1
~~~
# Menjalankan Web Server
Untuk menjalankan web server dari menu XAMPP Control.
![Screenshot (110)](https://user-images.githubusercontent.com/81818989/118352213-5c161f00-b58a-11eb-8f15-a1f032b900cc.png)
# Memulai PHP
Buat folder lab7_php_dasar pada root directory web server (d:\xampp\htdocs)
![Screenshot (111)](https://user-images.githubusercontent.com/81818989/118352226-764ffd00-b58a-11eb-88f8-3a1de0a3fd40.png)
Kemudia untuk mengakses direktory tersebut pada web server dengan mengakses URL: http://localhost/lab7_php_dasar/ 
![Screenshot (114)](https://user-images.githubusercontent.com/81818989/118352296-e78fb000-b58a-11eb-990b-b571acf8bd01.png)
# PHP Dasar
Buat file baru dengan nama php_dasar.php pada directory tersebut. Kemudian buat kode seperti berikut.
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>PHP Dasar</title>
</head>
<body>
    <h1>Belajar PHP Dasar</h1>
    <?php
        echo "Hello World";
    ?>
</body>
</html>
~~~
Kemudian untuk mengakses hasilnya melalui URL: http://localhost/lab7_php_dasar/php_dasar.php
![Screenshot (116)](https://user-images.githubusercontent.com/81818989/118352998-ac8f7b80-b58e-11eb-978f-94fd7e75af95.png)
# Variable PHP
Menambahkan variable pada program
~~~
<h2>Menggunakan Variable</h2>
    <?php
        $nim = "311910284";
        $nama = 'Andry Prasetia Perdana';
        echo "NIM : " . $nim . "<br>";
        echo "Nama : $nama";
    ?>
~~~
![Screenshot (117)](https://user-images.githubusercontent.com/81818989/118353076-03955080-b58f-11eb-9085-407a26d773a6.png)
# Predefine Variable $_GET
~~~
<h2>Predefine Variable</h2>
    <?php 
        echo 'Selamat Datang ' . $_GET['nama'];
    ?>
~~~
Untuk mengaksesnya gunakan URL: http://localhost/lab7_php_dasar/latihan2.php?nama=Andry
![Screenshot (118)](https://user-images.githubusercontent.com/81818989/118353089-0d1eb880-b58f-11eb-8ef2-06a4f7e08fdf.png)
# Membuat Form Input
~~~
<h2>Form Input</h2>
    <form method="post">
        <label>Nama: </label>
        <input type="text" name="nama">
        <input type="submit" value="Kirim">
    </form>
    <?php 
        echo 'Selamat Datang ' . $_POST['nama'];
    ?>
~~~
![Screenshot (119)](https://user-images.githubusercontent.com/81818989/118353111-20318880-b58f-11eb-81f0-ca2beff29adc.png)
# Operator
~~~
<h2>Operator</h2>
    <?php
        $gaji = 1000000;
![Uploading Screenshot (117).png…]()
        $pajak = 0.1;
        $thp = $gaji - ($gaji*$pajak);
            echo "Gaji sebelum pajak = Rp. $gaji <br>";
            echo "Gaji yang dibawa pulang = Rp. $thp";
    ?>
~~~
![Screenshot (120)](https://user-images.githubusercontent.com/81818989/118353152-40f9de00-b58f-11eb-8501-1033019877fb.png)
# Kondisi IF
~~~
<h2>Kondisi IF</h2>
    <?php
        $nama_hari = date("l");
            if ($nama_hari == "Sunday") {
        echo "Minggu";
            } elseif ($nama_hari == "Monday") {
        echo "Senin";
            } else {
        echo "Selasa";
        }
    ?>
~~~
![Screenshot (121)](https://user-images.githubusercontent.com/81818989/118353163-4c4d0980-b58f-11eb-9e1f-c3162e177675.png)
# Kondisi Switch
~~~
<h2>Kondisi Switch</h2>
    <?php
        $nama_hari = date("l");
            switch ($nama_hari) {
            case "Sunday":
        echo "Minggu";
            break;
            case "Monday":
    echo "Senin";
            break;
            case "Tuesday":
    echo "Selasa";
            break;
            default:
    echo "Sabtu";
            }
    ?>
~~~
![Screenshot (122)](https://user-images.githubusercontent.com/81818989/118353183-5c64e900-b58f-11eb-85cd-93644c18a602.png)
# Perulangan for
~~~
<h2>Perulangan For</h2>
    <?php
        echo "Perulangan 1 sampai 10 <br />";
            for ($i=1; $i<=10; $i++) {
        echo "Perulangan ke: " . $i . '<br />';
        }
        echo "Perulangan Menurun dari 10 ke 1 <br />";
            for ($i=10; $i>=1; $i--) {
        echo "Perulangan ke: " . $i . '<br />';
        }
    ?>
~~~
![Screenshot (123)](https://user-images.githubusercontent.com/81818989/118353194-671f7e00-b58f-11eb-912f-38163b3060da.png)
# Perulangan while
~~~
<h2>Perulangan While</h2>
    <?php
        echo "Perulangan 1 sampai 10 <br />";
            $i=1;
            while ($i<=10) {
        echo "Perulangan ke: " . $i . '<br />';
            $i++;
        }
    ?>
~~~
![Screenshot (124)](https://user-images.githubusercontent.com/81818989/118353197-71417c80-b58f-11eb-99be-f1cdfe15d36e.png)
# Perulangan dowhile
~~~
<h2>Perulangan Dowhile</h2>
    <?php
        echo "Perulangan 1 sampai 10 <br />";
            $i=1;
            do {
        echo "Perulangan ke: " . $i . '<br />';
            $i++;
            } while ($i<=10);
    ?>
~~~
![Screenshot (126)](https://user-images.githubusercontent.com/81818989/118353320-ef058800-b58f-11eb-99ed-ed4e1b330aa4.png)

# Pertanyaan dan Tugas
Buatlah program PHP sederhana dengan menggunakan form input yang menampilkan nama, tanggal lahir dan pekerjaan. Kemudian tampilkan outputnya dengan menghitung umur berdasarkan inputan tanggal lahir. Dan pilihan pekerjaan dengan gaji yang berbeda-beda sesuai pilihan pekerjaan.
~~~
<h2>Pertanyaan dan Tugas</h2>
    <form method="post">
            <label>Nama Lengkap: </label>
            <input type="text" name="nama">
            <br>
            <label>Tempat Lahir: </label>
            <input type="text" name="tempat_lahir">
            <br>
            <label>Tanggal Lahir: </label>
            <input type="date" name="tgl_lahir">
            <br>
            <label>Alamat: </label>
            <input type="text" name="alamat">
            <br>
            <label>Pekerjaan:
            <select name='pekerjaan'>
                <option value='Presiden'>Presiden</option>
                <option value='Mentri'>Mentri</option>
                <option value='Gubernur'>Gubernur</option>
                <option value='Bupati'>Bupati</option>
            </select>
            </label>
            <br>
            <input type="submit" value="Kirim">
    </form>
    <h2>Output</h2>
    <?php
        echo '<br> Nama Lengkap : ' . $_POST['nama'];
        echo '<br> Tempat Lahir : ' . $_POST['tempat_lahir'];
        echo '<br> Alamat : ' . $_POST['alamat'];
            $tgl_lahir = @$_POST['tgl_lahir'];
            $lahir = new DateTime($tgl_lahir);
            $hari_ini = new DateTime();
            $diff = $hari_ini->diff($lahir);
        echo "<br> Usia : ". $diff->y ." Tahun";
        echo "<br> Pekerjaan : ". $_POST['pekerjaan'];
            $pekerjaan = @$_POST['pekerjaan'];
            if($pekerjaan == "Presiden"){
                echo '<br> Gaji : Rp. 1.000.000.000,-';
            }
            elseif($pekerjaan == "Mentri"){
                echo '<br> Gaji : Rp. .500.000.000,-';
            }
            elseif($pekerjaan == "Gubernur"){
                echo '<br> Gaji : Rp. 250.000.000,-';
            }
            elseif($pekerjaan == "Bupati"){
                echo '<br> Gaji : Rp. 150.000.000,-';
            }
    ?>
~~~
![Screenshot (125)](https://user-images.githubusercontent.com/81818989/118352651-b6b07a80-b58c-11eb-994b-146d6bd4db18.png)

