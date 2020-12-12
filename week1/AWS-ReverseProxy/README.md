# Dumbways Bootcamp DevOps
## Week 1
### AWS-Reverse Proxy


1. Update dan upgrade Server
   
   ![1](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-ReverseProxy/img/1.png)

   ![2](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-ReverseProxy/img/2.png)

2. Install nginx
   
   ![3](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-ReverseProxy/img/3.png)

3. Test nginx dengan mengakses IP Public via browser
   
   ![4](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-ReverseProxy/img/4.png)

4. buat direktori pada /etc/nginx/...
   
   ![5](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-ReverseProxy/img/5.png)

5. buat file config reverse proxy pada direktori yang baru dibuat. Lalu buka file tersebut
   
   ![6](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-ReverseProxy/img/6.png)

6. Lalu isi file tersebut seperti pada gambar dibawah. listen pada port 80, server_name menggunakan IP public, lalu pada location proxy_pass dimasukan IP private dari private instance dengan port 3000. 
   
   ![7](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-ReverseProxy/img/7.png)

7. Buka file konfigurasi nginx.conf, lalu tambahkan direktori yang baru dibuat. seperti pada gambar dibawah.
   
   ![9](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-ReverseProxy/img/9.png)

8. Untuk mengujinya buka browser dan akses IP public tanpa port.
   
   ![10](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-ReverseProxy/img/10.png)