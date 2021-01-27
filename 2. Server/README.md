# Server Configuration

1. buat VPC baru berinama, disini saya berinama VPC-Master
    IPV4 : 10.10.0.0/16

![0](0.PNG)

2. buat private/public subnet
    Public Subnet : 10.10.2.0/24
    Private Subnet : 10.10.1.0/24

![0](1.PNG)
![0](2.PNG)

2. buat internet gateway baru, IG digunakan agar instances dapat terhubung ke internet

![0](3.PNG)

3. buat 2 Route table kemudian hubungkan masing-masing route ke ke VPC-MAster

![0](4-1.PNG)
![0](4-2.PNG)

4. asosiasikan route table yang sudah Public-RT ke Public Subnet

![0](5-1.PNG)
![0](5-2.PNG)

5. but Nat Gateway kemudian hubungkan Private-RT pada Nat Gateway tadi dengan cara diasosiasikan.

![0](6.PNG)
![0](7.PNG)

6. but Nat Gateway kemudian hubungkan Private-RT pada Nat Gateway tadi dengan cara diasosiasikan.

![0](8.PNG)

7. Buat Instance Baru Public Serveruntuk masing-masing server

![0](10.PNG)
![0](11.PNG)
![0](12.PNG)
![0](13.PNG)

buat elastic IP dan asosiasikan ke Public Instances yang baru dibuat agar memiliki ip yg tetap.

![0](14.PNG)

8. Buat Instances lainnya disini dibedakan hanya gunakan private subnet dan tambahkan security group berikut : 

![0](15.PNG)
![0](16.PNG)
![0](17.PNG)
![0](18.PNG)