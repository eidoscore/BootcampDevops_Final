# Web Server

1. Buka ip dari public dan disini dipastikan bahwa nginx belum terinstall pada server

![0](1.PNG)

cek koneksi kembali karna pada bagian user kita sudah membuat user baru dan login menggunakan akun yg sudah maka hasilnya akan unreachable ketika mencoba ping ke server lainnya, jadi kita perlu edit inventory dan file ansible.

![0](2.PNG)
![0](3.PNG)
![0](4.PNG)

2. pertama copy public key ansible server ke masing-masing server dan lakukan ping kembali.

![0](6.PNG)
![0](7.PNG)
![0](8.PNG)

3. lakukan update dan upgrade pada semua server.

![0](9.PNG)
![0](10.PNG)

4. kemudian install Nginx pada web server.

![0](11.PNG)
![0](12.PNG)

5. Rubah ip pada domain di dashboard cludflare dengan ip wev server kita.

![0](13.PNG)

6. lakukan reverse proxy server.

![0](14.PNG)
![0](15.PNG)