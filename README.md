# Final-Project-Os-Server-23TK01-23.83.0971
- Nama:Muhammad Hilmi Zaidan Rafi
- Kelas:23TK01
- Mata Kuliah:OS SERVER dan SISTEM ADMIN

## Daftar Isi
1. [Installasi OPEN SSH SERVER](#1.-Installasi-OPEN-SSH-SERVER)
2. [Installasi MY-SQL SERVER](#2.-Installasi-MY-SQL-SERVER)
3. [Installasi APACHE2](#3.-Installasi-APACHE2)
4. [Installasi DATABASE SERVER](#4.-Installasi-DATABASE-SERVER)
5. [Installasi SAMBA](#5.-Installasi-SAMBA)

## 1. Instalasi OPEN SSH Server
**Langkah 1: Lakukan Instalasi Paket SSH Server**

```
sudo apt install openssh-server -y
```
**Langkah 2: Mengaktifkan Layanan ssh server**
```
sudo systemctl enable ssh
```
**Langkah 3: Memulai Layanan SSH SERVER**

```
sudo systemctl start ssh
```
**Langkah 4: Cek ip ubuntu server**
```
ip add
```
**Langkah 5: Cek status SSH SERVER**

```
sudo systemctl status ssh
```
**Langkah 6: Konfigurasi SHH SERVER**
```
Buka CMD pada windows,lakukan konfigurasi pada ubuntu dengan cara <ssh username ubuntu@ip address ubuntu server> contoh:ssh hilmiserver@192.168.1.3
setelah itu ketik manual "yes" dan masukkan password ubuntu server
```

## 2. Instalasi MYSQL SERVER
 **Langkah 1: 1.	Install mysql server dengan perintah**
```
sudo apt install mysql-server -y
```
**Langkah 2: 2.	Install tumpukan LAMP (Linux, Apache, MySQL, PHP) pada sistem operasi dengan perintah**
```
sudo apt install php libapache2-mod-php phpmysq
```
**Langkah 3: 3.	Membuka File Konfigurasi Direktori Apache dengan perintah**
```
sudo nano /etc/apache2/mods-enabled/dir.con
```
- Tambahkan "index.php" pada di sebelah kanan "DirectoryIndex"
  
**Langkah 4: Membuka file bernama “info.php” pada direktori var/www/html**
```
sudo nano /var/www/html/info.php
```
```
<?php

phpinfo ();

?>
```

**Langkah 5: CEK KONFIGURASI**
- Buka pada google chrome pada windows <ip addres ubuntu server/info.php>
- cth :192.168.1.3/info.php
  
## 3. Instalasi APACHE2
**Langkah 1:Installasi paket mariadb**
```
sudo apt-get update
sudo apt-get install mariadb-server
```

**Langkah 2:Untuk mengamankan installasi (Opsional)**
```
sudo mysql_secure_installation
```

**Langkah 3:Memulai layanan server apahe2 dengan perintah**
```
sudo systemctl start apache2
```

**Langkah 4:Lakukan pengecekan ip addres ubuntu server dengan perintah**
```
ip add
```
**Langkah 5:CEK KONFIGURASI**
- Buka pada browser google chrome pada windows dan ketikkan ip addres tadi “192.168.1.3”

## 4. Instalasi DATABASE SERVER
**Langkah 1:1.	Perbarui daftar paket dengan perintah**
```
sudo apt update
```

**Langkah 2:Installasi apache 2 dengan perintah**
```
sudo apt install apache2 -y
```
- samakan dengan foto di bawah
  
**Langkah 3:3.Lakukan instalasi paket**
```
sudo apt-get install phpmyadmin
```
-lakukan langkah seperti di foto:


**Langkah 4:Restart ulang layanan**
```
sudo systemctl restart apache2
```
**Langkah 5:CEK KONFIGURASI**
- 5.	Buka pada browser windows gogole chrome dan ketikkan <ip address ubuntu server/phpmyadmin/> cth:192.168.1.3/phpmyadmin/ 

## 5.Instalasi SAMBA
