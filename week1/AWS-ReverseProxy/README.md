# Dumbways Bootcamp DevOps
## Week 1
### AWS-Reverse Proxy


1. Update dan upgrade Server
   
   ![1]()

   ![2]()

2. Install nginx
   
   ![3]()

3. Test nginx dengan mengakses IP Public via browser
   
   ![4]()

4. buat direktori pada /etc/nginx/...
   
   ![5]()

5. buat file config reverse proxy pada direktori yang baru dibuat. Lalu buka file tersebut
   
   ![6]()

6. Lalu isi file tersebut seperti pada gambar dibawah. listen pada port 80, server_name menggunakan IP public, lalu pada location proxy_pass dimasukan IP private dari private instance dengan port 3000. 
   
   ![7]()

7. Buka file konfigurasi nginx.conf, lalu tambahkan direktori yang baru dibuat. seperti pada gambar dibawah.
   
   ![9]()

8. Untuk mengujinya buka browser dan akses IP public tanpa port.
   
   ![10]()