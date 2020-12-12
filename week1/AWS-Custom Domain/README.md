# Dumbways Bootcamp DevOps
## Week 1
### AWS-Custom Domain


1. Buka dashboard cloudflare, lalu klik DNS, dan Add Route
   
   ![1](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Custom%20Domain/img/1.png)

2. Isi DNS management, Name disesuaikan, IPv4 menggunakan IP Publik dari Public Instance

   ![2](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Custom%20Domain/img/2.png)

3. Lalu buka konfigurasi reverse proxy.

    ![3](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Custom%20Domain/img/3.png)

4. Ubah server_name dengan domain yang baru sama dibuat.
   
   ![4](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Custom%20Domain/img/4.png)

5. Restart service nginx
   
   ![5](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Custom%20Domain/img/5.png)

6. Akses project dengan memasukan domain baru pada browser.

    ![6](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-Custom%20Domain/img/6.png)