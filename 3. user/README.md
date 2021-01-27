# User Setting

1. akses instances yang sudah kita buat dan tambahkan user baru pada masing-masing server 

![0](2.PNG)

2. disable PAsswordauthentication pada ```sshd_config``` dan restart services dan relogin

![0](3.PNG)
![0](4.PNG)

3. buat ssh key dan tambahkan public key ke akun github kita 

![0](1.PNG)
![0](5.PNG)

4. lakukan test koneksi ke github dan clone ansbible repo menggunakan ssh

![0](6.PNG)

5. buat file ```inventory``` yang berisikan host masin-masing server, kemudian buat file ```ansible.cfg```

![0](7.PNG)
![0](8.PNG)

6. lakukan update pada server dan install ansible pada server ansible, setelah itu lakukan ping 

```ansible all -i inventory -m ping ```

![0](10.PNG)
![0](11.PNG)
![0](12.PNG)

7. Install aplikasi mkpasswd untuk encrytp password user, dan jalankan script untuk membuat user pada masing-masing server dan lakukan login ke server tujuan

![0](13.PNG)
![0](14.PNG)
![0](15.PNG)
