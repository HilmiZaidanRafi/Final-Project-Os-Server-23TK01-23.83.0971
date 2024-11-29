# Final-Project-Os-Server-23TK01-23.83.0971
- Nama:Muhammad Hilmi Zaidan Rafi
- Kelas:23TK01
- Mata Kuliah:OS SERVER dan SISTEM ADMIN

## Daftar Isi
1. [Installasi OPEN SSH SERVER](#1.-Instalasi-OPEN-SSH-SERVER)
2. [Installasi MY-SQL SERVER](#2.-Instalasi-MYSQL-SERVER)
3. [Installasi APACHE2](#3.-Instalasi-APACHE2)
4. [Installasi DATABASE SERVER](#4.-Instalasi-DATABASE-SERVER)
5. [Installasi SAMBA](#5.-Instalasi-SAMBA)

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
**Langkah 5: LaCek status SSH SERVER**

```
sudo systemctl status ssh
```
**Langkah 6: Konfigurasi SHH SERVER**
Buka CMD pada windows,lakukan konfigurasi pada ubuntu dengan cara <ssh username ubuntu@ip address ubuntu server> contoh:ssh hilmiserver@192.168.1.3
setelah itu ketik manual "yes" dan masukkan password ubuntu server


8. ## 2. Instalasi MYSQL SERVER
9. ## 3. Instalasi APACHE2
10. ## 4. Instalasi DATABASE SERVER
11. ## 5.Instalasi SAMBA
