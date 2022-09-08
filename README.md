# cs-assignment-7

## IDOR

Menganalisa halaman dashboard terdapat
- Grid untuk menampilkan data barang
- terdapat tombol tambah barang
- terdapat tombol edit dan delete

Melakukan analisa semua halaman dashboard dengan mengguknakan burp suite


![image](https://user-images.githubusercontent.com/6330046/189142548-fcda0905-c57b-439c-9cf5-ad45a1da5bb0.png)


didapatkan 2 url yang berpotensi terhadapat IDOR yaitu

http://157.245.157.217/pertemuan7/user/edit_data.php?id=8
http://157.245.157.217/pertemuan7/user/delete_data.php?id=9

mencoba meng exploit dengan mengganti i pada halaman edit

http://157.245.157.217/pertemuan7/user/edit_data.php?id=2


![image](https://user-images.githubusercontent.com/6330046/189142869-f92d4e18-bd61-4f08-80ca-0d8f0e1c2d6b.png)


dapat mengakses databarang yang lain

## Host Header

Menganalisa halaman depan user didapatkan beberapa fitur

- Login 
- Register
- Forgot password

karena kerentanan host header paling berpotensi paa forgot password maka dicoba mengganti host hheader ketika submit forgot password dengan menggunakan burp suite sehingga diperoleh hasil sebagai berikut

![image](https://user-images.githubusercontent.com/6330046/189152869-3f5409e5-3d08-4d39-a866-05f1df20c3f6.png)



