## Membuat Client-Server Manual
> **Nama Kelompok:**
> 1. Futra S Hutasoit (2010131210002)
> 2. Muhammad Iman Rizqullah (2010131210017)
> 3. Muhammad Riza Nugroho (2010131210005)

**1. Client Server pada Linux Virtual Box dengan Windows**
+ Langkah pertama buka Linuxnya di VirtualBox kemudian masuk ke super user dengan command “su” dan masukkan password Linuxnya. Jika authentication failure silahkan menggunakan command “sudo -i” dan masukkan password Linuxnya.
![Image](tugas1no1_1.png)
+ Setelah berhasil masuk ke super user buka wired settings dengan mengklik yang dilingkaran merah.
![Image](tugas1no1_2.png)
![Image](tugas1no1_3.png)
+ Karena kita akan menyetting secara manual jadi pilih yang manual. Untuk addresses sebagai percobaan sesuaikan saja dengan gambar atau bisa juga ip jaringannya diganti susuai keinginan. Perlu di perhatikan untuk ip jaringan address dan gatewaysebaiknya disamakan saja, pada gambar saya membuatnya 10 kemudian apply.
![Image](tugas1no1_4.png)
+ Untuk melihat ip addressnya jalankan command “ip a”, maka ip address yang sudah kita buat tadi akan tampil. 
![Image](tugas1no1_5.png)
+ Setelah itu buka VirtualBox lalu klik Host Network Manager lalu create host baru. Setelah menambahkan host buka properties dan klik adapter, karena kita menyettingnya secara manual jadi kita konfigurasi adapternya secara manual juga. Untuk IPv4 Addressnya isi sesuai ip getaway dan Ipv4 Network Mask yang kita buat di linux tadi. Jika anda mengikuti langkah-langkah sama dengan yang saya buat silahkan untuk disesuaikan dengan gambar jika sudah apply. 
![Image](tugas1no1_6.png)
![Image](tugas1no1_7.png)
+ Kemudian buka settings lalu pilih network, pada attached to pilih hot-only adapter dan host yang baru kita buat tadi lalu klik ok.
![Image](tugas1no1_8.png)
![Image](tugas1no1_9.png)
+ Sekarang kita mengatur IP Address yang ada di windows dengan cara membuka network connections kemudian klik host yang sudah kita buat tadi dan buka properties. Pada properties klik internet protocol version 4.
![Image](tugas1no1_10.png)
![Image](tugas1no1_11.png)
+ Pilih yang Use the Following IP Address lalu isi IP addres dengan getaway yang di linux tadi dan default getaway isi dengan IP Address yang ada di Linux, untuk subnet mask disamakan saja.
![Image](tugas1no1_12.png)
+ Untuk mengetahui berhasil atau tidaknya, ping ip windows di linux dengan cara “ping (IP Address windos)”. Supaya bisa berjalan pastikan fire wall & network protection dinonaktifkan.
![Image](tugas1no1_13.png)
![Image](tugas1no1_14.png)
![Image](tugas1no1_15.png)
![Image](tugas1no1_16.png)
+ Selanjutnya ping ip linux di windows dengan cara “ping (IP Address Linux)”.
![Image](tugas1no1_17.png)

**2. Client-Server pada 2 PC/Laptop menggunakan kabel LAN**
+ Langkah pertama adalah menghubungkan dua atau lebih device, boleh laptop atau PC dan satu di antaranya akan dijadikan sebagai server.
+ Di tutorial kali ini saya menggunakan dua device yaitu linux dan windows. Saya mengkonfigurasi IP nya secara manual, caranya kurang lebih seperti pada tutorial sebelumnya, untuk linux (server) bisa mengubah settingan di wired setting
![Image](tugas1no2_1.png)
![Image](tugas1no2_2.png)
![Image](tugas1no2_3.png)
![Image](tugas1no2_4.png)
+ Untuk windows (klien) bisa mengubah di **Advanced network settings** yang ada di windows
![Image](tugas1no2_5.PNG)
![Image](tugas1no2_6.PNG)
+ Pastikan port jaringan dan default gatewaynya sama
![Image](tugas1no2_7.PNG)
![Image](tugas1no2_8.PNG)
+ Selanjutnya mengubah settingan network di virtual box (server)
![Image](tugas1no2_9.png)
![Image](tugas1no2_10.png)
+ Tahap terakhir yaitu testing dengan cara ping IP Address clien dan servernya, server ping clien dan clien ping server. Pastikan sebelumnya windows firewall yang ada di windows non aktif.
![Image](tugas1no2_11.png)
![Image](tugas1no2_12.png)
+ Selamat anda telah berhasil.
