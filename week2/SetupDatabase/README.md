# Dumbways Bootcamp DevOps
## Week 2
### Setup Database


1. Lakukan update dan upgrade pada instance database.
   

2. Install mysql kali ini tidak akan menggunakan metode apt, tetapi mendownload file .deb nya secara manual. Download terlebih dahulu file .deb dengan wget.
   
   ![3](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SetupDatabase/img/3.png)
   
   ![4](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SetupDatabase/img/5.png)
   
   ![5](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SetupDatabase/img/5.png)

3. Setelah itu install dengan command "dpkg -i". Lalu plih versi yang 5.7. 
   
   ![6](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SetupDatabase/img/6.png)

   ![7](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SetupDatabase/img/7.png)

   ![8](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SetupDatabase/img/8.png)

   ![9](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SetupDatabase/img/9.png)

4. Setelah menentukan versi mysql, install mysql-server dan mysql-client.
   
   ![10](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SetupDatabase/img/10.png)

5. Coba masuk ke mysql, dengan perintah "mysql -u root -p".
   
   ![11](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SetupDatabase/img/11.png)

6. Setelah masuk buat database untuk project.
   
   ![12](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SetupDatabase/img/12.png)

7. Buat user baru agar instance backend dapat melakukan remote database, tanpa menggunakan user root-nya.
   
   ![13](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SetupDatabase/img/13.png)   

8. Setup pada file mysqld.cnf pada line bind masukan IP instance database.
   
   ![15](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SetupDatabase/img/15.png)   

9. lakukan login database dari instance backend.
   
   ![14](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week2/SetupDatabase/img/14.png)   
