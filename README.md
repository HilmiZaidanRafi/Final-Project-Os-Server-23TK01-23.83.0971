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

6. ## 1. Instalasi OPEN SSH Server
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

8. ## 2. Instalasi MYSQL SERVER
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

**Langkah 5: Cek status SSH SERVER**

```
sudo systemctl status ssh
```
**Langkah 6: Konfigurasi SHH SERVER**
```
Buka CMD pada windows,lakukan konfigurasi pada ubuntu dengan cara <ssh username ubuntu@ip address ubuntu server> contoh:ssh hilmiserver@192.168.1.3
setelah itu ketik manual "yes" dan masukkan password ubuntu server
```  
10. ## 3. Instalasi APACHE2
11. ## 4. Instalasi DATABASE SERVER
12. ## 5.Instalasi SAMBA
