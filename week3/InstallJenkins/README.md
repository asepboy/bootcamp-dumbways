# Dumbways Bootcamp DevOps
## Week 3
### Install Jenkins

1. Buat instance baru untuk jenkins. Buat jaringan secara private, dan pastikan terkoneksi ke internet.
2. Lalu install Docker, dan docker compose seperti pada step sebelumnya.
3. Selanjutnya adalah menginstall Jenkins dengan menggunakan docker compose. Buat file docker-compose.yml lalu isi file tersebut seperti dibawah.
   
   ![1](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/InstallJenkins/img/1.png)

4. Lalu run docker-compose.yml
   
   ![2](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/InstallJenkins/img/2.png)

5. Selanjutnya membuat reverse proxy untuk Jenkins. Buat port 8080 menjadi 80. Pembuatan reverse proxy dilakukan di nginx, seperti pada gambar dibawah. Lalu restart nginx.

    ![3](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/InstallJenkins/img/3.png)

    ![4](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/InstallJenkins/img/4.png)

    ![5](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/InstallJenkins/img/5.png)

6. Lalu coba akses web jenkins menggunakan public IP.
   
   ![6](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/InstallJenkins/img/6.png)

7. Selanjutnya membuat Sub Domain dan SSL untuk web jenkins. Dengan ketentuan https://cicd.gilbran.instructype.com.
   
8. Buka dashboard cloudflare, lalu isi field sesuai ketentuan. Name diisi dengan Subdomain, dan IPv4 diisi IP Public, status proxy diganti DNS only.
   
   ![7](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/InstallJenkins/img/7.png)

9.  Lalu ubah rules reverse proxy pada nginx dengan mengubah server_name menjadi domain baru.
   
    ![8](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/InstallJenkins/img/8.png)

10. Lalu coba akses menggunakan browser dengan mengakses domain baru.
    
    ![9](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/InstallJenkins/img/9.png)

11. Membuat SSL untuk subdomain baru. Dengan menggunakan Certbot, karena sebelumnya sudah pernah melakukan configurasi SSL, maka disini saya hanya mendaftarkan domain baru tersebut.
    
    ![10](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/InstallJenkins/img/10.png)

    ![11](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/InstallJenkins/img/11.png)

12. Lalu Akses domain baru, dan cek apakah SSL sudah diterapkan atau belum.
    
    ![12](https://github.com/gilbranfairuz/Dumbways-Bootcamp-Devops/blob/master/week3/InstallJenkins/img/12.png)