# SSH

1. buat ssh key pada masing-masing server, kemudian ssh public key dari server ansible ke masing-masing server lainnya dengan cara ```ssh-copy-id -i .ssh/id_rsa.pub user@host```

![0](1.PNG)
![0](2.PNG)

2. Lakukan login ke server lainnya dari server ansible, dan tambahkan public key dari server frontend/backend ke akun github kita.

![0](3.PNG)
![0](4.PNG)
![0](5.PNG)