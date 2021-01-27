# Deployment

1. langkah pertama adalah menginstall Docker menggunakan ansible.

![0](1.PNG)
![0](2.PNG)

2. Install nodejs pada server frontend/backend dan lakukan ```npm install``` setelah itu install ```sequelize-cli```

![0](3.PNG)
![0](4.PNG)
![0](5.PNG)
![0](6.PNG)

3. pada server frontend rubah api dan arahkan ke backend, sementara pada backend rubah config database dan sesuaikan dengan database yang sudah dibuat pada bagian 5. Database, setelah lakukan migrasi database.

![0](7.PNG)
![0](8.PNG)

4. berikutnya buat Dockerfile dan build image backend untuk menjalankan image backend pada Docker container.

![0](9.PNG)
![0](10.PNG)
![0](11.PNG)

5. setelah semua step sudah selesai akses aplikasi melalui browser.

![0](12.PNG)

6. tambahkan SSL menggunakan let's encrypt agar website menjadi lebih aman.
![0](13.PNG)