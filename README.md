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

## 1. Installasi OPEN SSH SERVER
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
![5](https://github.com/user-attachments/assets/51dbafd6-661b-449c-adf9-6561d4781bf0)
![6 (2)](https://github.com/user-attachments/assets/9d176305-0c51-4fc8-b00d-89b805bb0651)
![7](https://github.com/user-attachments/assets/483c98b2-4a57-4aee-91bd-d04f646325b0)

## 2. Installasi MY-SQL SERVER
 **Langkah 1:Install mysql server dengan perintah**
```
sudo apt install mysql-server -y
```

**Langkah 2:Install tumpukan LAMP (Linux, Apache, MySQL, PHP) pada sistem operasi dengan perintah**
```
sudo apt install php libapache2-mod-php phpmysql
```

**Langkah 3:Membuka File Konfigurasi Direktori Apache dengan perintah**
```
sudo nano /etc/apache2/mods-enabled/dir.conf
```
- Tambahkan "index.php" pada di sebelah kanan "DirectoryIndex"
![13](https://github.com/user-attachments/assets/bc71d80c-e143-4286-87f4-263067b5e662)

**Langkah 4:Membuka file bernama “info.php” pada direktori var/www/html**
```
sudo nano /var/www/html/info.php
```
- isikan dengan code dibawah
```
<?php

phpinfo ();

?>
```


**Langkah 5:CEK KONFIGURASI**
- Buka pada google chrome pada windows <ip addres ubuntu server/info.php>
- cth :192.168.1.3/info.php
![17](https://github.com/user-attachments/assets/09d78e4b-6473-4435-9994-f8efce33b653)
![18](https://github.com/user-attachments/assets/c7119923-5f59-4e86-bb2a-3f155b4154c8)

## 3. Installasi APACHE2
**Langkah 1:Perbarui daftar paket dengan perintah**
```
sudo apt update
```

**Langkah 2:Installasi apache 2 dengan perintah**
```
sudo apt install apache2 -y
```
- samakan dengan foto di bawah

**Langkah 3:Memulai layanan server apahe2 dengan perintah**
```
sudo systemctl start apache2
```
**Langkah 4:4.	Lakukan pengecekan ip addres ubuntu server dengan perintah**
```
 ip add
```
**Langkah 5:5.	Buka pada browser google chrome pada windows dan ketikkan ip addres tadi “192.168.1.3”**
- contoh ip saya:192.168.1.3
  ![23](https://github.com/user-attachments/assets/a90e2a6c-dd81-4b99-a381-a4eb3c1e3f4b)

## 4. Installasi DATABASE SERVER
**Langkah 1:Installasi paket mariadb**
```
sudo apt-get update
sudo apt-get install mariadb-server
```

**Langkah 2:Untuk mengamankan installasi (Opsional)**
```
sudo mysql_secure_installation
```

**Langkah 3:Lakukan instalasi paket**
```
sudo apt-get install phpmyadmin
```

**Langkah 4:Restart ulang layanan**
```
sudo systemctl restart apache2
```
**Langkah 5:CEK KONFIGURASI**
5.	Buka pada browser windows gogole chrome dan ketikkan <ip address ubuntu server/phpmyadmin/> cth:192.168.1.3/phpmyadmin/ 

## 5.Installasi SAMBA
**Langkah 1:Memperbarui daftar paket dengan perintah**

```
sudo apt update
```
**Langkah 2:Menginstal paket vsftpd (Very Secure FTP Daemon) pada sistem Linux. Dengan perintah**
```
sudo apt-get install vsftpd
```
**Langkah 3:Membuat direktori baru bernama ‘sambashare” dengan perintah**

```
sudo mkdir /sambashare
```
**Langkah 4:Mengubah izin akses dengan perintah**
```
sudo chmod 0777  /sambasahre
```
**Langkah 5:Menambah pengguna baru bernama**
- cth: username “user1” dan membuat password ”0971”

```
sudo useradd user1
```
**Langkah 6:Mengedit file konfigurasi utama dengan perintah**
```
sudo nano /etc/samba/smb.conf
```
**Langkah 7:Memulai ulang layanan samba dengan perintah**
```
 sudo systemctl restart smbd
 sudo systemctl restart nmbd
```
**Langkah 8:Cek status dengan perintah “sudo systemctl status smbd” pastikan muncul tulisan “running”**
```
 sudo systemctl status smbd
```
**Langkah 9:Buka file eksplorer pada windows,dan pilih bagian “This PC” kemudian ketikkan pada taskbar atas ip add ubuntu server (192.168.1.3) lalu masukkan username dan passwd yang sudah di buat tadi**
