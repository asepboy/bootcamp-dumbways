# Dumbways Bootcamp DevOps
## Week 1
### AWS-Reverse Proxy


1. Update dan upgrade Server
   
   ![1](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Reverse%20Proxy/img/1.PNG)

2. Install nginx
   
   ![2](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Reverse%20Proxy/img/2.PNG)

3. Test nginx dengan mengakses IP Public via browser
   
   ![3](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Reverse%20Proxy/img/3.PNG)
   ![4](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Reverse%20Proxy/img/4.PNG)

4. Edit Inbound rule untuk instance proxy 

    ![5](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Reverse%20Proxy/img/5.PNG)
    
5.  buat direktori pada /etc/nginx/...
   
   ![5](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Reverse%20Proxy/img/6.PNG)

6. buat file config reverse proxy pada direktori yang baru dibuat. Lalu buka file tersebut, Lalu isi file tersebut seperti pada gambar dibawah. listen pada port 80, server_name menggunakan IP public, lalu pada location proxy_pass dimasukan IP private dari private instance dengan port 3000.
   
   ![6](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Reverse%20Proxy/img/7.PNG)

7.  Buka file konfigurasi nginx.conf, lalu tambahkan direktori yang baru dibuat. seperti pada gambar dibawah.
   
   ![7](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Reverse%20Proxy/img/8.PNG)

8. Untuk mengujinya buka browser dan akses IP public tanpa port.
   
   ![8](https://github.com/asepboy/bootcamp-dumbways/blob/main/week%201/AWS%20-%20Reverse%20Proxy/img/9.PNG)
