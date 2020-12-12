# Dumbways Bootcamp DevOps
## Week 1
### AWS-SSL Configuration

1. Cek package update terakhir
   
   ![1](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-SSLConfiguration/img/1.png)

2. tambah repo ppa certbot
   
   ![2](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-SSLConfiguration/img/2.png)

3. Install certbot
   
   ![3](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-SSLConfiguration/img/3.png)

4. Daftarkan domain ke certbot. Lalu isikan email, agreement, dsb.
   
   ![4](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-SSLConfiguration/img/4.png)

5. Setelah selesai, cek pada konfigurasi reverse proxy (/etc/nginx/gilbran/gilbran.conf). Pastikan SSL telah diterapkan.

    ![9](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-SSLConfiguration/img/9.png)

6. Akses project menggunakan domain pada browser.

    ![10](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week1/AWS-SSLConfiguration/img/10.png)