# Dumbways Bootcamp DevOps
## Week 1
### AWS-Create & Setup Server

### Step:
   1. Membuat VPC
   2. Membuat Instance Public
   3. Membuat Instance Private
   4. Membuat NAT Instance



### VPC

1. Buat VPC baru. Tentukan nama VPC dan CIDR block VPC.
   
   ![1]()

2. Buat subnet public. Klik create subnet.
   
   ![3]()

3. Pilih VPC yang digunakan, tentukan nama subnet public, dan tentukan CIDR block untuk subnet public.
   
   ![4]()

   ![5]()

4. Buat subnet private, tentukan nama subnet private, dan tenrukan CIDR block untuk subnet private.
   
   ![6]()

   ![7]()

5. Buat dan terapkan Intenet Gateway.
   
   ![8]()

6. Tentukan nama Internet Gateway yang dibuat. lalu attach ke VPC yang dibuat. 

   ![9]()

   ![10]()

   ![12]()

7. Buat Route untuk Subnet Public. Lalu berikan nama pada subnet public, dan tentukan nama VPC.
   
   ![13]()

   ![14]()

8. Tentukan routes ke internet, dengan target gateway yang sudah dibuat.

   ![15]()

   ![16]()

9. Associate route public ke subnet public

   ![17]()

   ![18]()

### Public Instance

1. Untuk membuat Instance, klik "Launch Virtual Machine".
   
   ![1]()

2. Tentukan Operating System yang akan digunakan.

   ![2]()

3. Tentukan instance type yang akan digunakan.

   ![3]()

4. Konfigurasi instance dengan network menggunakan VPC yang sudah dibuat, Subnet menggunakan subnet public yang baru dibuat, dan auto assign IP di-disable-kan

   ![4]()

5. Tentukan besaran storage yang digunakan

   ![5]()

6. (optional) memberikan tags pada instance.

   ![6]()

7. Tentukan security Group. Pada Instance public hanya SSH, HTTP, HTTPS.
   
   ![7]()

8. Lalu Launch Instance.

   ![8]()

9. Download keypair baru.

   ![9]()

10. Pada menu instance akan muncul instance yang sudah dibuat.

   ![11]()

11. Selanjutnya memberikan IP public pada Public Instance. Dengan menggunakan Elastic IP. Buat Elastic IP. 
   
   ![12]()

12. klik Allocate untuk merequest IP.
    
   ![13]()

13. Associate IP tersebut ke Public Instance.

   ![14]()

   ![15]()

14. Selanjutnya melakukan Remote ke Public Instance. Ubah hak akses keypair.

   ![16]()

15. Lalu remote public Instance dengan menggunakan keypair tersebut.

   ![17]()

   ![18]()

16. Tambahkan user pada public instance.

   ![19]()

17. Masukan user baru ke grup sudo, dan berikan akses super user.

   ![20]()

   ![21]()

18. Edit file konfigurasi ssh agar dapat melakukan remote tanpa keypair. Pada "PasswordAuthention" diubah menjadi "yes"

   ![22]()

   ![23]()

19. Restart service ssh.

   ![24]()

20. Lalu exit dari public Instance, dan remote dengan user yang baru dibuat tanpa keypair.

   ![25]()

   ![26]()

### Private Instance

1. Untuk membuat private instance langkah yang dilakukan seperti pada pembuatan public instance. Namun pada langkah konfigurasi instance dan security group sedikit berbeda. Pada konfigurasi instance Network menggunakan VPC yang sama dengan public instance, subnet menggunakan private subnet, dan auto assign public IP di-disable-kan. Pada private instance tidak akan menggunakan IP public.
   
   ![1]()

2. Lalu pada security group, type yang dipilih adalah "All Traffic" dan source yang digunakan merupakan public subnet.

   ![2]()

3. Setelah selesai pembuatan instance, selanjutnya melakukan remote. Remote dilakukan dari public instance, karena tidak dapat melakukan remote langsung ke private instance. Jadi pada public instance perlu menambahkan keypair terlebih dahulu. Buat file keypair dengan extention .pem.

   ![3]()

4. Lalu copy isi file keypair dari local (laptop), ke file yang baru dibuat.

   ![4]()

5. ubah hak akses keypair.

   ![5]()

6. Lakukan remote ke private instance dengan menggunakan IP yang diberikan dari subnet private dan keypair. 

   ![6]()

7. Tambahkan user untuk private instance.

   ![7]()

8. Masukan user baru ke grup sudo, dan berikan akses super user.

   ![8]()

   ![9]()

9. Edit file konfigurasi ssh agar dapat melakukan remote tanpa keypair. Pada "PasswordAuthention" diubah menjadi "yes"

   ![10]()

   ![11]()

10. Restart service ssh.

   ![12]()

11. Lalu exit dari public Instance, dan remote dengan user yang baru dibuat tanpa keypair.

   ![13]()

   ![14]()
 


### NAT Instance

1. Agar private instance dapat terkoneksi ke internet terdapat 2 cara, yaitu NAT gateway dan NAT instance. Untuk kali ini akan dilakukan NAT Instance. Yang pertama dilakukan adalah membuat instance baru dengan menggunakan AMIS (amzn-ami-vpc-nat....). Pada kali ini dipilih versi tahun 2017.
   
   ![1]()

2. Lalu memilih tipe instance

   ![2]()

3. Pada konfigurasi instance, network yang digunakan menggunakan VPC yang sama dengan instance public dan private. Subnet menggunakan public, dan auto assign public IP menggunakan enable. Bisa juga memilih disable tapi nanti perlu melakukan associate Elastic IP.

   ![3]()

4. Selajutnya security group, tipe yang dipilih adalah all traffic dan source nya adalah subnet private.

   ![4]()

5. Setelah selesai, pada menu instance klik instance NAT, lalu klik actions, networking, change source/destination check.
   
   ![6]()

6. Lalu centang pada "Stop", agar tidak ada pengecekan.
   
   ![7]()

7. Lalu buat route table untuk private route.

   ![8]()

8. Tentukan nama Route dan pilih VPC yang digunakan.
   
   ![9]()

9. Tambahkan route ke internet (0.0.0.0/0) dengan target NAT instance
    
   ![10]()

   ![11]()

10. Lalu edit subnet Associate dan tambahkan subnet private.
   ![12]()
   
      ![13]()

### Test Koneksi Internet

1. Lakukan ping dari public instance
   
   ![1]()

2. Lakukan ping dari public instance
   
   ![2]()