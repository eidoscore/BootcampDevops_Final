# Database Server

1. jalankan script berikut untuk membuat galeraDatabase Cluster pada server database

![0](1.PNG)
![0](2.PNG)
![0](3.PNG)

2. kemudian jalankan akses database yang berjalan pada container docker, untuk proses proses instalasi docker ada pada step 7. Deployment.

![0](4.PNG)

3. selanjutnya Haproxy untuk melakukan load balancing database, dan tambahkan script balancing pada ```haproxy.cfg``` kemudian restart service

![0](5.PNG)
![0](6.PNG)
![0](7.PNG)

4. akses database melalui server backend, pertama install mysql client dan renote database.

![0](8.PNG)
![0](5.PNG)