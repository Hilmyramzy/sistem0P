Hilmy Syaddad Ramzy NurFauzan - 312210162 - TI22A1

[312210162_Hilmy_syaddad_Sistem_Operasi.pdf](https://github.com/user-attachments/files/17514362/312210162_Hilmy_syaddad_Sistem_Operasi.pdf)

Tugas pertemuan 7

Mencari Jumlah User

Menghitung Jumlah User di Sistem:

• Gunakan grep untuk mencari semua baris di file /etc/passwd yang memiliki informasi 
tentang user, lalu hitung jumlahnya.

Petunjuk: Gunakan pencarian yang relevan dengan direktori home untuk menghitung jumlah user.
• Jalankan perintah berikut untuk mencari semua baris di file /etc/passwd yang mengindikasikan 
user dengan direktori home:

- grep "/home" /etc/passwd | wc -l
- 
- grep "/home" /etc/passwd: Mencari baris yang memiliki "/home" sebagai direktori.
- 
- | wc -l: Menghitung jumlah baris yang dihasilkan oleh grep, yang mencerminkan 
jumlah user dengan direktori home.

• Menggunakan awk untuk Menghitung:
Gunakan awk untuk menghitung jumlah baris di file /etc/passwd yang mewakili user.
Petunjuk: Pastikan Anda menampilkan hanya nama user (kolom pertama) dan kemudian menghitung 
jumlahnya.

- -F:: Menentukan tanda pemisah kolom sebagai titik dua :.
- 
- {print $1}: Menampilkan kolom pertama (nama user).
- 
- | wc -l: Menghitung jumlah baris hasil dari awk, yaitu jumlah user.
Menampilkan Kolom di /etc/passwd:

Gunakan awk untuk menampilkan nama pengguna (kolom 1) dan direktori rumah pengguna (kolom 

6) di file /etc/passwd.
   
- $1: Kolom pertama (nama user).
- 
- $6: Kolom keenam (direktori home user).
- 
- Perintah ini akan menampilkan nama user diikuti dengan direktori home mereka.
- 
Menghitung Baris dengan Kata "error" di /var/log/syslog:

Gunakan grep untuk mencari dan menghitung jumlah baris yang mengandung kata "error" di file log 
tersebut.

- Sudo grep -i "error" /var/log/syslog | wc -


![Screenshot (402)](https://github.com/user-attachments/assets/588adc99-c6bb-4b1c-bcbc-b59631d50f50)

