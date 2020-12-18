# Dumbways Bootcamp DevOps
## Week 2
### Setup Database


1. Lakukan update dan upgrade pada instance database.
   

2. Install mysql kali ini tidak akan menggunakan metode apt, tetapi mendownload file .deb nya secara manual. Download terlebih dahulu file .deb dengan wget.
   
   ![3]()

   ![4]()

    ![4]()

3. Setelah itu install dengan command "dpkg -i". Lalu plih versi yang 5.7. 
   
   ![6]()

   ![7]()

   ![8]()

   ![9]()

4. Setelah menentukan versi mysql, install mysql-server dan mysql-client.
   
   ![10]()

5. Coba masuk ke mysql, dengan perintah "mysql -u root -p".
   
   ![11]()

6. Setelah masuk buat database untuk project.
   
   ![12]()

7. Buat user baru agar instance backend dapat melakukan remote database, tanpa menggunakan user root-nya.
   
   ![13]()   

8. Setup pada file mysqld.cnf pada line bind masukan IP instance database.
   
   ![15]()   

9. lakukan login database dari instance backend.
   
   ![14]()   
