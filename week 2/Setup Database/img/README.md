# Dumbways Bootcamp DevOps
## Week 2
### Setup Database


1. Membuat Instance baru untuk database.
   
   ![1](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Setup%20Database/img/1.PNG)

2. Install mysql-server di instance Database.
   
   ![2](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Setup%20Database/img/2.PNG)
   
3. Login ke mysql dengan perintah "mysql -u root -p" lalu menambah user baru dan memberikan izin akses. 
   
   ![3](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Setup%20Database/img/3.PNG)

4. Mengubah IP Bind-address menjadi IP instance di directory /etc/mysql/mysql.conf.d.
   
   ![4](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Setup%20Database/img/4.PNG)
   
### Setup Mysql Client di Instance Backend

5. Instal MySQL Client di server backend yang sudah dibuat sudo apt-get install mysql-client.
   
   ![5](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Setup%20Database/img/5.PNG)

6. Remote login ke mysql yang ada di server database dari server backend degan perintah "mysql -u backend -h 172.31.50.109 -p".
   
   ![6](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%202/Setup%20Database/img/6.PNG)

