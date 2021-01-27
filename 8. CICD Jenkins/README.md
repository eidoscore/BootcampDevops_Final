# CI/CD

1. Install jenkins menggunakan docker container pada server ansible

![0](1.PNG)

2. cek password default jenkins yang berjalan pada docker container.

![0](2.PNG)

3. Lakukan instalasi jenkins dan configurasi dasar jenkins seperti install plugin, membuat user dan lainnya.

![0](3.PNG)
![0](4.PNG)
![0](5.PNG)
![0](6.PNG)
![0](7.PNG)

4. pertama install plugin ```publish over ssh``` pada bagian plugin, dan ```install without restart``` 

![0](8.PNG)

5. tambahkan credential server pada jenkins agar bisa melakukan remote ke server backend/frontend

![0](9.PNG)
![0](10.PNG)
![0](11.PNG)
![0](12.PNG)
![0](13.PNG)

6. tambahkan server tujuan pada global config timeout set menjadi ```0``` dan lakukan test koneksi.

![0](14.PNG)
![0](15.PNG)

7. buat job baru pada jenkins pilih ```Freestyle project``` kemudian set seperti source code management dan trigger serta set notifikasi build.

![0](16.PNG)
![0](17.PNG)
![0](18.PNG)

8. pada step exec command perhatikan baik-baik ini adalah step penting perhatikan command yg diberikan.

![0](19.PNG)

9. cek history build yang sudah dilakukan.

![0](20.PNG)
![0](21.PNG)

10. langkah terakhir setelah berhasil melakukan build image dan running container maka image akan di push ke docker hub.

![0](22.PNG)