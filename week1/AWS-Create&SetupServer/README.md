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
   
   ![1](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/VPC/1.png)

2. Buat subnet public. Klik create subnet.
   
   ![3](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/VPC/3.png)

3. Pilih VPC yang digunakan, tentukan nama subnet public, dan tentukan CIDR block untuk subnet public.
   
   ![4](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/VPC/4.png)

   ![5](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/VPC/5.png)

4. Buat subnet private, tentukan nama subnet private, dan tenrukan CIDR block untuk subnet private.
   
   ![6](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/VPC/6.png)

   ![7](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/VPC/7.png)

5. Buat dan terapkan Intenet Gateway.
   
   ![8](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/VPC/8.png)

6. Tentukan nama Internet Gateway yang dibuat. lalu attach ke VPC yang dibuat. 

   ![9](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/VPC/9.png)

   ![10](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/VPC/10.png)

   ![12](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/VPC/12.png)

7. Buat Route untuk Subnet Public. Lalu berikan nama pada subnet public, dan tentukan nama VPC.
   
   ![13](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/VPC/13.png)

   ![14](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/VPC/14.png)

8. Tentukan routes ke internet, dengan target gateway yang sudah dibuat.

   ![15](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/VPC/15.png)

   ![16](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/VPC/16.png)

9. Associate route public ke subnet public

   ![17](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/VPC/17.png)

   ![18](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/VPC/18.png)

### Public Instance

1. Untuk membuat Instance, klik "Launch Virtual Machine".
   
   ![1](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/1.png)

2. Tentukan Operating System yang akan digunakan.

   ![2](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/2.png)

3. Tentukan instance type yang akan digunakan.

   ![3](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/3.png)

4. Konfigurasi instance dengan network menggunakan VPC yang sudah dibuat, Subnet menggunakan subnet public yang baru dibuat, dan auto assign IP di-disable-kan

   ![4](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/4.png)

5. Tentukan besaran storage yang digunakan

   ![5](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/5.png)

6. (optional) memberikan tags pada instance.

   ![6](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/6.png)

7. Tentukan security Group. Pada Instance public hanya SSH, HTTP, HTTPS.
   
   ![7](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/7.png)

8. Lalu Launch Instance.

   ![8](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/8.png)

9. Download keypair baru.

   ![9](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/9.png)

10. Pada menu instance akan muncul instance yang sudah dibuat.

   ![11](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/11.png)

11. Selanjutnya memberikan IP public pada Public Instance. Dengan menggunakan Elastic IP. Buat Elastic IP. 
   
   ![12](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/12.png)

12. klik Allocate untuk merequest IP.
    
   ![13](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/13.png)

13. Associate IP tersebut ke Public Instance.

   ![14](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/14.png)

   ![15](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/15.png)

14. Selanjutnya melakukan Remote ke Public Instance. Ubah hak akses keypair.

   ![16](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/16.png)

15. Lalu remote public Instance dengan menggunakan keypair tersebut.

   ![17](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/17.png)

   ![18](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/18.png)

16. Tambahkan user pada public instance.

   ![19](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/19.png)

17. Masukan user baru ke grup sudo, dan berikan akses super user.

   ![20](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/20.png)

   ![21](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/21.png)

18. Edit file konfigurasi ssh agar dapat melakukan remote tanpa keypair. Pada "PasswordAuthention" diubah menjadi "yes"

   ![22](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/22.png)

   ![23](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/23.png)

19. Restart service ssh.

   ![24](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/24.png)

20. Lalu exit dari public Instance, dan remote dengan user yang baru dibuat tanpa keypair.

   ![25](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/25.png)

   ![26](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/public/26.png)

### Private Instance

1. Untuk membuat private instance langkah yang dilakukan seperti pada pembuatan public instance. Namun pada langkah konfigurasi instance dan security group sedikit berbeda. Pada konfigurasi instance Network menggunakan VPC yang sama dengan public instance, subnet menggunakan private subnet, dan auto assign public IP di-disable-kan. Pada private instance tidak akan menggunakan IP public.
   
   ![1](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/private/1.png)

2. Lalu pada security group, type yang dipilih adalah "All Traffic" dan source yang digunakan merupakan public subnet.

   ![2](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/private/2.png)

3. Setelah selesai pembuatan instance, selanjutnya melakukan remote. Remote dilakukan dari public instance, karena tidak dapat melakukan remote langsung ke private instance. Jadi pada public instance perlu menambahkan keypair terlebih dahulu. Buat file keypair dengan extention .pem.

   ![3](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/private/3.png)

4. Lalu copy isi file keypair dari local (laptop), ke file yang baru dibuat.

   ![4](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/private/4.png)

5. ubah hak akses keypair.

   ![5](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/private/5.png)

6. Lakukan remote ke private instance dengan menggunakan IP yang diberikan dari subnet private dan keypair. 

   ![6](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/private/6.png)

7. Tambahkan user untuk private instance.

   ![7](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/private/7.png)

8. Masukan user baru ke grup sudo, dan berikan akses super user.

   ![8](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/private/8.png)

   ![9](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/private/9.png)

9. Edit file konfigurasi ssh agar dapat melakukan remote tanpa keypair. Pada "PasswordAuthention" diubah menjadi "yes"

   ![10](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/private/10.png)

   ![11](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/private/11.png)

10. Restart service ssh.

   ![12](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/private/12.png)

11. Lalu exit dari public Instance, dan remote dengan user yang baru dibuat tanpa keypair.

   ![13](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/private/13.png)

   ![14](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/private/14.png)
 


### NAT Instance

1. Agar private instance dapat terkoneksi ke internet terdapat 2 cara, yaitu NAT gateway dan NAT instance. Untuk kali ini akan dilakukan NAT Instance. Yang pertama dilakukan adalah membuat instance baru dengan menggunakan AMIS (amzn-ami-vpc-nat....). Pada kali ini dipilih versi tahun 2017.
   
   ![1](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/NATInstances/1.png)

2. Lalu memilih tipe instance

   ![2](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/NATInstances/2.png)

3. Pada konfigurasi instance, network yang digunakan menggunakan VPC yang sama dengan instance public dan private. Subnet menggunakan public, dan auto assign public IP menggunakan enable. Bisa juga memilih disable tapi nanti perlu melakukan associate Elastic IP.

   ![3](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/NATInstances/3.png)

4. Selajutnya security group, tipe yang dipilih adalah all traffic dan source nya adalah subnet private.

   ![4](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/NATInstances/4.png)

5. Setelah selesai, pada menu instance klik instance NAT, lalu klik actions, networking, change source/destination check.
   
   ![6](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/NATInstances/6.png)

6. Lalu centang pada "Stop", agar tidak ada pengecekan.
   
   ![7](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/NATInstances/7.png)

7. Lalu buat route table untuk private route.

   ![8](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/NATInstances/8.png)

8. Tentukan nama Route dan pilih VPC yang digunakan.
   
   ![9](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/NATInstances/9.png)

9. Tambahkan route ke internet (0.0.0.0/0) dengan target NAT instance
    
   ![10](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/NATInstances/10.png)

   ![11](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/NATInstances/11.png)

10. Lalu edit subnet Associate dan tambahkan subnet private.
   ![12](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/NATInstances/12.png)
   
      ![13](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/NATInstances/13.png)

### Test Koneksi Internet

1. Lakukan ping dari public instance
   
   ![1](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/TestKoneksiInternet/1.png)

2. Lakukan ping dari public instance
   
   ![2](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Create%26SetupServer/img/TestKoneksiInternet/2.png)